# Info Boxes

Enhanced information containers with various styles and purposes.

## Basic Info Box

<div class="info-box">
  <div class="info-icon">💡</div>
  <div class="info-content">
    <h3>Quick Tip</h3>
    <p>Here's a helpful tip to improve your workflow.</p>
  </div>
</div>

## Info Box Variants

<div class="info-box primary">
  <div class="info-icon">📘</div>
  <div class="info-content">
    <h3>Documentation</h3>
    <p>Read the documentation for more details.</p>
  </div>
</div>

<div class="info-box secondary">
  <div class="info-icon">🎯</div>
  <div class="info-content">
    <h3>Best Practice</h3>
    <p>Follow these guidelines for best results.</p>
  </div>
</div>

<div class="info-box accent">
  <div class="info-icon">✨</div>
  <div class="info-content">
    <h3>Pro Tip</h3>
    <p>Advanced users can take advantage of this feature.</p>
  </div>
</div>

<style>
.info-box {
  display: flex;
  gap: 1rem;
  padding: 1.5rem;
  border-radius: 0.75rem;
  margin: 1rem 0;
  background: var(--vp-c-bg-soft);
  border: 1px solid var(--vp-c-border);
  transition: transform 0.2s ease;
}

.info-box:hover {
  transform: translateY(-2px);
}

.info-icon {
  font-size: 1.5rem;
}

.info-content h3 {
  margin: 0 0 0.5rem 0;
}

.info-content p {
  margin: 0;
  color: var(--vp-c-text-2);
}

.info-box.primary {
  background: #e0f2fe;
  border-color: #0ea5e9;
}

.info-box.secondary {
  background: #f0fdf4;
  border-color: #22c55e;
}

.info-box.accent {
  background: #fdf4ff;
  border-color: #d946ef;
}
</style>