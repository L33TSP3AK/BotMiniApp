# Grid System

<BackToAdmin />

<div class="threat-container">
  <div class="cyber-grid"></div>
  <div class="map-header">
    <h1 class="neon-text">CYBER THREAT MAP</h1>
    <div class="cyber-line"></div>
    <div class="stats-bar">
      <div class="stat">
        <span class="label">ACTIVE THREATS</span>
        <span class="value" id="activeThreats">0</span>
      </div>
      <div class="stat">
        <span class="label">ATTACKS/MIN</span>
        <span class="value" id="attacksPerMin">0</span>
      </div>
      <div class="stat">
        <span class="label">TOP TARGET</span>
        <span class="value" id="topTarget">USA</span>
      </div>
    </div>
  </div>

  <div class="map-container">
    <canvas id="threatMap"></canvas>
    <div class="attack-list" id="attackList"></div>
  </div>

  <div class="legend">
    <div class="legend-item">
      <span class="dot attack"></span>
      <span>Attack Origin</span>
    </div>
    <div class="legend-item">
      <span class="dot target"></span>
      <span>Target Location</span>
    </div>
    <div class="legend-item">
      <span class="line"></span>
      <span>Attack Path</span>
    </div>
  </div>
</div>

<script setup>
import { onMounted, onUnmounted } from 'vue'

// Map initialization and rendering
onMounted(() => {
  const canvas = document.getElementById('threatMap')
  const ctx = canvas.getContext('2d')
  const attackList = document.getElementById('attackList')
  const activeThreats = document.getElementById('activeThreats')
  const attacksPerMin = document.getElementById('attacksPerMin')
  
  // Set canvas size
  function resize() {
    canvas.width = canvas.offsetWidth
    canvas.height = canvas.offsetHeight
  }
  
  resize()
  window.addEventListener('resize', resize)

  // Define major countries/regions with coordinates for outlines
  const countries = {
    USA: {
      color: '#00ff00',
      points: [
        {x: 0.15, y: 0.25}, {x: 0.25, y: 0.25},
        {x: 0.25, y: 0.35}, {x: 0.15, y: 0.35}
      ]
    },
    China: {
      color: '#ff0000',
      points: [
        {x: 0.65, y: 0.3}, {x: 0.75, y: 0.3},
        {x: 0.75, y: 0.4}, {x: 0.65, y: 0.4}
      ]
    },
    Russia: {
      color: '#ffff00',
      points: [
        {x: 0.55, y: 0.2}, {x: 0.75, y: 0.2},
        {x: 0.75, y: 0.3}, {x: 0.55, y: 0.3}
      ]
    },
    EU: {
      color: '#00ffff',
      points: [
        {x: 0.45, y: 0.25}, {x: 0.55, y: 0.25},
        {x: 0.55, y: 0.35}, {x: 0.45, y: 0.35}
      ]
    },
    India: {
      color: '#ff00ff',
      points: [
        {x: 0.6, y: 0.35}, {x: 0.7, y: 0.35},
        {x: 0.7, y: 0.45}, {x: 0.6, y: 0.45}
      ]
    },
    Brazil: {
      color: '#00ff00',
      points: [
        {x: 0.25, y: 0.5}, {x: 0.35, y: 0.5},
        {x: 0.35, y: 0.6}, {x: 0.25, y: 0.6}
      ]
    }
  }

  // Convert country coordinates to attack points
  const attackPoints = Object.entries(countries).map(([name, data]) => {
    const centerX = data.points.reduce((sum, p) => sum + p.x, 0) / data.points.length
    const centerY = data.points.reduce((sum, p) => sum + p.y, 0) / data.points.length
    return { x: centerX, y: centerY, name }
  })

  // Active attacks
  let attacks = []
  let threatCount = 0
  let attackRate = 0
  let topTargetCount = {}

  // Generate random attack
  function generateAttack() {
    const origin = attackPoints[Math.floor(Math.random() * attackPoints.length)]
    const target = attackPoints[Math.floor(Math.random() * attackPoints.length)]
    
    // Update target statistics
    topTargetCount[target.name] = (topTargetCount[target.name] || 0) + 1
    
    // Update top target display
    const topTarget = Object.entries(topTargetCount)
      .sort(([,a], [,b]) => b - a)[0]
    if (topTarget) {
      document.getElementById('topTarget').textContent = topTarget[0]
    }
    
    return {
      origin: {
        x: origin.x * canvas.width,
        y: origin.y * canvas.height
      },
      target: {
        x: target.x * canvas.width,
        y: target.y * canvas.height
      },
      targetName: target.name,
      progress: 0,
      type: ['DDoS', 'Malware', 'Ransomware', 'Data Breach'][Math.floor(Math.random() * 4)]
    }
  }

  // Add attack to list
  function addAttackToList(attack) {
    const item = document.createElement('div')
    item.className = 'attack-item'
    item.innerHTML = `
      <span class="attack-type">${attack.type} → ${attack.targetName}</span>
      <span class="attack-progress"></span>
    `
    attackList.prepend(item)
    
    // Remove old items
    if (attackList.children.length > 5) {
      attackList.removeChild(attackList.lastChild)
    }
  }

  // Animation loop
  function animate() {
    // Clear canvas
    ctx.fillStyle = 'rgba(0, 0, 0, 0.1)'
    ctx.fillRect(0, 0, canvas.width, canvas.height)

    // Draw country outlines
    Object.entries(countries).forEach(([name, data]) => {
      ctx.beginPath()
      data.points.forEach((point, index) => {
        const x = point.x * canvas.width
        const y = point.y * canvas.height
        if (index === 0) {
          ctx.moveTo(x, y)
        } else {
          ctx.lineTo(x, y)
        }
      })
      // Close the path
      const first = data.points[0]
      ctx.lineTo(first.x * canvas.width, first.y * canvas.height)
      
      ctx.strokeStyle = data.color
      ctx.lineWidth = 2
      ctx.stroke()
      
      // Fill with semi-transparent color
      ctx.fillStyle = data.color.replace(')', ', 0.1)')
      ctx.fill()
    })
    
    
    // Update and draw attacks
    attacks = attacks.filter(attack => {
      attack.progress += 0.01
      
      if (attack.progress >= 1) {
        return false
      }
      
      // Calculate current position
      const x = attack.origin.x + (attack.target.x - attack.origin.x) * attack.progress
      const y = attack.origin.y + (attack.target.y - attack.origin.y) * attack.progress
      
      // Draw attack path
      ctx.beginPath()
      ctx.moveTo(attack.origin.x, attack.origin.y)
      ctx.lineTo(x, y)
      ctx.strokeStyle = `rgba(0, 255, 0, ${1 - attack.progress})`
      ctx.stroke()
      
      // Draw attack point
      ctx.beginPath()
      ctx.arc(x, y, 3, 0, Math.PI * 2)
      ctx.fillStyle = '#ff0000'
      ctx.fill()
      
      return true
    })
    
    // Generate new attacks
    if (Math.random() < 0.05) {
      const attack = generateAttack()
      attacks.push(attack)
      addAttackToList(attack)
      threatCount++
      attackRate = Math.min(attackRate + 1, 120)
    }
    
    // Update stats
    activeThreats.textContent = attacks.length
    attacksPerMin.textContent = attackRate
    
    requestAnimationFrame(animate)
  }
  
  // Start animation
  animate()
  
  // Update attack rate
  setInterval(() => {
    attackRate = Math.max(attackRate - 1, 0)
  }, 1000)
  
  // Cleanup
  onUnmounted(() => {
    window.removeEventListener('resize', resize)
  })
})
</script>

