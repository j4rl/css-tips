[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Variables and calc
Combine custom properties with `calc()` for consistent spacing.

```css
:root {
  --space: 1rem;
}

.card {
  padding: calc(var(--space) * 1.5);
  gap: calc(var(--space) * 0.75);
}
```

Why it helps: global tweaks without hunt-and-replace.
