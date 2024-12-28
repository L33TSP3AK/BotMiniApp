# Advanced Operations

<div class="neural-container">
  <canvas id="neuralCanvas"></canvas>
  <div class="overlay-content">
    <h1 class="cyber-title">ADVANCED OPS</h1>
    <div class="system-stats">
      <div class="stat">
        <span class="label">SYSTEM LOAD</span>
        <span class="value">87%</span>
      </div>
      <div class="stat">
        <span class="label">NETWORK</span>
        <span class="value">SECURE</span>
      </div>
      <div class="stat">
        <span class="label">STATUS</span>
        <span class="value">ACTIVE</span>
      </div>
    </div>
  </div>
</div>

## Operation Modules

<div class="ops-grid">
  <div class="ops-card" data-priority="high">
    <div class="card-header">
      <div class="priority-indicator"></div>
      <h3>Critical Operations</h3>
    </div>
    <div class="card-content">
      <ul>
        <li>System Infiltration</li>
        <li>Data Extraction</li>
        <li>Trace Removal</li>
      </ul>
    </div>
    <div class="card-footer">
      <div class="status">ACTIVE</div>
      <div class="timestamp">00:00:00</div>
    </div>
  </div>

  <div class="ops-card" data-priority="medium">
    <div class="card-header">
      <div class="priority-indicator"></div>
      <h3>Tactical Operations</h3>
    </div>
    <div class="card-content">
      <ul>
        <li>Network Analysis</li>
        <li>Pattern Recognition</li>
        <li>Automated Response</li>
      </ul>
    </div>
    <div class="card-footer">
      <div class="status">STANDBY</div>
      <div class="timestamp">00:00:00</div>
    </div>
  </div>

  <div class="ops-card" data-priority="low">
    <div class="card-header">
      <div class="priority-indicator"></div>
      <h3>Support Operations</h3>
    </div>
    <div class="card-content">
      <ul>
        <li>Resource Management</li>
        <li>System Maintenance</li>
        <li>Log Analysis</li>
      </ul>
    </div>
    <div class="card-footer">
      <div class="status">READY</div>
      <div class="timestamp">00:00:00</div>
    </div>
  </div>
</div>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  const canvas = document.getElementById('neuralCanvas')
  if (!canvas) return
  if (!canvas.getContext) return
  
  const ctx = canvas.getContext('2d')
  if (!ctx) return
  
  // Set canvas size
  function resize() {
    if (!canvas || !ctx) return
    canvas.width = canvas.offsetWidth
    canvas.height = canvas.offsetHeight
  }
  
  resize()
  window.addEventListener('resize', resize)
  
  // Neural network nodes
  const nodes = []
  const connections = []
  const nodeCount = 50
  
  // Create nodes
  for (let i = 0; i < nodeCount; i++) {
    nodes.push({
      x: Math.random() * canvas.width,
      y: Math.random() * canvas.height,
      vx: (Math.random() - 0.5) * 2,
      vy: (Math.random() - 0.5) * 2
    })
  }
  
  // Create connections
  for (let i = 0; i < nodes.length; i++) {
    for (let j = i + 1; j < nodes.length; j++) {
      if (Math.random() < 0.1) {
        connections.push([i, j])
      }
    }
  }
  
  // Animation loop
  function animate() {
    ctx.fillStyle = 'rgba(0, 0, 0, 0.1)'
    ctx.fillRect(0, 0, canvas.width, canvas.height)
    
    // Update nodes
    nodes.forEach(node => {
      node.x += node.vx
      node.y += node.vy
      
      if (node.x < 0 || node.x > canvas.width) node.vx *= -1
      if (node.y < 0 || node.y > canvas.height) node.vy *= -1
      
      ctx.fillStyle = '#00ff00'
      ctx.beginPath()
      ctx.arc(node.x, node.y, 2, 0, Math.PI * 2)
      ctx.fill()
    })
    
    // Draw connections
    ctx.strokeStyle = 'rgba(0, 255, 0, 0.1)'
    ctx.lineWidth = 1
    connections.forEach(([i, j]) => {
      ctx.beginPath()
      ctx.moveTo(nodes[i].x, nodes[i].y)
      ctx.lineTo(nodes[j].x, nodes[j].y)
      ctx.stroke()
    })
    
    requestAnimationFrame(animate)
  }
  
  animate()
})
</script>

<style>
.neural-container {
  position: relative;
  height: 300px;
  margin: 2rem 0;
  border-radius: 1rem;
  overflow: hidden;
  background: #000;
}

#neuralCanvas {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.overlay-content {
  position: relative;
  z-index: 1;
  padding: 2rem;
  color: #00ff00;
}

.cyber-title {
  font-size: 3rem;
  text-align: center;
  margin: 0;
  text-shadow: 0 0 10px #00ff00;
  animation: glitch 1s infinite;
}

.system-stats {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 2rem;
}

.stat {
  text-align: center;
}

.stat .label {
  display: block;
  font-size: 0.8rem;
  color: #666;
  margin-bottom: 0.5rem;
}

.stat .value {
  font-size: 1.2rem;
  font-weight: bold;
  color: #00ff00;
}

.ops-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.ops-card {
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid;
  border-radius: 0.5rem;
  overflow: hidden;
}

.ops-card[data-priority="high"] { border-color: #ff0000; }
.ops-card[data-priority="medium"] { border-color: #ffff00; }
.ops-card[data-priority="low"] { border-color: #00ff00; }

.card-header {
  padding: 1rem;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  align-items: center;
  gap: 1rem;
}

.priority-indicator {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: currentColor;
  animation: blink 1s infinite;
}

.card-content {
  padding: 1rem;
}

.card-content ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.card-content li {
  padding: 0.5rem 0;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.card-footer {
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.status {
  color: #00ff00;
  font-family: monospace;
}

.timestamp {
  font-family: monospace;
  color: #666;
}

@keyframes blink {
  0% { opacity: 1; }
  50% { opacity: 0.3; }
  100% { opacity: 1; }
}
</style>