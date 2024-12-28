# Tooltips

Tooltips provide additional information when hovering over elements.

## Basic Tooltips

<div class="tooltip-demo">
  <span class="tooltip" data-tooltip="This is a tooltip">Hover me</span>
</div>

## Tooltip Positions

<div class="tooltip-demo">
  <span class="tooltip tooltip-top" data-tooltip="Top tooltip">Top</span>
  <span class="tooltip tooltip-right" data-tooltip="Right tooltip">Right</span>
  <span class="tooltip tooltip-bottom" data-tooltip="Bottom tooltip">Bottom</span>
  <span class="tooltip tooltip-left" data-tooltip="Left tooltip">Left</span>
</div>

## Implementation

```vue
<template>
  <span class="tooltip" data-tooltip="Tooltip text">
    Hover element
  </span>
</template>

<style>
.tooltip {
  position: relative;
  display: inline-block;
  cursor: pointer;
}

.tooltip::after {
  content: attr(data-tooltip);
  position: absolute;
  /* Additional styling */
}
</style>
```

<style>
.tooltip-demo {
  display: flex;
  gap: 1rem;
  margin: 2rem 0;
}

.tooltip {
  position: relative;
  display: inline-block;
  padding: 0.5rem 1rem;
  background: #f3f4f6;
  border-radius: 0.25rem;
  cursor: pointer;
}

.tooltip::after {
  content: attr(data-tooltip);
  position: absolute;
  background: #1f2937;
  color: white;
  padding: 0.25rem 0.5rem;
  border-radius: 0.25rem;
  font-size: 0.875rem;
  white-space: nowrap;
  opacity: 0;
  pointer-events: none;
  transition: all 0.2s ease;
}

.tooltip:hover::after {
  opacity: 1;
}

.tooltip-top::after {
  bottom: 100%;
  left: 50%;
  transform: translateX(-50%) translateY(-0.5rem);
}

.tooltip-right::after {
  top: 50%;
  left: 100%;
  transform: translateY(-50%) translateX(0.5rem);
}

.tooltip-bottom::after {
  top: 100%;
  left: 50%;
  transform: translateX(-50%) translateY(0.5rem);
}

.tooltip-left::after {
  top: 50%;
  right: 100%;
  transform: translateY(-50%) translateX(-0.5rem);
}
</style>