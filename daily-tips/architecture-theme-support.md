[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Dark/light theme support
Use CSS variables and `prefers-color-scheme` for theme-aware tokens.

```css
:root {
  color-scheme: light dark;
  --surface: #ffffff;
  --text: #0f172a;
}

@media (prefers-color-scheme: dark) {
  :root {
    --surface: #0b1220;
    --text: #e2e8f0;
  }
}
```

Why it helps: one set of components, two themes.
