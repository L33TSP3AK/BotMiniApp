# Pricing Plans

<div class="hero-section">
  <div class="cyber-grid"></div>
  <h1 class="neon-text">Elite Access Plans</h1>
  <div class="cyber-line"></div>
</div>

## Available Plans

<div class="pricing-grid">
  <PriceCard
    tier="Basic"
    icon="🔵"
    :prices="{
      monthly: 29.99,
      quarterly: 80.97,
      biannual: 143.95
    }"
  />
  
  <PriceCard
    tier="Premium"
    icon="⭐"
    :prices="{
      monthly: 49.99,
      quarterly: 134.97,
      biannual: 239.95
    }"
  />
  
  <PriceCard
    tier="VIP"
    icon="👑"
    :prices="{
      monthly: 99.99,
      quarterly: 269.97,
      biannual: 479.95
    }"
  />

  <PriceCard
    tier="Diamond"
    icon="💎"
    :prices="{
      monthly: 199.99,
      quarterly: 539.97,
      biannual: 959.95
    }"
  />
</div>

## Payment Methods

<Card title="Secure Payments" icon="🔒">
  <div class="payment-methods">
    <span title="Bitcoin">₿</span>
    <span title="Litecoin">Ł</span>
    <span title="Ethereum">Ξ</span>
    <span title="Monero">ɱ</span>
  </div>
</Card>

## Billing FAQ

<div class="faq-section">
  <Card title="Common Questions" icon="❓">
    <details class="faq-item">
      <summary>How often am I billed?</summary>
      <p>Choose between monthly, quarterly, or biannual billing cycles. All plans are auto-renewed unless cancelled.</p>
    </details>
    
    <details class="faq-item">
      <summary>Can I upgrade my plan?</summary>
      <p>Yes, you can upgrade at any time. The price difference will be prorated based on your remaining subscription time.</p>
    </details>
    
    <details class="faq-item">
      <summary>What payment methods are accepted?</summary>
      <p>We accept various cryptocurrencies for maximum privacy and convenience. Contact support for specific payment arrangements.</p>
    </details>

    <details class="faq-item">
      <summary>Is there a refund policy?</summary>
      <p>Due to the nature of our services, all sales are final. No refunds will be processed once access is granted.</p>
    </details>
  </Card>
</div>

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

@keyframes gridScroll {
  0% { transform: translate(0, 0); }
  100% { transform: translate(20px, 20px); }
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

.pricing-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.payment-methods {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin: 1rem 0;
  font-size: 1.5rem;
}

.payment-methods span {
  color: var(--vp-c-brand);
  cursor: help;
}

.faq-section {
  margin: 2rem 0;
}

.faq-item {
  margin: 1rem 0;
  padding: 0.5rem 0;
  border-bottom: 1px solid var(--vp-c-border);
}

.faq-item:last-child {
  border-bottom: none;
}

.faq-item summary {
  cursor: pointer;
  color: var(--vp-c-brand);
  font-weight: 500;
}

.faq-item p {
  margin: 0.5rem 0;
  padding-left: 1rem;
  color: var(--vp-c-text-2);
}
</style>