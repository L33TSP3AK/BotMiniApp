# Advanced Tools Arsenal

<div class="tools-container">
  <div class="matrix-bg"></div>
  <div class="tools-header">
    <div class="scanner-line"></div>
    <h1 class="cyber-title">TOOLS ARSENAL</h1>
    <div class="header-decor"></div>
  </div>
</div>

## Essential Tools

<div class="tools-grid">
  <div class="tool-card" @mousemove="handleMouseMove" @mouseleave="handleMouseLeave" style="transform-style: preserve-3d">
    <div class="tool-hologram"></div>
    <div class="tool-content">
      <div class="tool-icon">🔧</div>
      <h3>OpenBullet</h3>
      <div class="tool-stats">
        <div class="stat">
          <span class="label">Power</span>
          <div class="stat-bar">
            <div class="fill" style="width: 85%"></div>
          </div>
        </div>
        <div class="stat">
          <span class="label">Complexity</span>
          <div class="stat-bar">
            <div class="fill" style="width: 65%"></div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="tool-card" @mousemove="handleMouseMove" @mouseleave="handleMouseLeave" style="transform-style: preserve-3d">
    <div class="tool-hologram"></div>
    <div class="tool-content">
      <div class="tool-icon">⚡</div>
      <h3>SilverBullet</h3>
      <div class="tool-stats">
        <div class="stat">
          <span class="label">Power</span>
          <div class="stat-bar">
            <div class="fill" style="width: 95%"></div>
          </div>
        </div>
        <div class="stat">
          <span class="label">Complexity</span>
          <div class="stat-bar">
            <div class="fill" style="width: 75%"></div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="tool-card" @mousemove="handleMouseMove" @mouseleave="handleMouseLeave" style="transform-style: preserve-3d">
    <div class="tool-hologram"></div>
    <div class="tool-content">
      <div class="tool-icon">🌐</div>
      <h3>BAS</h3>
      <div class="tool-stats">
        <div class="stat">
          <span class="label">Power</span>
          <div class="stat-bar">
            <div class="fill" style="width: 90%"></div>
          </div>
        </div>
        <div class="stat">
          <span class="label">Complexity</span>
          <div class="stat-bar">
            <div class="fill" style="width: 85%"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

## Advanced Arsenal

<div class="total-configs">
  <div class="total-header">Total Configs Available</div>
  <div class="total-count">730</div>
  <div class="total-breakdown">
    <div class="breakdown-item">
      <span class="item-label">Openbullet:</span>
      <span class="item-value">25</span>
    </div>
    <div class="breakdown-item">
      <span class="item-label">Openbullet 2:</span>
      <span class="item-value">271</span>
    </div>
    <div class="breakdown-item">
      <span class="item-label">Silverbullet:</span>
      <span class="item-value">28</span>
    </div>
    <div class="breakdown-item">
      <span class="item-label">Cookiebullet:</span>
      <span class="item-value">47</span>
    </div>
    <div class="breakdown-item">
      <span class="item-label">BAS:</span>
      <span class="item-value">213</span>
    </div>
    <div class="breakdown-item">
      <span class="item-label">BL Tool Projects:</span>
      <span class="item-value">146</span>
    </div>
  </div>
</div>

<div class="arsenal-grid">
  <div class="arsenal-item" v-for="(count, tool) in {
    'Openbullet': 25,
    'Openbullet 2': 271,
    'Silverbullet': 28,
    'Cookiebullet': 47,
    'BAS': 213,
    'BL Tool Projects': 146
  }">
    <div class="item-header">
      <div class="status-light"></div>
      <span class="item-id">{{ tool }}</span>
      <span class="count">{{ count }}</span>
    </div>
    <div class="item-body">
      <div class="loading-bar">
        <div class="loading-progress" :style="{ width: Math.round(count / 271 * 100) + '%' }"></div>
      </div>
    </div>
  </div>
</div>

## Recommended Tools

