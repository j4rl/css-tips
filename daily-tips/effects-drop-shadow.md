[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Drop shadow for transparent images
Use `drop-shadow()` to shadow non-rectangular PNG or SVG.

```css
.logo {
  filter: drop-shadow(0 6px 12px rgba(0, 0, 0, 0.2));
}
```

Why it helps: shadows follow the visible shape.
