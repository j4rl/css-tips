[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Grid auto-fit cards
Let the grid choose how many columns fit the space.

```css
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(16rem, 1fr));
  gap: 1rem;
}
```

Why it helps: responsive grids with no extra breakpoints.
