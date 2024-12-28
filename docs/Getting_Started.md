# Getting Started

<div class="welcome-container">
  <div class="welcome-header">
    <div class="neon-text">WELCOME TO THE<br><br>ELITES</div>
    <div class="cyber-line"></div>
  </div>
</div>

## Quick Access Portal

<div class="portal-grid">
  <div class="portal-card" data-portal="training">
    <div class="portal-icon">🎯</div>
    <div class="portal-content">
      <h3>Training Modules</h3>
      <ul>
        <li><a href="/bootcamp/overview">Elite Bootcamp</a></li>
        <li><a href="/bootcamp/tools">Tools Arsenal</a></li>
        <li><a href="/bootcamp/config">Configuration Lab</a></li>
      </ul>
      <div class="portal-status">
        <div class="status-dot"></div>
        <span>SYSTEM ACTIVE</span>
      </div>
    </div>
  </div>

  <div class="portal-card" data-portal="tools">
    <div class="portal-icon">⚡</div>
    <div class="portal-content">
      <h3>Essential Tools</h3>
      <ul>
        <li>OpenBullet Suite</li>
        <li>SilverBullet Platform</li>
        <li>Browser Automation Studio</li>
      </ul>
      <div class="portal-status">
        <div class="status-dot"></div>
        <span>TOOLS READY</span>
      </div>
    </div>
  </div>

  <div class="portal-card" data-portal="security">
    <div class="portal-icon">🔒</div>
    <div class="portal-content">
      <h3>Security Protocols</h3>
      <ul>
        <li>OPSEC Guidelines</li>
        <li>Proxy Management</li>
        <li>Anti-Detection Systems</li>
      </ul>
      <div class="portal-status">
        <div class="status-dot"></div>
        <span>SECURE MODE</span>
      </div>
    </div>
  </div>
</div>

## System Notices

<div class="notices-container">
  <div class="notice warning">
    <div class="notice-icon">⚠️</div>
    <div class="notice-content">
      <h4 class="glitch-text" data-text="Security Protocol Active">Security Protocol Active</h4>
      <p>Maintain OPSEC at all times. Follow security guidelines.</p>
    </div>
    <div class="notice-indicator"></div>
  </div>

  <div class="notice info">
    <div class="notice-icon">ℹ️</div>
    <div class="notice-content">
      <h4 class="glitch-text" data-text="System Status">System Status</h4>
      <p>All systems operational. Tools and resources ready.</p>
    </div>
    <div class="notice-indicator"></div>
  </div>
</div>

<style>
.welcome-container {
  background: linear-gradient(45deg, #000, #1a1a1a);
  padding: 4rem 2rem;
  margin: 2rem 0;
  border-radius: 1rem;
  position: relative;
  overflow: hidden;
}

.welcome-container::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: 
    repeating-linear-gradient(90deg, 
      transparent, 
      transparent 50px, 
      rgba(0, 255, 0, 0.1) 50px, 
      rgba(0, 255, 0, 0.1) 51px
    );
  animation: scanline 8s linear infinite;
}

@keyframes scanline {
  0% { transform: translateY(0); }
  100% { transform: translateY(100%); }
}

.welcome-header {
  position: relative;
  z-index: 1;
  text-align: center;
}

.neon-text {
  font-size: 3rem;
  font-weight: bold;
  color: #00ff00;
  text-shadow: 
    0 0 5px #00ff00,
    0 0 10px #00ff00,
    0 0 20px #00ff00;
  animation: neonPulse 2s infinite;
}

@keyframes neonPulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.8; }
}

.cyber-line {
  height: 2px;
  background: linear-gradient(90deg, transparent, #00ff00, transparent);
  margin: 2rem auto;
  width: 200px;
  position: relative;
}

.cyber-line::before {
  content: '';
  position: absolute;
  top: -2px;
  left: 50%;
  width: 20px;
  height: 6px;
  background: #00ff00;
  transform: translateX(-50%);
  animation: linePulse 2s infinite;
}

@keyframes linePulse {
  0%, 100% { transform: translateX(-50%) scaleX(1); }
  50% { transform: translateX(-50%) scaleX(1.5); }
}

.portal-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 3rem 0;
}

.portal-card {
  background: rgba(0, 0, 0, 0.7);
  border: 1px solid #00e5ff;
  border-radius: 1rem;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  transition: all 0.3s ease;
}

