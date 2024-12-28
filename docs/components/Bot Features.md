# Bot Features

<div class="hero-section">
  <h1>The #1 Must Have Service for Maximizing Your Profits!</h1>
</div>

## Service Categories

<div class="service-grid">
  <div class="service-category">
    <h2>💳 Financial Services</h2>
    <div class="service-list">
      <Feature
        icon="💳"
        title="Card Check"
        details="Advanced card validation and verification services"
      />
      <Feature
        icon="🏦"
        title="Bank Check"
        details="Comprehensive bank account verification"
      />
      <Feature
        icon="🔢"
        title="BIN Checking"
        details="Bank identification number validation and lookup"
      />
      <Feature
        icon="💰"
        title="IVR Balance Checker"
        details="Automated balance verification system"
      />
    </div>
  </div>

  <div class="service-category">
    <h2>⚙️ Configuration Tools</h2>
    <div class="service-list">
      <Feature
        icon="⚙️"
        title="Bullet Configs"
        details="Streamlined configuration management"
      />
      <Feature
        icon="🛠️"
        title="Available Configs"
        details="Browse and manage system configurations"
      />
      <Feature
        icon="🔧"
        title="BAS Configs"
        details="Advanced BAS configuration tools"
      />
      <Feature
        icon="🍪"
        title="Cookie Configs"
        details="Cookie management and configuration"
      />
    </div>
  </div>

  <div class="service-category">
    <h2>🔍 Search Tools</h2>
    <div class="service-list">
      <Feature
        icon="🔍"
        title="Request ULP"
        details="Universal log processing and search"
      />
      <Feature
        icon="📬"
        title="Search Inbox"
        details="Advanced inbox search capabilities"
      />
      <Feature
        icon="🔎"
        title="Search By Request"
        details="Request-based search functionality"
      />
      <Feature
        icon="🌐"
        title="Search By Country"
        details="Geographic search filtering"
      />
    </div>
  </div>

  <div class="service-category">
    <h2>📧 Request Services</h2>
    <div class="service-list">
      <Feature
        icon="💭"
        title="Suggest Requests"
        details="Intelligent request suggestions"
      />
      <Feature
        icon="📧"
        title="Email Targets"
        details="Email targeting system"
      />
      <Feature
        icon="🍪"
        title="Cookie Targets"
        details="Cookie-based targeting tools"
      />
      <Feature
        icon="📝"
        title="Request Config"
        details="Configuration request system"
      />
    </div>
  </div>
</div>

## Membership Levels

<div class="membership-grid">
  <Card title="Basic" icon="🔵">
    <Badge type="info" text="Basic Access" />
    <ul class="feature-list">
      <li>✅ Basic Guides</li>
      <li>⚠️ Limited Card Check</li>
      <li>⚠️ Limited Bank Check</li>
      <li>❌ IVR Check</li>
      <li>⚠️ Limited Cookies</li>
    </ul>
  </Card>

  <Card title="Premium" icon="🔰">
    <Badge type="tip" text="Enhanced Access" />
    <ul class="feature-list">
      <li>✅ Full Guide Access</li>
      <li>⚠️ Enhanced Card Check</li>
      <li>✅ Full Bank Check</li>
      <li>❌ IVR Check</li>
      <li>✅ Full Cookie Access</li>
    </ul>
  </Card>

  <Card title="VIP" icon="👑">
    <Badge type="warning" text="VIP Access" />
    <ul class="feature-list">
      <li>✅ Premium Guides</li>
      <li>✅ Full Card Check</li>
      <li>✅ Advanced Bank Check</li>
      <li>⚠️ Limited IVR</li>
      <li>✅ Advanced Cookies</li>
    </ul>
  </Card>

  <Card title="Diamond" icon="💎">
    <Badge type="info" text="Ultimate Access" />
    <ul class="feature-list">
      <li>🌟 Elite Guides</li>
      <li>✅ Ultimate Card Check</li>
      <li>✅ Premium Bank Check</li>
      <li>✅ Full IVR Access</li>
      <li>✅ Elite Cookie System</li>
    </ul>
  </Card>
</div>

<style>
.hero-section {
  text-align: center;
  padding: 2rem 0;
  margin-bottom: 3rem;
  background: linear-gradient(45deg, var(--vp-c-bg-soft), var(--vp-c-bg-alt));
  border-radius: 1rem;
  border: 1px solid var(--vp-c-brand);
}

.hero-section h1 {
  background: linear-gradient(120deg, var(--vp-c-brand), var(--vp-c-brand-light));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 2.5rem;
  margin: 0;
  padding: 0 1rem;
}

.service-grid {
  display: grid;
  gap: 2rem;
  margin: 2rem 0;
}

.service-category h2 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  padding: 0.5rem 1rem;
  background: var(--vp-c-bg-soft);
  border-radius: 0.5rem;
  color: var(--vp-c-brand);
  border-left: 4px solid var(--vp-c-brand);
}

.service-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
}

.membership-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

.feature-list {
  list-style: none;
  padding: 0;
  margin: 1rem 0 0 0;
}

.feature-list li {
  padding: 0.5rem 0;
  border-bottom: 1px solid var(--vp-c-border);
}

.feature-list li:last-child {
  border-bottom: none;
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

:deep(.feature-details) {
  color: var(--vp-c-text-2);
}

@media (max-width: 768px) {
  .service-list {
    grid-template-columns: 1fr;
  }
  
  .membership-grid {
    grid-template-columns: 1fr;
  }
  
  .hero-section h1 {
    font-size: 2rem;
  }
}
</style>