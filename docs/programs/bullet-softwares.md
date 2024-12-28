# Bullet Software Suite

<div class="hero-section">
  <div class="cyber-grid"></div>
  <h1 class="neon-text">BULLET ARSENAL</h1>
  <div class="cyber-line"></div>
</div>

## Available Tools

<div class="tools-grid">
  <AccordionItem type="cyber" title="OpenBullet" icon="🎯" status="STABLE">
    <div class="tool-content">
      <p>Advanced web automation and testing suite with LoliScript support.</p>
      <div class="features-list">
        <div class="feature">✓ Multi-threaded operations</div>
        <div class="feature">✓ Custom LoliScript language</div>
        <div class="feature">✓ Advanced proxy support</div>
        <div class="feature">✓ Built-in debugger</div>
      </div>
      <div class="download-section">
        <a href="https://github.com/openbullet/openbullet/releases" class="download-button" target="_blank">
          <span class="icon">⬇️</span>
          Download Latest
        </a>
        <span class="version">v2.1.0</span>
      </div>
    </div>
  </AccordionItem>

  <AccordionItem type="neon" title="SilverBullet" icon="⚡" status="PREMIUM">
    <div class="tool-content">
      <p>Premium automation tool with enhanced features and performance.</p>
      <div class="features-list">
        <div class="feature">✓ High-performance engine</div>
        <div class="feature">✓ Advanced scripting</div>
        <div class="feature">✓ Real-time statistics</div>
        <div class="feature">✓ Custom plugins</div>
      </div>
      <div class="download-section">
        <a href="https://silverbullet.com/download" class="download-button" target="_blank">
          <span class="icon">⬇️</span>
          Download Premium
        </a>
        <span class="version">v3.0.5</span>
      </div>
    </div>
  </AccordionItem>

  <AccordionItem type="hologram" title="OpenBullet 2" icon="🚀" status="LATEST">
    <div class="tool-content">
      <p>Next generation of OpenBullet with modern architecture.</p>
      <div class="features-list">
        <div class="feature">✓ Cross-platform support</div>
        <div class="feature">✓ Modern C# implementation</div>
        <div class="feature">✓ Enhanced security</div>
        <div class="feature">✓ Improved UI/UX</div>
      </div>
      <div class="download-section">
        <a href="https://github.com/openbullet/openbullet2/releases" class="download-button" target="_blank">
          <span class="icon">⬇️</span>
          Download Latest
        </a>
        <span class="version">v0.2.3</span>
      </div>
    </div>
  </AccordionItem>
</div>

## Security Notice

::: warning OPSEC
Always maintain proper operational security when using these tools.
:::

<style>
.hero-section {
  text-align: center;
  padding: 4rem 2rem;
  margin: 2rem 0;
  background: linear-gradient(45deg, #000, #1a1a1a);
  border-radius: 1rem;
  position: relative;
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
}

.neon-text {
  font-size: 3rem;
  color: #00ff00;
  text-shadow: 
    0 0 5px #00ff00,
    0 0 10px #00ff00,
    0 0 20px #00ff00;
  margin: 0;
  position: relative;
  z-index: 1;
}

.cyber-line {
  height: 2px;
  background: linear-gradient(90deg, transparent, #00ff00, transparent);
  margin: 2rem auto;
  width: 200px;
  position: relative;
  z-index: 1;
}

.tools-grid {
  display: grid;
  gap: 2rem;
  margin: 2rem 0;
}

.tool-content {
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  border-radius: 0.5rem;
}

.features-list {
  margin: 1rem 0;
  display: grid;
  gap: 0.5rem;
}

.feature {
  padding: 0.5rem;
  background: rgba(0, 255, 0, 0.1);
  border-radius: 0.25rem;
  font-family: monospace;
}

.download-section {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-top: 1.5rem;
}

.download-button {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.75rem 1.5rem;
  background: var(--vp-c-brand);
  color: var(--vp-c-bg);
  border-radius: 0.5rem;
  text-decoration: none;
  font-weight: bold;
  transition: all 0.3s ease;
}

.download-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 0 20px rgba(0, 255, 0, 0.3);
}

.version {
  font-family: monospace;
  color: var(--vp-c-text-2);
}

@keyframes gridScroll {
  0% { transform: translate(0, 0); }
  100% { transform: translate(20px, 20px); }
}
</style>