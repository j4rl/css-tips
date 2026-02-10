# Staggered entrances
Stagger a list with a simple delay calc.

```css
.item {
  animation: rise 400ms ease both;
  animation-delay: calc(var(--i) * 80ms);
}
```

Why it helps: subtle motion without complex timelines.
