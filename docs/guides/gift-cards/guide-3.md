<div class="guide-container">
  <div class="cyber-grid"></div>
  <div class="guide-header">
    <div class="neon-text" data-text="MegaBonanza">MegaBonanza</div>
    <div class="cyber-line"></div>
  </div>

  <div class="guide-info">
    <AccordionItem type="cyber" title="Target Information" icon="🎯" status="ACTIVE">
      <div class="info-grid">
        <div class="info-item">
          <span class="label">Website</span>
          <a href="https://www.megabonanza.com" class="value website-link" target="_blank" rel="noopener noreferrer">
            megabonanza.com
            <div class="website-meta">
              <a href="https://web-check.xyz/check/https%3A%2F%2Fmegabonanza.com" class="meta-item" target="_blank" rel="noopener noreferrer">
                <span class="meta-icon">🔒</span>
                <span class="meta-text">SSL:</span>
                <span class="meta-value">Valid</span>
              </a>
              <a href="https://web-check.xyz/check/https%3A%2F%2Fmegabonanza.com" class="meta-item" target="_blank" rel="noopener noreferrer">
                <span class="meta-icon">🌍</span>
                <span class="meta-text">Location:</span>
                <span class="meta-value">US</span>
              </a>
              <a href="https://web-check.xyz/check/https%3A%2F%2Fmegabonanza.com" class="meta-item" target="_blank" rel="noopener noreferrer">
                <span class="meta-icon">⚡</span>
                <span class="meta-text">Response:</span>
                <span class="meta-value">150ms</span>
              </a>
            </div>
          </a>
        </div>
        <div class="info-item">
          <span class="label">Tags</span>
          <div class="tags">
            <span class="tag">Sports Apparel</span>
            <span class="tag">Merchandise</span>
            <span class="tag">Fan Gear</span>
          </div>
        </div>
        <div class="info-item">
          <span class="label">Payment Methods</span>
          <div class="payment-methods">
            <span class="payment-chip" title="Credit Card">
              <span class="chip-icon">💳</span>
              <span class="chip-text">CC</span>
            </span>
            <span class="payment-chip" title="PayPal">
              <span class="chip-icon">💰</span>
              <span class="chip-text">PP</span>
            </span>
            <span class="payment-chip" title="Bank Transfer">
              <span class="chip-icon">🏦</span>
              <span class="chip-text">ACH</span>
            </span>
          </div>
        </div>
        <div class="info-item">
          <span class="label">AVS Enforced</span>
          <span class="value yes">Yes</span>
        </div>
        <div class="info-item">
          <span class="label">Hackable</span>
          <div class="hackable-options">
            <span class="option unavailable" title="Email Access">📧 ❌</span>
            <span class="option" title="Direct Access">🔑 ✓</span>
            <span class="option" title="Cookie Access">🍪 ✓</span>
          </div>
        </div>
      </div>
    </AccordionItem>
  </div>

  <div class="guide-content">
    <AccordionItem type="neon" title="Requirements" icon="📋" status="INFO">
      <ul class="requirements-list">
        <li>Valid payment method</li>
        <li>US residential proxy</li>
        <li>Walmart+ account</li>
        <li>SMS verification</li>
      </ul>
    </AccordionItem>
    <AccordionItem type="hologram" title="Step-by-Step Guide" icon="📝" status="GUIDE">
      <div class="steps">
        <div class="step">
          <div class="step-number">01</div>
          <div class="step-content">
            <h3>Account Creation</h3>
            <p>Set up new Walmart account with clean profile.</p>
            <div class="step-notes">
              <span class="note">Verify phone</span>
              <span class="note">Add Walmart+</span>
            </div>
          </div>
        </div>
        <div class="step">
          <div class="step-number">02</div>
          <div class="step-content">
            <h3>Location Setup</h3>
            <p>Configure delivery and pickup locations.</p>
            <div class="step-notes">
              <span class="note">Local store</span>
              <span class="note">Valid address</span>
            </div>
          </div>
        </div>
        <div class="step">
          <div class="step-number">03</div>
          <div class="step-content">
            <h3>Payment Method</h3>
            <p>Add and verify payment information.</p>
            <div class="step-notes">
              <span class="note">Verify card</span>
              <span class="note">Check limits</span>
            </div>
          </div>
        </div>
      </div>
    </AccordionItem>
  </div>

  <div class="guide-warnings">
    <div class="warning-card">
      <div class="warning-icon">
        <div class="warning-circle">
          <span class="warning-symbol">⚠️</span>
        </div>
      </div>
      <div class="warning-content">
        <h4 class="glitch-text" data-text="SECURITY NOTICE">SECURITY NOTICE</h4>
        <p>Maintain strict OPSEC and secure all gift card codes immediately.</p>
      </div>
      <div class="warning-scanner"></div>
    </div>
  </div>
</div>

