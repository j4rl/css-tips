# Performance
Make styles fast to render and easy to maintain.

## Rendering cost
- Layout is expensive; avoid properties that trigger layout in animations
- Prefer `transform` and `opacity` for motion

## Paint and composite
- Large shadows and filters can be costly
- Use `will-change` sparingly

```css
.card {
  will-change: transform;
}
```

## Containment
- `contain` can reduce layout and paint scope
- `content-visibility` skips offscreen rendering

## Selector efficiency
- Avoid overly complex selectors
- Keep selector depth shallow

## Fonts
- Subset and preload critical fonts
- Avoid too many font weights
