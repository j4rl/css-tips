# Layout
How elements flow and how to arrange them on the page.

## Normal flow
- Use margins and `gap` in layout containers
- Avoid clearing hacks; use flex or grid where possible

## Flexbox
- Best for one-dimensional layouts
- Main axis: `flex-direction` and `justify-content`
- Cross axis: `align-items` and `align-content`
- `gap` works in modern browsers

```css
.row {
  display: flex;
  gap: 1rem;
  align-items: center;
}
```

## Grid
- Best for two-dimensional layouts
- Use `minmax()` and `auto-fit`/`auto-fill` for responsive grids

```css
.grid {
  display: grid;
  gap: 1rem;
  grid-template-columns: repeat(auto-fit, minmax(14rem, 1fr));
}
```

## Positioning
- `relative` moves an element and creates a containing block
- `absolute` removes from flow; `fixed` binds to viewport
- `sticky` works within scroll containers

## Alignment
- Prefer `align-*` and `justify-*` over manual margins
- Use `place-*` shorthands where it improves readability

## Containment
- `contain` and `content-visibility` can improve performance

```css
.card-list {
  content-visibility: auto;
  contain-intrinsic-size: 1px 800px;
}
```
## Columns
- Use columns for multi-column text layouts
- Control column width and gap with `column-width` and `column-gap`
- Use `column-count` to specify the number of columns
- Use `break-inside` to control how content breaks between columns
- Use `break-before` and `break-after` to control breaks before and after elements
- Can be used as a masonry look.
