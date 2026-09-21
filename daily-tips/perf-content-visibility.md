[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Content visibility
Skip offscreen rendering for long pages.

```css
.card-list {
  content-visibility: auto;
  contain-intrinsic-size: 1px 800px;
}
```

Why it helps: faster initial render and scrolling.
