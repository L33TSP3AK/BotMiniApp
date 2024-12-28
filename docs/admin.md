# Admin Panel

<div class="admin-container">
  <div class="cyber-grid"></div>
  <div class="admin-header">
    <h1 class="neon-text">ADMIN CONTROL PANEL</h1>
    <div class="cyber-line"></div>
  </div>

  <div class="section-grid">
    <div class="section-card">
      <h2>📁 Callouts</h2>
      <div class="content-list">
        <a href="/callouts/alerts" class="content-item">
          <span class="item-icon">⚠️</span>
          <span class="item-text">Alerts</span>
        </a>
        <a href="/callouts/info-boxes" class="content-item">
          <span class="item-icon">ℹ️</span>
          <span class="item-text">Info Boxes</span>
        </a>
        <a href="/callouts/notifications" class="content-item">
          <span class="item-icon">🔔</span>
          <span class="item-text">Notifications</span>
        </a>
      </div>
    </div>
    <div class="section-card">
      <h2>🧩 Components</h2>
      <div class="content-list">
        <a href="/components/badges" class="content-item">
          <span class="item-icon">🏷️</span>
          <span class="item-text">Badges</span>
        </a>
        <a href="/components/cards" class="content-item">
          <span class="item-icon">📇</span>
          <span class="item-text">Cards</span>
        </a>
        <a href="/components/features" class="content-item">
          <span class="item-icon">✨</span>
          <span class="item-text">Features</span>
        </a>
      </div>
    </div>
    <div class="section-card">
      <h2>📝 Markdown</h2>
      <div class="content-list">
        <a href="/markdown/containers" class="content-item">
          <span class="item-icon">📦</span>
          <span class="item-text">Containers</span>
        </a>
        <a href="/markdown/extended" class="content-item">
          <span class="item-icon">🔧</span>
          <span class="item-text">Extended Syntax</span>
        </a>
        <a href="/markdown/vue" class="content-item">
          <span class="item-icon">⚡</span>
          <span class="item-text">Vue Integration</span>
        </a>
      </div>
    </div>
    <div class="section-card">
      <h2>📐 Layouts</h2>
      <div class="content-list">
        <a href="/layouts/grid" class="content-item">
          <span class="item-icon">🔲</span>
          <span class="item-text">Grid System</span>
        </a>
        <a href="/layouts/responsive" class="content-item">
          <span class="item-icon">📱</span>
          <span class="item-text">Responsive Design</span>
        </a>
      </div>
    </div>
    <div class="section-card">
      <h2>🎮 Interactive</h2>
      <div class="content-list">
        <a href="/interactive/toasts" class="content-item">
          <span class="item-icon">🔔</span>
          <span class="item-text">Toasts</span>
        </a>
        <a href="/interactive/url-anatomy" class="content-item">
          <span class="item-icon">🔗</span>
          <span class="item-text">URL Anatomy</span>
        </a>
        <a href="/interactive/ulp-data" class="content-item">
          <span class="item-icon">📊</span>
          <span class="item-text">ULP Data</span>
        </a>
        <a href="/interactive/accordions" class="content-item">
          <span class="item-icon">📂</span>
          <span class="item-text">Accordions</span>
        </a>
      </div>
    </div>
    <div class="section-card">
      <h2>⚡ Performance</h2>
      <div class="content-list">
        <a href="/performance/assets" class="content-item">
          <span class="item-icon">🖼️</span>
          <span class="item-text">Asset Loading</span>
        </a>
        <a href="/performance/best-practices" class="content-item">
          <span class="item-icon">📊</span>
          <span class="item-text">Best Practices</span>
        </a>
        <a href="/performance/images" class="content-item">
          <span class="item-icon">🎨</span>
          <span class="item-text">Image Optimization</span>
        </a>
      </div>
    </div>
  </div>
</div>

<style>
.admin-container {
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

.admin-header {
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

.section-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  position: relative;
  z-index: 1;
}

.section-card {
  background: rgba(0, 0, 0, 0.8);
  border: 1px solid #00ff00;
  border-radius: 1rem;
  padding: 1.5rem;
}

.section-card h2 {
  color: #00ff00;
  margin: 0 0 1.5rem 0;
  font-size: 1.5rem;
}

.content-list {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.content-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 0.75rem;
  background: rgba(0, 255, 0, 0.1);
  border: 1px solid rgba(0, 255, 0, 0.2);
  border-radius: 0.5rem;
  color: #00ff00;
  text-decoration: none;
  transition: all 0.3s ease;
}

.content-item:hover {
  background: rgba(0, 255, 0, 0.2);
  transform: translateX(0.5rem);
}

.item-icon {
  font-size: 1.25rem;
}

@keyframes gridScroll {
  0% { transform: translate(0, 0); }
  100% { transform: translate(20px, 20px); }
}
</style>