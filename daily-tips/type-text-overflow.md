[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Text overflow
Use `text-overflow: ellipsis` for single-line truncation.

```css
.title {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
```

Why it helps: prevents long titles from breaking layouts.
