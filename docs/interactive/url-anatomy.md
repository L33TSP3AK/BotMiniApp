# URL Components Guide

<div class="url-container">
  <div class="cyber-grid"></div>
  
  <div class="url-header">
    <h1 class="neon-text">URL ANATOMY</h1>
    <div class="cyber-line"></div>
  </div>

  <div class="url-diagram">
    <div class="diagram-container">
      <svg viewBox="0 0 800 200" class="url-svg">
        <!-- Protocol -->
        <g class="protocol-group">
          <path d="M10,100 L150,100" class="connector"/>
          <text x="80" y="80" class="label">Protocol</text>
          <text x="80" y="140" class="value">https://</text>
        </g>
        <!-- Domain -->
        <g class="domain-group">
          <path d="M150,100 L350,100" class="connector"/>
          <text x="250" y="80" class="label">Domain</text>
          <text x="250" y="140" class="value">www.example.com</text>
        </g>
        <!-- Port -->
        <g class="port-group">
          <path d="M350,100 L450,100" class="connector"/>
          <text x="400" y="80" class="label">Port</text>
          <text x="400" y="140" class="value">:443</text>
        </g>
        <!-- Path -->
        <g class="path-group">
          <path d="M450,100 L550,100" class="connector"/>
          <text x="500" y="80" class="label">Path</text>
          <text x="500" y="140" class="value">/path</text>
        </g>
        <!-- Query -->
        <g class="query-group">
          <path d="M550,100 L650,100" class="connector"/>
          <text x="600" y="80" class="label">Query</text>
          <text x="600" y="140" class="value">?param=value</text>
        </g>
        <!-- Fragment -->
        <g class="fragment-group">
          <path d="M650,100 L790,100" class="connector"/>
          <text x="720" y="80" class="label">Fragment</text>
          <text x="720" y="140" class="value">#section</text>
        </g>
      </svg>
    </div>
  </div>
  <div class="url-components">
    <div class="url-display">
      <code>https://www.example.com:443/path/page?name=value#section</code>
    </div>
    <div class="components-grid">
      <div class="component-card">
        <div class="component-header">
          <span class="component-icon">🔒</span>
          <h3>Protocol</h3>
        </div>
        <div class="component-content">
          <code>https://</code>
          <p>Defines how data is transmitted (HTTP, HTTPS, FTP, etc)</p>
        </div>
      </div>
      <div class="component-card">
        <div class="component-header">
          <span class="component-icon">🌐</span>
          <h3>Domain</h3>
        </div>
        <div class="component-content">
          <code>www.example.com</code>
          <p>The website's address on the internet</p>
        </div>
      </div>
      <div class="component-card">
        <div class="component-header">
          <span class="component-icon">🔌</span>
          <h3>Port</h3>
        </div>
        <div class="component-content">
          <code>:443</code>
          <p>Connection point (443 for HTTPS, 80 for HTTP)</p>
          <details class="ports-callout">
            <summary>
              <h4>Common Ports <span class="expand-icon">▼</span></h4>
            </summary>
            <div class="ports-grid">
              <div class="port-item">
                <span class="port">21</span>
                <span class="service">FTP</span>
              </div>
              <div class="port-item">
                <span class="port">22</span>
                <span class="service">SSH</span>
              </div>
              <div class="port-item">
                <span class="port">25</span>
                <span class="service">SMTP</span>
              </div>
              <div class="port-item">
                <span class="port">53</span>
                <span class="service">DNS</span>
              </div>
              <div class="port-item">
                <span class="port">80</span>
                <span class="service">HTTP</span>
              </div>
              <div class="port-item">
                <span class="port">110</span>
                <span class="service">POP3</span>
              </div>
              <div class="port-item">
                <span class="port">143</span>
                <span class="service">IMAP</span>
              </div>
              <div class="port-item">
                <span class="port">443</span>
                <span class="service">HTTPS</span>
              </div>
              <div class="port-item">
                <span class="port">3306</span>
                <span class="service">MySQL</span>
              </div>
              <div class="port-item">
                <span class="port">5432</span>
                <span class="service">PostgreSQL</span>
              </div>
            </div>
          </details>
        </div>
      </div>
      <div class="component-card">
        <div class="component-header">
          <span class="component-icon">📁</span>
          <h3>Path</h3>
        </div>
        <div class="component-content">
          <code>/path/page</code>
          <p>Location of the resource on the server</p>
          <details class="paths-callout">
            <summary>
              <h4>⚠ Exploitable Leads</h4>
            </summary>
            <div class="paths-grid">
              <div class="path-item">
                <span class="path">/admin</span>
                <span class="risk">Admin Panels</span>
              </div>
              <div class="path-item">
                <span class="path">/backup</span>
                <span class="risk">Backup Files</span>
              </div>
              <div class="path-item">
                <span class="path">/config</span>
                <span class="risk">Configuration Files</span>
              </div>
              <div class="path-item">
                <span class="path">/install</span>
                <span class="risk">Installation Scripts</span>
              </div>
              <div class="path-item">
                <span class="path">/phpmyadmin</span>
                <span class="risk">Database Admin</span>
              </div>
              <div class="path-item">
                <span class="path">/wp-admin</span>
                <span class="risk">WordPress Admin</span>
              </div>
              <div class="path-item">
                <span class="path">/api</span>
                <span class="risk">API Endpoints</span>
              </div>
              <div class="path-item">
                <span class="path">/debug</span>
                <span class="risk">Debug Information</span>
              </div>
            </div>
          </details>
        </div>
      </div>
      <div class="component-card">
        <div class="component-header">
          <span class="component-icon">❓</span>
          <h3>Query Parameters</h3>
        </div>
        <div class="component-content">
          <code>?name=value</code>
          <p>Additional data passed to the server</p>
        </div>
      </div>
      <div class="component-card">
        <div class="component-header">
          <span class="component-icon">🔖</span>
          <h3>Fragment</h3>
        </div>
        <div class="component-content">
          <code>#section</code>
          <p>Specific section within the page</p>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