<div class="tools-section">
  <AccordionItem type="cyber" title="Essential Tools" icon="🛠️" status="FREE">
    <div class="tool-content">
      <div class="tools-list">
        <div class="tools-row">
          <a href="https://www.voidtools.com/Everything-1.4.1.1026.x86-Setup.exe" class="tool-item" target="_blank">
            <span class="tool-icon">🔍</span>
            <div class="tool-info">
              <h4>Everything Search</h4>
              <p>Ultra-fast file search utility</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://notepad-plus-plus.org/" class="tool-item" target="_blank">
            <span class="tool-icon">📝</span>
            <div class="tool-info">
              <h4>Notepad++</h4>
              <p>Advanced text editor with syntax highlighting</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://www.python.org/" class="tool-item" target="_blank">
            <span class="tool-icon">🐍</span>
            <div class="tool-info">
              <h4>Python</h4>
              <p>Popular programming language for automation</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://www.win-rar.com/" class="tool-item" target="_blank">
            <span class="tool-icon">📦</span>
            <div class="tool-info">
              <h4>WinRAR</h4>
              <p>File compression and archive manager</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://obsidian.md/" class="tool-item" target="_blank">
            <span class="tool-icon">📓</span>
            <div class="tool-info">
              <h4>Obsidian</h4>
              <p>Knowledge base and note-taking app</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://www.mythicsoft.com/filelocatorpro/" class="tool-item" target="_blank">
            <span class="tool-icon">🗂️</span>
            <div class="tool-info">
              <h4>FileLocator Pro</h4>
              <p>Advanced file search and content analysis</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://www.comfortsoftware.com/clipboard-manager/" class="tool-item" target="_blank">
            <span class="tool-icon">📋</span>
            <div class="tool-info">
              <h4>Clipboard Manager</h4>
              <p>Enhanced clipboard with history</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://bablosoft.com/" class="tool-item" target="_blank">
            <span class="tool-icon">🤖</span>
            <div class="tool-info">
              <h4>Bablosoft</h4>
              <p>Browser automation tools</p>
            </div>
          </a>
        </div>
      </div>
    </div>
  </AccordionItem>

  <AccordionItem type="hologram" title="Coding Resources" icon="💻" status="FREE">
    <div class="tool-content">
      <div class="tools-list">
        <div class="tools-row">
          <a href="https://github.com" class="tool-item" target="_blank">
            <span class="tool-icon">🐙</span>
            <div class="tool-info">
              <h4>GitHub</h4>
              <p>Code hosting and version control</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://gitbook.io" class="tool-item" target="_blank">
            <span class="tool-icon">📚</span>
            <div class="tool-info">
              <h4>GitBook</h4>
              <p>Documentation and knowledge base platform</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://codepen.io" class="tool-item" target="_blank">
            <span class="tool-icon">✏️</span>
            <div class="tool-info">
              <h4>CodePen</h4>
              <p>Online code editor and playground</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://codesandbox.io" class="tool-item" target="_blank">
            <span class="tool-icon">📦</span>
            <div class="tool-info">
              <h4>CodeSandbox</h4>
              <p>Online IDE for web development</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://codehs.com" class="tool-item" target="_blank">
            <span class="tool-icon">🎓</span>
            <div class="tool-info">
              <h4>CodeHS</h4>
              <p>Learn to code with interactive tutorials</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://netlify.com/" class="tool-item" target="_blank">
            <span class="tool-icon">🌐</span>
            <div class="tool-info">
              <h4>Netlify</h4>
              <p>Web hosting and deployment platform</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://playcode.io/" class="tool-item" target="_blank">
            <span class="tool-icon">🎮</span>
            <div class="tool-info">
              <h4>PlayCode</h4>
              <p>JavaScript playground and editor</p>
            </div>
          </a>
        </div>
      </div>
    </div>
  </AccordionItem>
</div>

<style>
.tools-section {
  display: grid;
  gap: 2rem;
  margin: 2rem 0;
}

.tools-list {
  display: grid;
  gap: 1rem;
}

.tools-row {
  width: 100%;
}

.tool-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  border: 1px solid rgba(0, 255, 0, 0.2);
  border-radius: 0.5rem;
  text-decoration: none;
  transition: all 0.3s ease;
  width: 100%;
}

