# Responsive Design

<BackToAdmin />

Learn how to create responsive layouts that work across all devices.

## Responsive Grid Example

<div class="responsive-grid">
  <div class="grid-item">Item 1</div>
  <div class="grid-item">Item 2</div>
  <div class="grid-item">Item 3</div>
  <div class="grid-item">Item 4</div>
</div>

## Breakpoint System

<Card title="Breakpoint Reference" icon="📱">

- Mobile: < 640px
- Tablet: 640px - 1024px
- Desktop: > 1024px

</Card>

## Media Query Examples

```css
/* Mobile First Approach */
.container {
  width: 100%;
  padding: 1rem;
}

/* Tablet */
@media (min-width: 640px) {
  .container {
    max-width: 640px;
    padding: 2rem;
  }
}

/* Desktop */
@media (min-width: 1024px) {
  .container {
    max-width: 1024px;
    padding: 3rem;
  }
}
```

<style>
.responsive-grid {
  display: grid;
  gap: 1rem;
  margin: 2rem 0;
  grid-template-columns: repeat(1, 1fr);
}

@media (min-width: 640px) {
  .responsive-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 1024px) {
  .responsive-grid {
    grid-template-columns: repeat(4, 1fr);
  }
}

.grid-item {
  padding: 2rem;
  background: var(--vp-c-bg-soft);
  border-radius: 0.5rem;
  text-align: center;
  transition: transform 0.2s;
}

.grid-item:hover {
  transform: scale(1.05);
}
</style>