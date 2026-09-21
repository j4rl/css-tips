[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Fluid spacing with clamp
Scale padding and gaps smoothly across viewports.

```css
.section {
  padding: clamp(1rem, 2vw + 0.5rem, 3rem);
}
```

Why it helps: fewer breakpoints, consistent rhythm.
