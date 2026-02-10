# Content visibility
Skip offscreen rendering for long pages.

```css
.card-list {
  content-visibility: auto;
  contain-intrinsic-size: 1px 800px;
}
```

Why it helps: faster initial render and scrolling.
