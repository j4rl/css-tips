# Subgrid alignment
Align nested items to the parent grid.

```css
.grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
}

.card {
  display: grid;
  grid-template-columns: subgrid;
}
```

Why it helps: consistent column alignment across components.
