# Vue in Markdown

<BackToAdmin />

Learn how to use Vue components and features directly in markdown files.

## Using Components

<Feature 
  icon="⚡"
  title="Vue Components"
  details="Use Vue components directly in your markdown content."
/>

## Template Syntax

### Text Interpolation
{{ 1 + 1 }} equals 2

### Directives
<div v-for="i in 3" :key="i">Item {{ i }}</div>

## Script Setup

```vue
<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <button @click="count++">Count: {{ count }}</button>
</template>
```

## Interactive Example

<div class="demo-component">
  <h3>Counter Demo</h3>
  <p>Current count: {{ count }}</p>
  <button @click="count++">Increment</button>
  <button @click="count--">Decrement</button>
</div>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<style>
.demo-component {
  padding: 1.5rem;
  border-radius: 0.5rem;
  background: var(--vp-c-bg-soft);
  margin: 1rem 0;
}

.demo-component button {
  margin: 0.5rem;
  padding: 0.5rem 1rem;
  border-radius: 0.25rem;
  background: var(--vp-c-brand);
  color: white;
  border: none;
  cursor: pointer;
}

.demo-component button:hover {
  opacity: 0.9;
}
</style>