.tool-item:hover {
  transform: translateX(10px);
  border-color: var(--vp-c-brand);
  background: rgba(0, 0, 0, 0.4);
}

.tool-icon {
  font-size: 1.5rem;
}

.tool-info h4 {
  margin: 0 0 0.25rem 0;
  color: var(--vp-c-brand);
}

.tool-info p {
  margin: 0;
  color: var(--vp-c-text-2);
  font-size: 0.9rem;
}
          </div>
        </a>
        <a href="https://notepad-plus-plus.org/" class="tool-item" target="_blank">
          <span class="tool-icon">📝</span>
          <div class="tool-info">
            <h4>Notepad++</h4>
            <p>Advanced text editor with syntax highlighting</p>
          </div>
        </a>
        <a href="https://www.python.org/" class="tool-item" target="_blank">
          <span class="tool-icon">🐍</span>
          <div class="tool-info">
            <h4>Python</h4>
            <p>Popular programming language for automation</p>
          </div>
        </a>
        <a href="https://www.win-rar.com/" class="tool-item" target="_blank">
          <span class="tool-icon">📦</span>
          <div class="tool-info">
            <h4>WinRAR</h4>
            <p>File compression and archive manager</p>
          </div>
        </a>
        <a href="https://obsidian.md/" class="tool-item" target="_blank">
          <span class="tool-icon">📓</span>
          <div class="tool-info">
            <h4>Obsidian</h4>
            <p>Knowledge base and note-taking app</p>
          </div>
        </a>
        <a href="https://www.mythicsoft.com/filelocatorpro/" class="tool-item" target="_blank">
          <span class="tool-icon">🗂️</span>
          <div class="tool-info">
            <h4>FileLocator Pro</h4>
            <p>Advanced file search and content analysis</p>
          </div>
        </a>
        <a href="https://www.comfortsoftware.com/clipboard-manager/" class="tool-item" target="_blank">
          <span class="tool-icon">📋</span>
          <div class="tool-info">
            <h4>Clipboard Manager</h4>
            <p>Enhanced clipboard with history</p>
          </div>
        </a>
        <a href="https://bablosoft.com/" class="tool-item" target="_blank">
          <span class="tool-icon">🤖</span>
          <div class="tool-info">
            <h4>Bablosoft</h4>
            <p>Browser automation tools</p>
          </div>
        </a>
      </div>
    </div>
  </AccordionItem>

  <AccordionItem type="hologram" title="Coding Resources" icon="💻" status="FREE">
    <div class="tool-content">
      <div class="tools-list">
        <a href="https://github.com" class="tool-item" target="_blank">
          <span class="tool-icon">🐙</span>
          <div class="tool-info">
            <h4>GitHub</h4>
            <p>Code hosting and version control</p>
          </div>
        </a>
        <a href="https://gitbook.io" class="tool-item" target="_blank">
          <span class="tool-icon">📚</span>
          <div class="tool-info">
            <h4>GitBook</h4>
            <p>Documentation and knowledge base platform</p>
          </div>
        </a>
        <a href="https://codepen.io" class="tool-item" target="_blank">
          <span class="tool-icon">✏️</span>
          <div class="tool-info">
            <h4>CodePen</h4>
            <p>Online code editor and playground</p>
          </div>
        </a>
        <a href="https://codesandbox.io" class="tool-item" target="_blank">
          <span class="tool-icon">📦</span>
          <div class="tool-info">
            <h4>CodeSandbox</h4>
            <p>Online IDE for web development</p>
          </div>
        </a>
        <a href="https://codehs.com" class="tool-item" target="_blank">
          <span class="tool-icon">🎓</span>
          <div class="tool-info">
            <h4>CodeHS</h4>
            <p>Learn to code with interactive tutorials</p>
          </div>
        </a>
        <a href="https://netlify.com/" class="tool-item" target="_blank">
          <span class="tool-icon">🌐</span>
          <div class="tool-info">
            <h4>Netlify</h4>
            <p>Web hosting and deployment platform</p>
          </div>
        </a>
        <a href="https://playcode.io/" class="tool-item" target="_blank">
          <span class="tool-icon">🎮</span>
          <div class="tool-info">
            <h4>PlayCode</h4>
            <p>JavaScript playground and editor</p>
          </div>
        </a>
      </div>
    </div>
  </AccordionItem>
