# Tips and tricks
Quick patterns you can reuse.

## Centering
```css
.center {
  display: grid;
  place-items: center;
}
```

## Fluid cards
```css
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(16rem, 1fr));
  gap: 1rem;
}
```

## Scroll snap
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

## Aspect ratio
```css
.media {
  aspect-ratio: 16 / 9;
  object-fit: cover;
}
```

## Hide visually, keep for screen readers
```css
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  border: 0;
}
```
