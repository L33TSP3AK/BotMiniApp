# Advanced Accordions

<div class="accordion-container">
  <h2>Accordion Styles</h2>
  
  <AccordionItem 
    type="cyber"
    title="System Status"
    icon="⚡"
    status="ONLINE"
  >
    <CyberList :items="[
      { text: 'CPU Load', value: '45%' },
      { text: 'Memory', value: '2.4GB/8GB' },
      { text: 'Network', value: '100Mbps' }
    ]" />
  </AccordionItem>

  <AccordionItem
    type="neon"
    title="Neon Style"
    icon="💫"
  >
    <p>This accordion features a neon glow effect with vibrant colors.</p>
  </AccordionItem>

  <AccordionItem
    type="hologram"
    title="Holographic Display"
    icon="🌐"
  >
    <p>Experience the futuristic hologram effect in this accordion.</p>
  </AccordionItem>
</div>

<style>
.accordion-container {
  padding: 2rem;
  background: var(--vp-c-bg-soft);
  border-radius: 1rem;
  margin: 2rem 0;
}
</style>