</div>



  <AccordionItem type="cyber" title="Team Projects" icon="👥" status="ACTIVE">
    <div class="tool-content">
      <div class="tools-list">
        <div class="tools-row">
          <a href="https://dly.to/GF5kqX5Wa1N" class="tool-item" target="_blank">
            <span class="tool-icon">🔗</span>
            <div class="tool-info">
              <h4>Daily.dev</h4>
              <p>Developer news and collaboration platform</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://codesandbox.io/invite/mn499kgf2xhldtxw" class="tool-item" target="_blank">
            <span class="tool-icon">📦</span>
            <div class="tool-info">
              <h4>CodeSandbox Team</h4>
              <p>Collaborative development environment</p>
            </div>
          </a>
        </div>
        <div class="tools-row">
          <a href="https://github.com/organizations/Plug-Outlet" class="tool-item" target="_blank">
            <span class="tool-icon">🐙</span>
            <div class="tool-info">
              <h4>GitHub Organization</h4>
              <p>Team code repository and project management</p>
            </div>
          </a>
        </div>
      </div>
    </div>
  </AccordionItem>


<style>
.tools-section {
  display: grid;
  gap: 2rem;
  margin: 2rem 0;
}

.tools-list {
  display: grid;
  gap: 1rem;
}

.tool-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  border: 1px solid rgba(0, 255, 0, 0.2);
  border-radius: 0.5rem;
  text-decoration: none;
  transition: all 0.3s ease;
}

.tool-item:hover {
  transform: translateX(10px);
  border-color: var(--vp-c-brand);
  background: rgba(0, 0, 0, 0.4);
}

.tool-icon {
  font-size: 1.5rem;
}

.tool-info h4 {
  margin: 0 0 0.25rem 0;
  color: var(--vp-c-brand);
}

.tool-info p {
  margin: 0;
  color: var(--vp-c-text-2);
  font-size: 0.9rem;
}

.tools-container {
  position: relative;
  padding: 4rem 2rem;
  margin: 2rem 0;
  background: #000;
  border-radius: 1rem;
  overflow: hidden;
}

.matrix-bg {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(45deg, 
    rgba(0, 255, 0, 0.1) 25%, 
    transparent 25%, 
    transparent 75%, 
    rgba(0, 255, 0, 0.1) 75%
  );
  background-size: 10px 10px;
  animation: matrixMove 20s linear infinite;
}

@keyframes matrixMove {
  0% { background-position: 0 0; }
  100% { background-position: 50px 50px; }
}

.tools-header {
  position: relative;
  text-align: center;
  z-index: 1;
}

.scanner-line {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: #00ff00;
  animation: scan 2s linear infinite;
}

@keyframes scan {
  0% { transform: translateY(0); }
  100% { transform: translateY(100px); }
}

.cyber-title {
  font-size: 3rem;
  color: #00ff00;
  text-shadow: 0 0 10px #00ff00;
  margin: 0;
  letter-spacing: 4px;
}

.header-decor {
  height: 4px;
  background: linear-gradient(90deg, transparent, #00ff00, transparent);
  margin: 1rem auto;
  width: 200px;
}

.tools-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 3rem 0;
}

.tool-card {
  position: relative;
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid #00e5ff;
  border-radius: 1rem;
  padding: 2rem;
  overflow: hidden;
  perspective: 1000px;
  transition: transform 0.1s ease;
  transform: perspective(1000px) rotateX(0) rotateY(0) scale3d(1, 1, 1);
}

.tool-card:hover {
  transform: perspective(1000px) rotateX(0) rotateY(0) scale3d(1.05, 1.05, 1.05);
}

.tool-card:hover .tool-hologram {
  box-shadow: 
    -5px 5px 20px rgba(0, 255, 0, 0.2),
    5px -5px 20px rgba(0, 229, 255, 0.2);
}

