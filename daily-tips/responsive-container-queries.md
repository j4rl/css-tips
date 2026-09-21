[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Container queries
Make components respond to their container, not the viewport.

```css
.card {
  container-type: inline-size;
}

@container (min-width: 28rem) {
  .card {
    display: grid;
    grid-template-columns: auto 1fr;
  }
}
```

Why it helps: reusable components that scale in any layout.
