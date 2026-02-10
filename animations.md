# Animations
Motion that is purposeful and performant.

## Transitions
- Use `transform` and `opacity` for smooth animations
- Keep transitions short and consistent

```css
.button {
  transition: transform 120ms ease, box-shadow 120ms ease;
}

.button:hover {
  transform: translateY(-1px);
}
```

## Keyframes
- Use keyframes for multi-step motion
- Prefer `animation-fill-mode: both` for predictable states

## Reduced motion
- Respect user preference with `prefers-reduced-motion`

```css
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

## Scroll-driven animations
- Use `@scroll-timeline` and `animation-timeline` when supported
- Provide a non-animated fallback