.url-container {
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

.url-header {
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
  margin: 2rem auto;
  width: 200px;
}

.url-display {
  background: rgba(0, 0, 0, 0.8);
  padding: 1rem;
  border-radius: 0.5rem;
  border: 1px solid #00ff00;
  margin-bottom: 2rem;
  overflow-x: auto;
  white-space: nowrap;
}

.url-display code {
  color: #00ff00;
  font-family: monospace;
  font-size: 1.2rem;
}

.components-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
}

.component-card {
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid #00ff00;
  border-radius: 0.5rem;
  padding: 1.5rem;
  transition: all 0.3s ease;
}

.component-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 0 20px rgba(0, 255, 0, 0.2);
}

.component-header {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-bottom: 1rem;
}

.component-icon {
  font-size: 1.5rem;
}

.component-header h3 {
  margin: 0;
  color: #00ff00;
}

.component-content code {
  display: block;
  background: rgba(0, 255, 0, 0.1);
  padding: 0.5rem;
  border-radius: 0.25rem;
  margin-bottom: 0.5rem;
  color: #00ff00;
  font-family: monospace;
}

.component-content p {
  margin: 0;
  color: #a8b2c3;
  font-size: 0.9rem;
}

.ports-callout {
  margin-top: 1rem;
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  border-radius: 0.5rem;
  border: 1px solid rgba(0, 255, 0, 0.2);
  cursor: pointer;
  transition: all 0.3s ease;
}

.ports-callout:hover {
  border-color: rgba(0, 255, 0, 0.4);
  background: rgba(0, 0, 0, 0.4);
}

.ports-callout summary {
  list-style: none;
}

.ports-callout summary::-webkit-details-marker {
  display: none;
}

.ports-callout summary h4 {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 0;
}

.expand-icon {
  font-size: 0.8rem;
  transition: transform 0.3s ease;
}

.ports-callout[open] .expand-icon {
  transform: rotate(180deg);
}

.ports-grid {
  margin-top: 1rem;
}

.ports-callout h4 {
  margin: 0 0 1rem 0;
  color: #00ff00;
  font-size: 0.9rem;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.ports-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
  gap: 0.5rem;
}

.port-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0.5rem;
  background: rgba(0, 0, 0, 0.3);
  border-radius: 0.25rem;
  border: 1px solid rgba(0, 255, 0, 0.1);
}

.port-item .port {
  color: #00ff00;
  font-family: monospace;
  font-weight: bold;
}

.port-item .service {
  color: #a8b2c3;
  font-size: 0.8rem;
  margin-top: 0.25rem;
}

.paths-callout {
  margin-top: 1rem;
  padding: 1rem;
  background: rgba(255, 0, 0, 0.1);
  border-radius: 0.5rem;
  border: 1px solid rgba(255, 0, 0, 0.2);
  cursor: pointer;
  transition: all 0.3s ease;
}

.paths-callout:hover {
  border-color: rgba(255, 0, 0, 0.4);
  background: rgba(255, 0, 0, 0.15);
}

.paths-callout summary {
  list-style: none;
}

.paths-callout summary::-webkit-details-marker {
  display: none;
}

.paths-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 0.5rem;
  margin-top: 1rem;
}

.path-item {
  display: flex;
  flex-direction: column;
  padding: 0.5rem;
  background: rgba(0, 0, 0, 0.3);
  border-radius: 0.25rem;
  border: 1px solid rgba(255, 0, 0, 0.1);
}

.path-item .path {
  color: #ff0000;
  font-family: monospace;
  font-weight: bold;
}

.path-item .risk {
  color: #ff9999;
  font-size: 0.8rem;
  margin-top: 0.25rem;
}

/* URL Diagram Styles */
.url-diagram {
  margin: 2rem 0;
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  border-radius: 0.5rem;
  border: 1px solid #00ff00;
}

.diagram-container {
  width: 100%;
  overflow-x: auto;
}

.url-svg {
  width: 100%;
  height: auto;
  min-height: 200px;
}

.connector {
  stroke: #00ff00;
  stroke-width: 2;
  stroke-dasharray: 5,5;
}

.label {
  fill: #00ff00;
  font-size: 14px;
  text-anchor: middle;
  font-family: monospace;
}

.value {
  fill: #a8b2c3;
  font-size: 12px;
  text-anchor: middle;
  font-family: monospace;
}

/* Hover effects for diagram groups */
.protocol-group:hover,
.domain-group:hover,
.port-group:hover,
.path-group:hover,
.query-group:hover,
.fragment-group:hover {
  .connector { stroke: #00e5ff; }
  .label { fill: #00e5ff; }
  .value { fill: #ffffff; }
}

@keyframes gridScroll {
  0% { transform: translate(0, 0); }
  100% { transform: translate(20px, 20px); }
}
</style>