.tool-hologram {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: 
    linear-gradient(45deg, transparent 48%, rgba(0, 229, 255, 0.1) 49%, rgba(0, 229, 255, 0.1) 51%, transparent 52%),
    linear-gradient(-45deg, transparent 48%, rgba(0, 229, 255, 0.1) 49%, rgba(0, 229, 255, 0.1) 51%, transparent 52%);
  background-size: 4px 4px;
  pointer-events: none;
  transform: translateZ(10px);
}

.tool-content {
  position: relative;
  z-index: 1;
  transform: translateZ(30px);
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  border-radius: 0.5rem;
  overflow: hidden;
}

.tool-content::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: 
    linear-gradient(45deg, transparent 45%, rgba(0, 229, 255, 0.1) 50%, transparent 55%),
    linear-gradient(-45deg, transparent 45%, rgba(0, 229, 255, 0.1) 50%, transparent 55%);
  background-size: 20px 20px;
  animation: hologramScan 10s linear infinite;
  pointer-events: none;
}

@keyframes hologramScan {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}

.tools-list {
  display: grid;
  gap: 1rem;
}

.tool-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  border: 1px solid rgba(0, 255, 0, 0.2);
  border-radius: 0.5rem;
  text-decoration: none;
  transition: all 0.3s ease;
}

.tool-item:hover {
  transform: translateX(10px);
  border-color: var(--vp-c-brand);
  background: rgba(0, 0, 0, 0.4);
}

.tool-icon {
  font-size: 1.5rem;
}

.tool-info h4 {
  margin: 0 0 0.25rem 0;
  color: var(--vp-c-brand);
}

.tool-info p {
  margin: 0;
  color: var(--vp-c-text-2);
  font-size: 0.9rem;
}

.tools-container {
  position: relative;
  padding: 4rem 2rem;
  margin: 2rem 0;
  background: #000;
  border-radius: 1rem;
  overflow: hidden;
}

.matrix-bg {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(45deg, 
    rgba(0, 255, 0, 0.1) 25%, 
    transparent 25%, 
    transparent 75%, 
    rgba(0, 255, 0, 0.1) 75%
  );
  background-size: 10px 10px;
  animation: matrixMove 20s linear infinite;
}

@keyframes matrixMove {
  0% { background-position: 0 0; }
  100% { background-position: 50px 50px; }
}

.tools-header {
  position: relative;
  text-align: center;
  z-index: 1;
}

.scanner-line {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: #00ff00;
  animation: scan 2s linear infinite;
}

@keyframes scan {
  0% { transform: translateY(0); }
  100% { transform: translateY(100px); }
}

.cyber-title {
  font-size: 3rem;
  color: #00ff00;
  text-shadow: 0 0 10px #00ff00;
  margin: 0;
  letter-spacing: 4px;
}

.header-decor {
  height: 4px;
  background: linear-gradient(90deg, transparent, #00ff00, transparent);
  margin: 1rem auto;
  width: 200px;
}

.tools-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 3rem 0;
}

.tool-card {
  position: relative;
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid #00e5ff;
  border-radius: 1rem;
  padding: 2rem;
  overflow: hidden;
  perspective: 1000px;
  transition: transform 0.1s ease;
  transform: perspective(1000px) rotateX(0) rotateY(0) scale3d(1, 1, 1);
}

.tool-card:hover {
  transform: perspective(1000px) rotateX(0) rotateY(0) scale3d(1.05, 1.05, 1.05);
}

.tool-card:hover .tool-hologram {
  box-shadow: 
    -5px 5px 20px rgba(0, 255, 0, 0.2),
    5px -5px 20px rgba(0, 229, 255, 0.2);
}

.tool-hologram {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: 
    linear-gradient(45deg, transparent 48%, rgba(0, 229, 255, 0.1) 49%, rgba(0, 229, 255, 0.1) 51%, transparent 52%),
    linear-gradient(-45deg, transparent 48%, rgba(0, 229, 255, 0.1) 49%, rgba(0, 229, 255, 0.1) 51%, transparent 52%);
  background-size: 4px 4px;
  pointer-events: none;
  transform: translateZ(10px);
}

