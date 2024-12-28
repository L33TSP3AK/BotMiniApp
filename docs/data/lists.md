# Lists

Various ways to display lists and collections.

## Unordered Lists

- First item
- Second item
  - Nested item 1
  - Nested item 2
- Third item

## Ordered Lists

1. First step
2. Second step
   1. Sub-step one
   2. Sub-step two
3. Third step

## Custom List Styles

<div class="custom-list">
  <div class="list-item">
    <span class="list-icon">📌</span>
    <div class="list-content">
      <h3>Pinned Item</h3>
      <p>Description for the pinned item</p>
    </div>
  </div>
  
  <div class="list-item">
    <span class="list-icon">⭐</span>
    <div class="list-content">
      <h3>Featured Item</h3>
      <p>Description for the featured item</p>
    </div>
  </div>
</div>

<style>
.custom-list {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  margin: 2rem 0;
}

.list-item {
  display: flex;
  gap: 1rem;
  padding: 1rem;
  background: white;
  border-radius: 0.5rem;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
}

.list-icon {
  font-size: 1.5rem;
}

.list-content h3 {
  margin: 0 0 0.5rem 0;
}

.list-content p {
  margin: 0;
  color: #666;
}
</style>