# OKLCH palettes
Use `oklch()` to keep lightness consistent while changing hue.

```css
:root {
  --brand-600: oklch(62% 0.2 250);
  --brand-500: oklch(68% 0.18 250);
  --brand-400: oklch(74% 0.16 250);
}
```

Why it helps: lightness stays predictable, so gradients and scales feel even.
