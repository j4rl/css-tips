# Effects
Shadows, filters, blends, and masking.

## Shadows
- Use layered shadows for depth
- Avoid heavy blur for performance

```css
.card {
  box-shadow:
    0 1px 2px rgba(0, 0, 0, 0.08),
    0 8px 24px rgba(0, 0, 0, 0.12);
}
```

## Filters
- `filter` affects the whole element, `backdrop-filter` affects behind it
- Provide fallbacks for unsupported browsers

```css
.glass {
  background: rgba(255, 255, 255, 0.2);
  backdrop-filter: blur(12px);
}
```

## Blend modes
- Use `mix-blend-mode` carefully for text and icons
- Test contrast in multiple backgrounds

## Masking and clipping
- `clip-path` for simple shapes
- `mask-image` for complex fades and cutouts
