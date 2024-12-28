# Tools Setup

Essential tools and configurations for your training environment.

## Required Tools

<div class="tools-grid">
  <Feature
    icon="🔧"
    title="Core Tools"
    details="Essential software for basic operations"
  />
  <Feature
    icon="🛠️"
    title="Advanced Tools"
    details="Specialized tools for complex tasks"
  />
  <Feature
    icon="⚙️"
    title="Configuration Tools"
    details="Tools for managing settings and profiles"
  />
</div>

## Setup Instructions

<Card title="Installation Steps" icon="📥">

1. Download required software
2. Configure environment
3. Set up security measures
4. Test installation

</Card>

## Security Guidelines

::: warning Important
Always follow security best practices when setting up tools
:::

<style>
.tools-grid {
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