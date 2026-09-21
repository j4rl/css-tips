[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Safer viewport height units
Use `dvh` to avoid mobile browser UI jumps.

```css
.hero {
  min-height: 100vh;
  min-height: 100dvh;
}
```

Why it helps: the second line overrides when supported.
