# Asset Loading

<BackToAdmin />

Optimize how assets are loaded and managed in your documentation.

## Resource Prioritization

<Card title="Loading Priorities" icon="📊">

### Critical Resources
- CSS in `<head>`
- Above-the-fold content
- Core JavaScript

### Deferred Resources
- Below-fold images
- Non-critical scripts
- Third-party widgets

</Card>

## Loading Strategies

### Preloading Critical Assets

```html
<link rel="preload" href="/critical.css" as="style">
<link rel="preload" href="/hero-image.jpg" as="image">
```

### Resource Hints

```html
<!-- Preconnect to required origins -->
<link rel="preconnect" href="https://api.example.com">

<!-- Prefetch for likely navigation -->
<link rel="prefetch" href="/likely-next-page.html">
```

## Performance Metrics

<div class="metrics-grid">
  <Card title="First Paint" icon="🎨">
    Time until first visual render
  </Card>

  <Card title="LCP" icon="⚡">
    Largest Contentful Paint
  </Card>

  <Card title="TTI" icon="👆">
    Time to Interactive
  </Card>

  <Card title="CLS" icon="📏">
    Cumulative Layout Shift
  </Card>
</div>

<style>
.metrics-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
  margin: 2rem 0;
}
</style>