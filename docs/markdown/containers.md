# Custom Containers

<BackToAdmin />

Suports custom containers

## Basic Containers

::: tip
This is a tip container
:::

::: warning
This is a warning container
:::

::: danger
This is a danger container
:::

::: info
This is an info container
:::

## Custom Styled Containers

<div class="custom-block">
  <p class="custom-block-title">💡 Pro Tip</p>
  <p>Here's a custom-styled container with an icon.</p>
</div>

<div class="custom-block important">
  <p class="custom-block-title">🔑 Important Note</p>
  <p>This container uses custom styling for important information.</p>
</div>

## Collapsible Details

::: details Click me to view more
Here's some hidden content that can be revealed by clicking!

```js
console.log('Hello from the hidden section!')
```
:::

## Code Group Container

::: code-group
```js [config.js]
export default {
  title: 'My Site',
  description: 'Just playing around.'
}
```

```ts [config.ts]
export default defineConfig({
  title: 'My Site',
  description: 'Just playing around.'
})
```
:::