# Code Blocks

Display and format code snippets with syntax highlighting.

## Basic Code Block

```javascript
function greet(name) {
  return `Hello, ${name}!`;
}

// Usage
console.log(greet('World'));
```

## Code Groups

::: code-group
```js [JavaScript]
const sum = (a, b) => a + b;
```

```python [Python]
def sum(a, b):
    return a + b
```

```ruby [Ruby]
def sum(a, b)
  a + b
end
```
:::

## With Line Numbers

```javascript{1,3-4}
import { ref } from 'vue'

function counter() {
  const count = ref(0)
  return { count }
}
```

## With Line Highlights

```javascript
// [!code focus]
function highlight() {
  console.log('This line is highlighted')
}

// [!code warning]
function warning() {
  console.log('This is a warning')
}

// [!code error]
function error() {
  console.log('This shows an error')
}
```