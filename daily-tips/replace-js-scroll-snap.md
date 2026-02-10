# Replace JS with scroll snap
Build a simple carousel without JS.

```css
.carousel {
  display: grid;
  grid-auto-flow: column;
  grid-auto-columns: 80%;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
}

.carousel > * {
  scroll-snap-align: start;
}
```

Why it helps: smooth native scrolling and less code.