.tool-content {
  position: relative;
  z-index: 1;
  transform: translateZ(30px);
}

.tool-icon {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.tool-stats {
  margin-top: 1.5rem;
}

.stat {
  margin-bottom: 1rem;
}

.label {
  display: block;
  color: #00e5ff;
  margin-bottom: 0.5rem;
  font-size: 0.9rem;
}

.stat-bar {
  height: 4px;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 2px;
  overflow: hidden;
}

.fill {
  height: 100%;
  background: linear-gradient(90deg, #00ff00, #00e5ff);
  animation: fillPulse 2s infinite;
}

@keyframes fillPulse {
  0% { opacity: 1; }
  50% { opacity: 0.5; }
  100% { opacity: 1; }
}

.total-configs {
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid #00ff00;
  border-radius: 0.5rem;
  padding: 1.5rem;
  margin-bottom: 2rem;
  text-align: center;
}

.total-header {
  color: #00ff00;
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
}

.total-count {
  font-size: 3rem;
  font-weight: bold;
  color: #00ff00;
  text-shadow: 0 0 10px #00ff00;
  margin: 1rem 0;
}

.total-breakdown {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 0.5rem;
  text-align: left;
}

.breakdown-item {
  display: flex;
  justify-content: space-between;
  padding: 0.5rem;
  border-bottom: 1px solid rgba(0, 255, 0, 0.2);
}

.breakdown-item:last-child {
  border-bottom: none;
}

.item-label {
  color: #00e5ff;
  font-family: monospace;
}

.item-value {
  color: #00ff00;
  font-weight: bold;
  font-family: monospace;
}

.arsenal-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
  margin: 2rem 0;
}

.arsenal-item {
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid rgba(0, 229, 255, 0.3);
  border-radius: 0.5rem;
  padding: 1rem;
}

.item-header {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  margin-bottom: 1rem;
  justify-content: space-between;
}

.status-light {
  width: 8px;
  height: 8px;
  background: #00ff00;
  border-radius: 50%;
  animation: blink 1s infinite;
}

.item-id {
  color: #00e5ff;
  font-family: monospace;
  flex: 1;
}

.count {
  color: #00ff00;
  font-family: monospace;
  font-weight: bold;
  margin-left: auto;
}

.loading-bar {
  height: 2px;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 1px;
  overflow: hidden;
}

.loading-progress {
  height: 100%;
  background: #00ff00;
  position: relative;
  animation: pulse 2s infinite;
}

.loading-progress::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.8), transparent);
  transform: translateX(-100%);
  animation: shimmer 2s infinite;
}

@keyframes pulse {
  0% { opacity: 1; }
  50% { opacity: 0.3; }
  100% { opacity: 1; }
}

@keyframes shimmer {
  0% { transform: translateX(-100%); opacity: 0.8; }
  50% { opacity: 0.2; }
  100% { transform: translateX(100%); }
}

@keyframes blink {
  0% { opacity: 1; }
  50% { opacity: 0.3; }
  100% { opacity: 1; }
}
</style>

<script setup>
function handleMouseMove(e) {
  const card = e.currentTarget;
  const rect = card.getBoundingClientRect();
  
  const centerX = rect.width / 2;
  const centerY = rect.height / 2;
  const mouseX = e.clientX - rect.left;
  const mouseY = e.clientY - rect.top;
  
  // Calculate rotation based on distance from center
  const rotateY = ((mouseX - centerX) / centerX) * 20;
  const rotateX = -((mouseY - centerY) / centerY) * 20;
  
  // Apply smooth transition
  card.style.transform = `
    perspective(1000px)
    rotateX(${rotateX}deg)
    rotateY(${rotateY}deg)
    scale3d(1.05, 1.05, 1.05)
  `;
}

function handleMouseLeave(e) {
  e.currentTarget.style.transform = 'perspective(1000px) rotateX(0) rotateY(0) scale3d(1, 1, 1)';
}
</script>