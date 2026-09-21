[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Box sizing reset
Make sizing predictable across components.

```css
*, *::before, *::after {
  box-sizing: border-box;
}
```

Why it helps: borders and padding stay inside widths.
