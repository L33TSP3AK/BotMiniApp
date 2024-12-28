# Pricing Plans

Explore our flexible pricing options designed to meet your needs.

## Plan Options

<div class="pricing-grid">
  <Card title="Basic" icon="🔵">
    <Badge type="info" text="Starter" />
    <div class="price">$29.99<span>/month</span></div>
    <ul class="features">
      <li>✅ Basic Features</li>
      <li>✅ Community Support</li>
      <li>❌ Advanced Tools</li>
      <li>❌ Priority Support</li>
    </ul>
  </Card>

  <Card title="Premium" icon="⭐">
    <Badge type="tip" text="Popular" />
    <div class="price">$49.99<span>/month</span></div>
    <ul class="features">
      <li>✅ All Basic Features</li>
      <li>✅ Advanced Tools</li>
      <li>✅ Priority Support</li>
      <li>❌ Custom Solutions</li>
    </ul>
  </Card>

  <Card title="Enterprise" icon="👑">
    <Badge type="warning" text="Full Access" />
    <div class="price">$99.99<span>/month</span></div>
    <ul class="features">
      <li>✅ All Premium Features</li>
      <li>✅ Custom Solutions</li>
      <li>✅ 24/7 Support</li>
      <li>✅ Dedicated Manager</li>
    </ul>
  </Card>
</div>

## Payment Methods

<div class="payment-methods">
  <Card title="Accepted Payments" icon="💳">
    <div class="crypto-grid">
      <span title="Bitcoin">₿</span>
      <span title="Ethereum">Ξ</span>
      <span title="Litecoin">Ł</span>
      <span title="Monero">ɱ</span>
    </div>
  </Card>
</div>

<style>
.pricing-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

.price {
  font-size: 2rem;
  font-weight: bold;
  color: var(--vp-c-brand);
  margin: 1rem 0;
}

.price span {
  font-size: 1rem;
  color: var(--vp-c-text-2);
}

.features {
  list-style: none;
  padding: 0;
  margin: 1rem 0;
}

.features li {
  padding: 0.5rem 0;
  border-bottom: 1px solid var(--vp-c-border);
}

.features li:last-child {
  border-bottom: none;
}

.payment-methods {
  margin: 2rem 0;
}

.crypto-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(60px, 1fr));
  gap: 1rem;
  text-align: center;
  font-size: 1.5rem;
}

.crypto-grid span {
  color: var(--vp-c-brand);
  cursor: help;
}
</style>