# Service Limitations

<div class="hero-section">
  <div class="cyber-grid"></div>
  <h1 class="neon-text">System Constraints</h1>
  <div class="cyber-line"></div>
</div>

<script setup>
import { ref } from 'vue'

const activeAccordion = ref('')

function toggleAccordion(id) {
  activeAccordion.value = activeAccordion.value === id ? '' : id
}
</script>

## Usage Limits

<div class="limits-grid">
  <AccordionItem 
    type="cyber" 
    title="Basic Tier" 
    icon="🔵" 
    status="ACTIVE"
    :isOpen="activeAccordion === 'basic'"
    @click="toggleAccordion('basic')"
  >
    <div class="limits-list">
      <div class="limit-item">
        <span class="limit-label">Guides:</span>
        <span class="limit-value">✅ All Guides</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Card Check:</span>
        <span class="limit-value">15 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Bank Check:</span>
        <span class="limit-value">15 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">IVR Check:</span>
        <span class="limit-value">❌ No Access</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Cookies:</span>
        <span class="limit-value">10 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">ULP:</span>
        <span class="limit-value">500 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Inboxes:</span>
        <span class="limit-value">100 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Request Logs:</span>
        <span class="limit-value">15 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Configs:</span>
        <span class="limit-value">OB/SB</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Cards:</span>
        <span class="limit-value">❌ No Access</span>
      </div>
    </div>
  </AccordionItem>

  <AccordionItem 
    type="neon" 
    title="Premium Tier" 
    icon="⭐" 
    status="ACTIVE"
    :isOpen="activeAccordion === 'premium'"
    @click="toggleAccordion('premium')"
  >
    <div class="limits-list">
      <div class="limit-item">
        <span class="limit-label">Guides:</span>
        <span class="limit-value">✅ All Guides</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Card Check:</span>
        <span class="limit-value">175 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Bank Check:</span>
        <span class="limit-value">100 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">IVR Check:</span>
        <span class="limit-value">100 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Cookies:</span>
        <span class="limit-value">50 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">ULP:</span>
        <span class="limit-value">1000 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Inboxes:</span>
        <span class="limit-value">500 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Request Logs:</span>
        <span class="limit-value">25 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Configs:</span>
        <span class="limit-value">OB/SB/OB2</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Cards:</span>
        <span class="limit-value">5 Daily</span>
      </div>
    </div>
  </AccordionItem>

  <AccordionItem 
    type="hologram" 
    title="VIP Tier" 
    icon="👑" 
    status="ACTIVE"
    :isOpen="activeAccordion === 'vip'"
    @click="toggleAccordion('vip')"
  >
    <div class="limits-list">
      <div class="limit-item">
        <span class="limit-label">Guides:</span>
        <span class="limit-value">✅ All Guides</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Card Check:</span>
        <span class="limit-value">175 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Bank Check:</span>
        <span class="limit-value">100 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">IVR Check:</span>
        <span class="limit-value">100 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Cookies:</span>
        <span class="limit-value">25 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">ULP:</span>
        <span class="limit-value">2000 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Inboxes:</span>
        <span class="limit-value">750 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Request Logs:</span>
        <span class="limit-value">50 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Configs:</span>
        <span class="limit-value">OB/SB/BAS</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Cards:</span>
        <span class="limit-value">5 Daily</span>
      </div>
    </div>
  </AccordionItem>

  <AccordionItem 
    type="cyber" 
    title="Diamond Tier" 
    icon="💎" 
    status="ELITE"
    :isOpen="activeAccordion === 'diamond'"
    @click="toggleAccordion('diamond')"
  >
    <div class="limits-list">
      <div class="limit-item">
        <span class="limit-label">Guides:</span>
        <span class="limit-value">🌟 Elite Guides</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Card Check:</span>
        <span class="limit-value">175 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Bank Check:</span>
        <span class="limit-value">100 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">IVR Check:</span>
        <span class="limit-value">100 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Cookies:</span>
        <span class="limit-value">25 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">ULP:</span>
        <span class="limit-value">10,000 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Inboxes:</span>
        <span class="limit-value">500 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Request Logs:</span>
        <span class="limit-value">5 Daily</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Configs:</span>
        <span class="limit-value">OB/SB/BAS</span>
      </div>
      <div class="limit-item">
        <span class="limit-label">Cards:</span>
        <span class="limit-value">50 Daily</span>
      </div>
    </div>
  </AccordionItem>
</div>

## System Restrictions

<div class="restrictions-grid">
  <Feature
    icon="⏱️"
    title="Rate Limiting"
    details="Requests are rate-limited based on your plan tier to ensure system stability"
  />
  <Feature
    icon="💾"
    title="Storage Quotas"
    details="Storage limits apply to all account data including configs and results"
  />
  <Feature
    icon="🔄"
    title="Concurrent Tasks"
    details="Task limits are enforced based on plan level and current server load"
  />
</div>

## Important Notices

::: warning Fair Usage Policy
All plans are subject to fair usage policies. Abuse of the system may result in account restrictions.
:::

::: danger Abuse Prevention
Automated abuse detection systems are in place. Violations may result in immediate account termination.
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

.limits-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

.limits-list {
  margin: 1rem 0;
  padding: 1rem;
  background: var(--vp-c-bg-alt);
  border-radius: 0.5rem;
}

.limit-item {
  display: flex;
  justify-content: space-between;
  padding: 0.5rem 0;
  border-bottom: 1px solid rgba(0, 229, 255, 0.2);
}

.limit-item:last-child {
  border-bottom: none;
}

.limit-label {
  color: var(--vp-c-text-2);
}

.limit-value {
  font-weight: 500;
  color: var(--vp-c-brand);
}

.restrictions-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
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