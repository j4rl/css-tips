# Color mix for tints
Use `color-mix()` to generate consistent tints and shades.

```css
:root {
  --brand: oklch(62% 0.2 250);
}

.button {
  background: color-mix(in oklch, var(--brand), white 20%);
}
```

Why it helps: faster palette tweaks without manual hex math.
