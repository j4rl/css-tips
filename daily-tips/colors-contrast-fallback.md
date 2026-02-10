# Contrast-safe fallback
Provide a simple sRGB fallback before `oklch()` for older browsers.

```css
.button {
  background: #3b82f6;
  background: oklch(62% 0.2 250);
}
```

Why it helps: progressive enhancement without sacrificing support.
