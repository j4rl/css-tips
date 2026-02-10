# Responsive
Design that adapts to content and screens.

## Media queries
- Use mobile-first: start with the base styles, then add breakpoints
- Favor `min-width` breakpoints for clarity

```css
.nav {
  gap: 1rem;
}

@media (min-width: 48rem) {
  .nav {
    gap: 2rem;
  }
}
```

## Container queries
- Use them for component-level responsiveness
- Pair with `container-type: inline-size`

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

## Fluid sizing
- Use `clamp()` to scale text and spacing

```css
h1 {
  font-size: clamp(2rem, 2vw + 1.5rem, 3.5rem);
}
```

## Viewport units
- Prefer `dvh` and `dvw` for mobile toolbars
- Use `svh` when you want the smallest possible viewport height

## Responsiveness by using grid
- Use `minmax()` and `auto-fit`/`auto-fill` for responsive grids
```css
.grid {
  display: grid;
  gap: 1rem;
  grid-template-columns: repeat(auto-fit, minmax(14rem, 1fr));
}
```
- You can also use `auto-fill` instead of `auto-fit` depending on your layout needs

## Responsiveness by using flex
- Use `flex-wrap: wrap` to allow items to wrap on smaller screens
- Use `gap` to control spacing between flex items
- Use `justify-content` and `align-items` to control alignment within the flex container

## Special considerations for mobile phones
- Use `dvh` and `dvw` viewport units to handle mobile browser UI changes
- Use `svh` when you want the smallest possible viewport height
- Scroll events can affect viewport size and layout
- Consider using `env(safe-area-inset-*)` for devices with notches or rounded corners
- Hovering can be tricky on touch devices; consider using `@media (hover: hover)` to target devices that support hover or fine pointer interactions