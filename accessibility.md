# Accessibility
Inclusive CSS patterns.

## Focus and visibility
- Always show focus states
- Use `:focus-visible` for keyboard-only focus

```css
.link:focus-visible {
  outline: 2px solid #2563eb;
  outline-offset: 2px;
}
```

## Reduced motion
- Respect user settings
- Avoid parallax in the base experience

## Color and contrast
- Ensure text and interactive controls meet contrast requirements
- Avoid color-only state changes

## Touch targets
- Minimum 44 by 44 px for touch targets
- Use padding rather than scaling text