<style>
/* Same styles as previous guides */
.guide-container {
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

.guide-header {
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
  position: relative;
}

.neon-text::before,
.neon-text::after {
  content: attr(data-text);
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  opacity: 0.5;
  animation: glitch 0.3s infinite alternate-reverse;
}

.neon-text::before {
  color: #ff0000;
  clip-path: polygon(0 0, 100% 0, 100% 45%, 0 45%);
  transform: translateX(-2px);
}

.neon-text::after {
  color: #0000ff;
  clip-path: polygon(0 55%, 100% 55%, 100% 100%, 0 100%);
  transform: translateX(2px);
}

.cyber-line {
  height: 2px;
  background: linear-gradient(90deg, transparent, #00ff00, transparent);
  margin: 2rem auto;
  width: 200px;
}

.info-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  border-radius: 0.5rem;
}

.info-item {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.label {
  color: var(--vp-c-text-2);
  font-size: 0.9rem;
}

.value {
  font-family: monospace;
  color: var(--vp-c-brand);
}

.value.yes {
  color: #00ff00;
}

.value.no {
  color: #ff0000;
}

.value.check {
  color: #00ff00;
  font-size: 1.2rem;
}

.tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.tag {
  padding: 0.25rem 0.75rem;
  background: rgba(0, 255, 0, 0.1);
  border: 1px solid #00ff00;
  border-radius: 1rem;
  font-size: 0.8rem;
  color: #00ff00;
}

.payment-methods {
  display: flex;
  gap: 0.5rem;
}

.method {
  font-size: 1.2rem;
  cursor: help;
}

.requirements-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.requirements-list li {
  padding: 0.5rem 0;
  border-bottom: 1px solid rgba(0, 255, 0, 0.2);
  color: var(--vp-c-text-2);
}

.requirements-list li:last-child {
  border-bottom: none;
}

.steps {
  display: grid;
  gap: 1.5rem;
}

.step {
  display: flex;
  gap: 1rem;
  padding: 1rem;
  background: rgba(0, 0, 0, 0.3);
  border-radius: 0.5rem;
  border: 1px solid rgba(0, 255, 0, 0.2);
}

.step-number {
  font-size: 1.5rem;
  font-weight: bold;
  color: #00ff00;
  font-family: monospace;
}

.step-content h3 {
  margin: 0 0 0.5rem 0;
  color: var(--vp-c-brand);
}

.step-content p {
  margin: 0 0 0.5rem 0;
  color: var(--vp-c-text-2);
}

.step-notes {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}

.note {
  padding: 0.25rem 0.75rem;
  background: rgba(0, 255, 0, 0.1);
  border-radius: 1rem;
  font-size: 0.8rem;
  color: #00ff00;
}

.warning-card {
  display: flex;
  gap: 1rem;
  padding: 1rem;
  background: linear-gradient(45deg, rgba(255, 0, 0, 0.1), rgba(255, 0, 0, 0.2));
  border: 1px solid #ff0000;
  border-radius: 0.5rem;
  margin-top: 2rem;
  position: relative;
  overflow: hidden;
}

.warning-icon {
  display: flex;
  align-items: center;
  justify-content: center; 
}

.warning-circle {
  width: 2.5rem;
  height: 2.5rem;
  border: 2px solid #ff0000;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  animation: pulseWarning 2s infinite;
  position: relative;
  overflow: hidden;
}

.warning-circle::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: linear-gradient(
    45deg,
    transparent,
    rgba(255, 0, 0, 0.2),
    transparent
  );
  transform: rotate(45deg);
  animation: warningGlow 2s linear infinite;
}

.warning-symbol {
  font-size: 1.5rem;
  position: relative;
  z-index: 1;
}

.warning-scanner {
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 2px;
  background: linear-gradient(90deg, transparent, #ff0000, transparent);
  animation: scanWarning 2s linear infinite;
}

.warning-content h4 {
  margin: 0 0 0.5rem 0;
  color: #ff0000;
}

.warning-content p {
  margin: 0;
  color: var(--vp-c-text-2);
}

.glitch-text {
  position: relative;
  color: #ff0000;
  text-shadow: 0 0 5px #ff0000;
  animation: glitchText 3s infinite linear alternate-reverse;
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
  color: #ff3300;
  animation: glitchText 2s infinite;
  clip-path: polygon(0 0, 100% 0, 100% 45%, 0 45%);
  transform: translate(-2px);
  opacity: 0.7;
}

.glitch-text::after {
  color: #ff0066;
  animation: glitchText 2.5s infinite;
  clip-path: polygon(0 55%, 100% 55%, 100% 100%, 0 100%);
  transform: translate(2px);
  opacity: 0.7;
}

@keyframes gridScroll {
  0% { transform: translate(0, 0); }
  100% { transform: translate(20px, 20px); }
}

@keyframes glitch {
  0% { transform: translateX(-2px); }
  100% { transform: translateX(2px); }
}

@keyframes pulseWarning {
  0% { transform: scale(1); opacity: 1; }
  50% { transform: scale(1.1); opacity: 0.7; }
  100% { transform: scale(1); opacity: 1; }
}

@keyframes scanWarning {
  0% { left: -100%; }
  100% { left: 100%; }
}

@keyframes warningGlow {
  0% { transform: translateX(-100%) rotate(45deg); }
  100% { transform: translateX(100%) rotate(45deg); }
}

@keyframes glitchText {
  0% { transform: translate(0); }
  20% { transform: translate(-2px, 2px); }
  40% { transform: translate(-2px, -2px); }
  60% { transform: translate(2px, 2px); }
  80% { transform: translate(2px, -2px); }
  100% { transform: translate(0); }
}
</style>