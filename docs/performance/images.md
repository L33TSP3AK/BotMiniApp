# Image Optimization

<BackToAdmin />

Best practices for optimizing images in your documentation.

## Image Loading Strategies

<Card title="Lazy Loading" icon="🔄">

```html
<img loading="lazy" src="/large-image.jpg" alt="Lazy loaded image">
```

- Defers loading until image is near viewport
- Reduces initial page load time
- Saves bandwidth for unused images

</Card>

## Responsive Images

```html
<picture>
  <source media="(min-width: 800px)" srcset="/large.jpg">
  <source media="(min-width: 400px)" srcset="/medium.jpg">
  <img src="/small.jpg" alt="Responsive image">
</picture>
```

## Image Format Guidelines

<div class="format-grid">
  <Card title="JPEG" icon="📸">
    - Best for photographs
    - Lossy compression
    - Smaller file sizes
  </Card>

  <Card title="PNG" icon="🎨">
    - Best for graphics
    - Lossless quality
    - Supports transparency
  </Card>

  <Card title="WebP" icon="🚀">
    - Modern format
    - Better compression
    - Wide browser support
  </Card>

  <Card title="SVG" icon="✨">
    - Vector graphics
    - Scalable
    - Small file size
  </Card>
</div>

## Optimization Checklist

<Feature
  icon="✅"
  title="Optimization Steps"
  details="Follow these steps to ensure optimal image performance"
/>

1. Choose the right format
2. Compress images appropriately
3. Use responsive images
4. Implement lazy loading
5. Provide alt text for accessibility

<style>
.format-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 1rem;
  margin: 2rem 0;
}
</style>