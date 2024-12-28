# Performance Best Practices

<BackToAdmin />

Essential guidelines for maintaining high-performance documentation.

## Core Web Vitals

<Feature
  icon="📊"
  title="Core Web Vitals"
  details="Focus on these key metrics for optimal user experience"
/>

### LCP (Largest Contentful Paint)
<Card title="LCP Optimization" icon="⚡">

- Target: Under 2.5 seconds
- Optimize image loading
- Minimize server response time
- Reduce CSS/JS blocking time

</Card>

### FID (First Input Delay)
<Card title="FID Optimization" icon="👆">

- Target: Under 100ms
- Minimize JavaScript execution
- Break up long tasks
- Optimize event handlers

</Card>

### CLS (Cumulative Layout Shift)
<Card title="CLS Prevention" icon="📏">

- Target: Under 0.1
- Set image dimensions
- Reserve space for dynamic content
- Avoid inserting content above existing content

</Card>

## Code Optimization

### JavaScript
```javascript
// Bad
import { everything } from 'large-library'

// Good
import { onlyWhatINeed } from 'large-library'
```

### CSS
```css
/* Bad */
* { box-sizing: border-box; }

/* Good */
.specific-component { box-sizing: border-box; }
```

## Checklist

<div class="checklist">
  <Card title="Initial Load" icon="🚀">

  - [ ] Minimize initial bundle size
  - [ ] Implement code splitting
  - [ ] Optimize critical rendering path
  - [ ] Enable compression

  </Card>

  <Card title="Runtime" icon="⚙️">

  - [ ] Debounce scroll/resize events
  - [ ] Use requestAnimationFrame
  - [ ] Optimize DOM operations
  - [ ] Cache expensive computations

  </Card>
</div>

<style>
.checklist {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}
</style>