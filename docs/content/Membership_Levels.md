# Membership Levels

<div class="hero-container">
  <div class="matrix-bg"></div>
  <div class="hero-content">
    <div class="glitch-text" data-text="ACCESS TIERS">ACCESS TIERS</div>
    <div class="cyber-subtitle">Choose Your Power Level</div>
    <div class="pulse-line"></div>
  </div>
</div>

## Available Tiers

<div class="tiers-grid">
  <Card title="Basic Access" icon="🔵">
    <Badge type="info" text="Entry Level" />
    <div class="tier-features">
      <div class="feature">
        <div class="feature-item">
          <span class="icon">✅</span>
          <span>Basic tool access</span>
        </div>
      </div>
      <div class="feature">
        <div class="feature-item">
          <span class="icon">✅</span>
          <span>Community support</span>
        </div>
      </div>
      <div class="feature">
        <div class="feature-item">
          <span class="icon">✅</span>
          <span>Standard configs</span>
        </div>
      </div>
      <div class="feature">
        <div class="feature-item">
          <span class="icon">❌</span>
          <span>Advanced features</span>
        </div>
      </div>
      <div class="feature">
        <div class="feature-item">
          <span class="icon">❌</span>
          <span>Priority support</span>
        </div>
      </div>
    </div>
    <PricingButton tier="Basic" icon="🔵" />
  </Card>

  <Card title="Premium Access" icon="⭐">
    <Badge type="tip" text="Most Popular" />
    <div class="tier-features">
      <div class="feature">
        <span class="icon">✅</span>
        <span>All basic features</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Advanced tools</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Priority support</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Premium configs</span>
      </div>
      <div class="feature">
        <span class="icon">❌</span>
        <span>Custom solutions</span>
      </div>
    </div>
    <PricingButton tier="Premium" icon="⭐" />
  </Card>

  <Card title="VIP Access" icon="👑">
    <Badge type="warning" text="Elite" />
    <div class="tier-features">
      <div class="feature">
        <span class="icon">✅</span>
        <span>All premium features</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Custom solutions</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>24/7 support</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Private training</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Exclusive tools</span>
      </div>
    </div>
    <PricingButton tier="VIP" icon="👑" />
  </Card>

  <Card title="Diamond Access" icon="💎">
    <Badge type="danger" text="Ultimate" />
    <div class="tier-features">
      <div class="feature">
        <span class="icon">✅</span>
        <span>All VIP features</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Priority development</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Direct developer access</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Custom tool development</span>
      </div>
      <div class="feature">
        <span class="icon">✅</span>
        <span>Unlimited everything</span>
      </div>
    </div>
    <PricingButton tier="Diamond" icon="💎" />
  </Card>
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

.tiers-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.tier-features {
  margin: 1rem 0;
}

.feature {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 0;
  border-bottom: 1px solid var(--vp-c-border);
}

.feature:last-child {
  border-bottom: none;
}

.feature .icon {
  font-size: 1.2rem;
}

.feature-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem;
  border-radius: 0.25rem;
  cursor: pointer;
  transition: all 0.2s ease;
}

.feature-item:hover {
  background: var(--vp-c-bg-alt);
}
</style>