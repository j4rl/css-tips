[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Focus-visible outlines
Show focus for keyboard users without noisy mouse focus.

```css
.link:focus-visible {
  outline: 2px solid #2563eb;
  outline-offset: 2px;
}
```

Why it helps: accessible focus with minimal visual clutter.
