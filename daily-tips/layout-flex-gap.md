[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Flex gap
Use `gap` in flex layouts instead of margins on children.

```css
.row {
  display: flex;
  gap: 1rem;
  align-items: center;
}
```

Why it helps: easier spacing control and no edge trimming.
