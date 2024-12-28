# Configuration Laboratory

<div class="config-container">
  <div class="cyber-grid"></div>
  <div class="terminal-header">
    <div class="terminal-controls">
      <span class="control"></span>
      <span class="control"></span>
      <span class="control"></span>
    </div>
    <div class="terminal-title">DOOMSDAY_X_PRODUCTIONS v1.0</div>
  </div>
  
  <div class="terminal-window">
    <div class="line">Initializing configuration collection...</div>
    <div class="line">Found 312 Bullet Configs...</div>
    <div class="line">Found 267 BAS Configs...</div>
    <div class="line">Found 281 BL Tools Configs...</div>
    <div class="line success">System ready.</div>
  </div>
</div>

## Available Tools

<div class="tools-grid">
  <Feature
    icon="🎯"
    title="OpenBullet"
    details="Industry standard automation with LoliScript support"
  />
  <Feature
    icon="⚡"
    title="SilverBullet"
    details="Premium automation with enhanced features"
  />
  <Feature
    icon="🌐"
    title="BAS"
    details="Browser Automation Studio for advanced operations"
  />
  <Feature
    icon="🛠️"
    title="Custom Tools"
    details="Specialized tools for specific requirements"
  />
</div>

## Module Selection

<div class="module-grid">
  <div class="module" data-type="web">
    <div class="module-header">
      <div class="status-indicator"></div>
      <h3>Web Automation</h3>
    </div>
    <div class="code-preview">
      ```js
      async function webConfig() {
        await page.goto(target);
        await page.evaluate(() => {
          // Custom logic
        });
      }
      ```
    </div>
  </div>

  <div class="module" data-type="api">
    <div class="module-header">
      <div class="status-indicator"></div>
      <h3>API Integration</h3>
    </div>
    <div class="code-preview">
      ```js
      const apiConfig = {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json'
        },
        body: JSON.stringify(data)
      };
      ```
    </div>
  </div>

  <div class="module" data-type="data">
    <div class="module-header">
      <div class="status-indicator"></div>
      <h3>Data Processing</h3>
    </div>
    <div class="code-preview">
      ```js
      function processData(input) {
        return input
          .filter(valid)
          .map(transform)
          .reduce(aggregate);
      }
      ```
    </div>
  </div>
</div>

## Configuration Types

<div class="config-section">
  <Card title="Basic Configs" icon="⚙️">
    <Badge type="tip" text="Essential" />
    <ul>
      <li>Standard Operations</li>
      <li>Basic Automation</li>
      <li>Simple Validation</li>
      <li>Data Extraction</li>
    </ul>
  </Card>

  <Card title="Advanced Configs" icon="🚀">
    <Badge type="warning" text="Professional" />
    <ul>
      <li>Complex Operations</li>
      <li>Custom Protocols</li>
      <li>Advanced Parsing</li>
      <li>Pattern Matching</li>
    </ul>
  </Card>
</div>

## Security Guidelines

::: warning Operational Security
Always follow security best practices when developing configs
:::

::: danger Important Notice
Verify compliance with terms of service and local regulations
:::

<style>
.config-container {
  background: #0a0a0a;
  border-radius: 1rem;
  padding: 2rem;
  margin: 2rem 0;
  position: relative;
  overflow: hidden;
  border: 1px solid #00ff00;
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

@keyframes gridScroll {
  0% { transform: translate(0, 0); }
  100% { transform: translate(20px, 20px); }
}

.terminal-header {
  position: relative;
  z-index: 1;
  background: #1a1a1a;
  padding: 0.5rem 1rem;
  border-radius: 0.5rem 0.5rem 0 0;
  display: flex;
  align-items: center;
}

.terminal-controls {
  display: flex;
  gap: 0.5rem;
}

.control {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: #ff5f56;
}

.control:nth-child(2) { background: #ffbd2e; }
.control:nth-child(3) { background: #27c93f; }

.terminal-title {
  position: absolute;
  width: 100%;
  text-align: center;
  color: #666;
  font-family: monospace;
}

.terminal-window {
  position: relative;
  z-index: 1;
  background: rgba(0, 0, 0, 0.8);
  padding: 1rem;
  font-family: monospace;
  color: #00ff00;
}

.line {
  margin: 0.5rem 0;
  opacity: 0;
  animation: typeLine 0.5s ease forwards;
}

.line.success {
  color: #27c93f;
}

@keyframes typeLine {
  from { opacity: 0; transform: translateX(-10px); }
  to { opacity: 1; transform: translateX(0); }
}

.tools-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

.module-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.module {
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid;
  border-radius: 0.5rem;
  overflow: hidden;
  transition: all 0.3s ease;
}

.module[data-type="web"] { border-color: #ff5f56; }
.module[data-type="api"] { border-color: #ffbd2e; }
.module[data-type="data"] { border-color: #27c93f; }

.module:hover {
  transform: translateY(-5px);
  box-shadow: 0 0 20px rgba(0, 255, 0, 0.2);
}

.module-header {
  padding: 1rem;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  align-items: center;
  gap: 1rem;
}

.status-indicator {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: currentColor;
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0% { transform: scale(1); opacity: 1; }
  50% { transform: scale(1.2); opacity: 0.5; }
  100% { transform: scale(1); opacity: 1; }
}

.code-preview {
  padding: 1rem;
  background: #1a1a1a;
}

.code-preview pre {
  margin: 0;
  font-family: monospace;
}

.config-section {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

:deep(.feature-box) {
  background: var(--vp-c-bg-soft);
  border: 1px solid var(--vp-c-border);
  transition: all 0.3s ease;
}

:deep(.feature-box:hover) {
  transform: translateY(-4px);
  border-color: var(--vp-c-brand);
  box-shadow: 0 8px 16px rgba(0, 229, 255, 0.1);
}

:deep(.feature-title) {
  background: linear-gradient(120deg, var(--vp-c-brand), var(--vp-c-brand-dark));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>