.portal-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: 
    linear-gradient(45deg, transparent 48%, rgba(0, 229, 255, 0.1) 49%, rgba(0, 229, 255, 0.1) 51%, transparent 52%);
  background-size: 4px 4px;
  opacity: 0.5;
  pointer-events: none;
}

.portal-card:hover {
  transform: translateY(-5px);
  border-color: #00ff00;
  box-shadow: 0 0 20px rgba(0, 255, 0, 0.2);
}

.portal-icon {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.portal-content h3 {
  color: #00e5ff;
  margin: 0 0 1rem 0;
}

.portal-content ul {
  list-style: none;
  padding: 0;
  margin: 0 0 1.5rem 0;
}

.portal-content li {
  color: #a8b2c3;
  padding: 0.5rem 0;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.portal-content li:last-child {
  border-bottom: none;
}

.portal-status {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  font-family: monospace;
  color: #00ff00;
}

.status-dot {
  width: 8px;
  height: 8px;
  background: #00ff00;
  border-radius: 50%;
  animation: statusBlink 1s infinite;
}

@keyframes statusBlink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}

.notices-container {
  display: grid;
  gap: 1rem;
  margin: 2rem 0;
}

.notice {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1.5rem;
  border-radius: 0.5rem;
  background: rgba(0, 0, 0, 0.7);
  border: 1px solid;
  position: relative;
  overflow: hidden;
}

.notice.warning {
  border-color: #ffd700;
}

.notice.info {
  border-color: #00e5ff;
}

.notice-icon {
  font-size: 1.5rem;
}

.notice-content h4 {
  margin: 0 0 0.5rem 0;
  color: #fff;
}

.notice-content p {
  margin: 0;
  color: #a8b2c3;
}

.notice-indicator {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: linear-gradient(90deg, transparent, currentColor, transparent);
  animation: indicatorSlide 2s infinite;
}

@keyframes glitch {
  0% {
    clip-path: polygon(0 2%, 100% 2%, 100% 5%, 0 5%);
    transform: translate(0);
  }
  20% {
    clip-path: polygon(0 15%, 100% 15%, 100% 15%, 0 15%);
    transform: translate(-5px);
  }
  30% {
    clip-path: polygon(0 10%, 100% 10%, 100% 20%, 0 20%);
    transform: translate(5px);
  }
  40% {
    clip-path: polygon(0 1%, 100% 1%, 100% 2%, 0 2%);
    transform: translate(-5px);
  }
  50% {
    clip-path: polygon(0 33%, 100% 33%, 100% 33%, 0 33%);
    transform: translate(0);
  }
  60% {
    clip-path: polygon(0 44%, 100% 44%, 100% 44%, 0 44%);
    transform: translate(5px);
  }
  70% {
    clip-path: polygon(0 50%, 100% 50%, 100% 20%, 0 20%);
    transform: translate(-5px);
  }
  80% {
    clip-path: polygon(0 70%, 100% 70%, 100% 70%, 0 70%);
    transform: translate(0);
  }
  100% {
    clip-path: polygon(0 70%, 100% 70%, 100% 70%, 0 70%);
    transform: translate(0);
  }
}

.glitch-text {
  position: relative;
  animation: glitch-skew 1s infinite linear alternate-reverse;
}

.glitch-text::before,
.glitch-text::after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.glitch-text::before {
  color: #ff0000;
  animation: glitch 2s infinite;
  clip-path: polygon(0 0, 100% 0, 100% 45%, 0 45%);
}

.glitch-text::after {
  color: #00ff00;
  animation: glitch 2s infinite reverse;
  clip-path: polygon(0 55%, 100% 55%, 100% 100%, 0 100%);
}

@keyframes glitch-skew {
  0% { transform: skew(0deg); }
  20% { transform: skew(-2deg); }
  40% { transform: skew(2deg); }
  60% { transform: skew(-1deg); }
  80% { transform: skew(3deg); }
  100% { transform: skew(0deg); }
}

@keyframes indicatorSlide {
  0% { transform: translateX(-100%); }
  100% { transform: translateX(100%); }
}

[data-portal="training"] { border-color: #ff0000; }
[data-portal="tools"] { border-color: #00ff00; }
[data-portal="security"] { border-color: #0000ff; }
</style>
