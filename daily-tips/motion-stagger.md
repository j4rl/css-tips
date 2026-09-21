[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Staggered entrances
Stagger a list with a simple delay calc.

```css
.item {
  animation: rise 400ms ease both;
  animation-delay: calc(var(--i) * 80ms);
}
```

Why it helps: subtle motion without complex timelines.
