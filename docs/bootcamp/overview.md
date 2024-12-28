# Elite Training Program

<div class="hero-container">
  <div class="matrix-bg"></div>
  <div class="hero-content">
    <div class="glitch-text" data-text="ELITE TRAINING">ELITE TRAINING</div>
    <div class="cyber-subtitle">Advanced Black Hat Operations</div>
    <div class="pulse-line"></div>
  </div>
</div>

## Training Modules

<div class="module-grid">
  <div class="module-card" data-category="stealer">
    <div class="card-glow"></div>
    <div class="module-icon">🎭</div>
    <h3>Stealer Operations</h3>
    <ul>
      <li>Log Analysis</li>
      <li>Data Extraction</li>
      <li>Cookie Management</li>
    </ul>
    <div class="progress-bar">
      <div class="progress" style="width: 75%"></div>
    </div>
  </div>

  <div class="module-card" data-category="carding">
    <div class="card-glow"></div>
    <div class="module-icon">💳</div>
    <h3>Carding Techniques</h3>
    <ul>
      <li>Card Validation</li>
      <li>Bank Verification</li>
      <li>Balance Checking</li>
    </ul>
    <div class="progress-bar">
      <div class="progress" style="width: 60%"></div>
    </div>
  </div>

  <div class="module-card" data-category="config">
    <div class="card-glow"></div>
    <div class="module-icon">⚙️</div>
    <h3>Config Development</h3>
    <ul>
      <li>Pattern Creation</li>
      <li>Script Writing</li>
      <li>Error Handling</li>
    </ul>
    <div class="progress-bar">
      <div class="progress" style="width: 45%"></div>
    </div>
  </div>

  <div class="module-card" data-category="security">
    <div class="card-glow"></div>
    <div class="module-icon">🔒</div>
    <h3>Security Protocols</h3>
    <ul>
      <li>OPSEC Basics</li>
      <li>Proxy Management</li>
      <li>Anti-Detection</li>
    </ul>
    <div class="progress-bar">
      <div class="progress" style="width: 90%"></div>
    </div>
  </div>
</div>

<style>
.hero-container {
  background: linear-gradient(45deg, #000, #1a1a1a);
  padding: 4rem 2rem;
  margin: 2rem 0;
  border-radius: 1rem;
  position: relative;
  overflow: hidden;
}

.matrix-bg {
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

.hero-content {
  position: relative;
  z-index: 1;
  text-align: center;
}

.glitch-text {
  font-size: 3rem;
  font-weight: bold;
  color: #00ff00;
  text-shadow: 
    0 0 5px #00ff00,
    0 0 10px #00ff00,
    0 0 20px #00ff00;
  animation: glitch 1s infinite;
}

@keyframes glitch {
  0% { transform: translate(0); }
  20% { transform: translate(-2px, 2px); }
  40% { transform: translate(-2px, -2px); }
  60% { transform: translate(2px, 2px); }
  80% { transform: translate(2px, -2px); }
  100% { transform: translate(0); }
}

.cyber-subtitle {
  font-size: 1.5rem;
  color: #00e5ff;
  margin-top: 1rem;
  text-transform: uppercase;
  letter-spacing: 4px;
}

.pulse-line {
  height: 2px;
  background: #00ff00;
  margin: 2rem auto;
  width: 200px;
  position: relative;
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0% { transform: scaleX(1); opacity: 1; }
  50% { transform: scaleX(1.5); opacity: 0.5; }
  100% { transform: scaleX(1); opacity: 1; }
}

.module-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
  margin: 3rem 0;
}

.module-card {
  background: rgba(0, 0, 0, 0.7);
  border-radius: 1rem;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  border: 1px solid rgba(0, 229, 255, 0.2);
  transition: all 0.3s ease;
}

.module-card:hover {
  transform: translateY(-5px);
  border-color: #00ff00;
  box-shadow: 0 0 20px rgba(0, 255, 0, 0.2);
}

.card-glow {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: radial-gradient(circle at 50% 50%, rgba(0, 255, 0, 0.1), transparent);
  opacity: 0;
  transition: opacity 0.3s ease;
}

.module-card:hover .card-glow {
  opacity: 1;
}

.module-icon {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.module-card h3 {
  color: #00e5ff;
  margin: 0 0 1rem 0;
}

.module-card ul {
  list-style: none;
  padding: 0;
  margin: 0 0 1.5rem 0;
}

.module-card li {
  color: #a8b2c3;
  padding: 0.5rem 0;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.module-card li:last-child {
  border-bottom: none;
}

.progress-bar {
  height: 4px;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 2px;
  overflow: hidden;
}

.progress {
  height: 100%;
  background: linear-gradient(90deg, #00ff00, #00e5ff);
  animation: progressPulse 2s infinite;
}

@keyframes progressPulse {
  0% { opacity: 1; }
  50% { opacity: 0.5; }
  100% { opacity: 1; }
}

[data-category="stealer"] { border-color: #ff0000; }
[data-category="carding"] { border-color: #00ff00; }
[data-category="config"] { border-color: #0000ff; }
[data-category="security"] { border-color: #ffff00; }
</style>