<style>
.threat-container {
  position: relative;
  padding: 2rem;
  background: linear-gradient(45deg, #000, #1a1a1a);
  border-radius: 1rem;
  margin: 2rem 0;
  overflow: hidden;
}

.cyber-grid {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: 
    linear-gradient(90deg, rgba(0, 255, 0, 0.1) 1px, transparent 1px),
    linear-gradient(rgba(0, 255, 0, 0.1) 1px, transparent 1px);
  background-size: 20px 20px;
  animation: gridScroll 20s linear infinite;
  pointer-events: none;
}

.map-header {
  text-align: center;
  margin-bottom: 2rem;
  position: relative;
  z-index: 1;
}

.neon-text {
  font-size: 3rem;
  color: #00ff00;
  text-shadow: 
    0 0 5px #00ff00,
    0 0 10px #00ff00,
    0 0 20px #00ff00;
  margin: 0;
}

.cyber-line {
  height: 2px;
  background: linear-gradient(90deg, transparent, #00ff00, transparent);
  margin: 1rem auto;
  width: 200px;
}

.stats-bar {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 1rem;
}

.stat {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 0.5rem;
}

.stat .label {
  color: #666;
  font-size: 0.8rem;
  font-family: monospace;
}

.stat .value {
  color: #00ff00;
  font-size: 1.5rem;
  font-family: monospace;
  font-weight: bold;
}

.map-container {
  position: relative;
  height: 400px;
  margin: 2rem 0;
  background: rgba(0, 0, 0, 0.5);
  border: 1px solid #00ff00;
  border-radius: 0.5rem;
  overflow: hidden;
}

#threatMap {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.attack-list {
  position: absolute;
  top: 1rem;
  right: 1rem;
  width: 200px;
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid #00ff00;
  border-radius: 0.5rem;
  padding: 0.5rem;
}

.attack-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.5rem;
  border-bottom: 1px solid rgba(0, 255, 0, 0.2);
  color: #00ff00;
  font-family: monospace;
  font-size: 0.8rem;
}

.attack-item:last-child {
  border-bottom: none;
}

.attack-type {
  color: #ff0000;
}

.legend {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 1rem;
}

.attack-type {
  color: #ff0000;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.legend-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  color: #666;
  font-size: 0.8rem;
  white-space: nowrap;
}

.dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
}

.dot.attack {
  background: #ff0000;
}

.dot.target {
  background: #00ff00;
}

.line {
  width: 20px;
  height: 2px;
  background: #00ff00;
}

@keyframes gridScroll {
  0% { transform: translate(0, 0); }
  100% { transform: translate(20px, 20px); }
}
</style>