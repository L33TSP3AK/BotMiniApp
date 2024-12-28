# ULP Data Analysis

<div class="cyber-container">
  <div class="matrix-bg"></div>
  <div class="cyber-header">
    <h1 class="neon-text">ULP Data Scanner</h1>
    <div class="status-line">
      <span class="label">STATUS</span>
      <span class="value">ACTIVE</span>
    </div>
  </div>

  <div class="data-grid">
    <div class="data-card">
      <div class="card-header">
        <div class="icon">🔐</div>
        <h3>Account Data</h3>
        <div class="status-indicator"></div>
      </div>
      <div class="data-preview">
        <div class="data-line">Email: <span class="highlight">***@***.**</span></div>
        <div class="data-line">Pass: <span class="highlight">********</span></div>
        <div class="data-line">Type: <span class="highlight">Premium</span></div>
      </div>
      <div class="scan-line"></div>
    </div>
    <div class="data-card">
      <div class="card-header">
        <div class="icon">🍪</div>
        <h3>Cookie Data</h3>
        <div class="status-indicator"></div>
      </div>
      <div class="data-preview">
        <div class="data-line">Session: <span class="highlight">Active</span></div>
        <div class="data-line">Valid: <span class="highlight">Yes</span></div>
        <div class="data-line">Type: <span class="highlight">Auth</span></div>
      </div>
      <div class="scan-line"></div>
    </div>
    <div class="data-card">
      <div class="card-header">
        <div class="icon">🔑</div>
        <h3>Token Data</h3>
        <div class="status-indicator"></div>
      </div>
      <div class="data-preview">
        <div class="data-line">Type: <span class="highlight">Bearer</span></div>
        <div class="data-line">Valid: <span class="highlight">Yes</span></div>
        <div class="data-line">Exp: <span class="highlight">24h</span></div>
      </div>
      <div class="scan-line"></div>
    </div>
  </div>
</div>

<style>
.cyber-container {
  background: #000;
  border-radius: 1rem;
  padding: 2rem;
  margin: 2rem 0;
  position: relative;
  overflow: hidden;
  border: 1px solid #00ff00;
}

.matrix-bg {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: 
    linear-gradient(90deg, rgba(0, 255, 0, 0.1) 1px, transparent 1px),
    linear-gradient(rgba(0, 255, 0, 0.1) 1px, transparent 1px);
  background-size: 20px 20px;
  animation: matrixScroll 20s linear infinite;
  pointer-events: none;
}

.cyber-header {
  position: relative;
  text-align: center;
  margin-bottom: 2rem;
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

.status-line {
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin-top: 1rem;
  font-family: monospace;
  color: #00ff00;
}

.data-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  position: relative;
  z-index: 1;
}

.data-card {
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid #00ff00;
  border-radius: 0.5rem;
  padding: 1.5rem;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  transition: all 0.3s ease;
}

.data-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 0 20px rgba(0, 255, 0, 0.3);
}

.card-header {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-bottom: 1rem;
}

.icon {
  font-size: 1.5rem;
}

.status-indicator {
  width: 8px;
  height: 8px;
  background: #00ff00;
  border-radius: 50%;
  margin-left: auto;
  animation: pulse 2s infinite;
}

.data-preview {
  font-family: monospace;
  color: #00ff00;
}

.data-line {
  padding: 0.5rem 0;
  border-bottom: 1px solid rgba(0, 255, 0, 0.2);
}

.highlight {
  color: #00e5ff;
}

.scan-line {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: #00ff00;
  animation: scan 2s linear infinite;
}

@keyframes matrixScroll {
  0% { transform: translate(0, 0); }
  100% { transform: translate(20px, 20px); }
}

@keyframes pulse {
  0% { opacity: 1; }
  50% { opacity: 0.3; }
  100% { opacity: 1; }
}

@keyframes scan {
  0% { transform: translateY(-100%); }
  100% { transform: translateY(300%); }
}
</style>