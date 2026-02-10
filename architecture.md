# Architecture
How to keep CSS scalable and maintainable.

## Naming
- Use clear, consistent names (BEM, CUBE, or utility-first)
- Avoid overly generic class names

## Layers and order
- Organize styles from low to high specificity
- Use cascade layers to codify order

## Tokens and theming
- Store spacing, colors, and type sizes in variables
- Support themes by overriding variables

```css
:root {
  --space-1: 0.25rem;
  --space-4: 1rem;
}

[data-theme="dark"] {
  --surface: #0b1220;
}
```

## Utilities
- Use utilities for one-off styling or layout helpers
- Avoid mixing utilities and complex selectors in the same rule

## Component boundaries
- Keep component styles close to components
- Limit global styles to resets and tokens
