[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Fluid type with clamp
Scale text smoothly between small and large screens.

```css
h1 {
  font-size: clamp(2rem, 2vw + 1.5rem, 3.5rem);
}
```

Why it helps: fewer breakpoints, consistent rhythm.
