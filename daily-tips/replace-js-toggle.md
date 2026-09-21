[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Replace JS with checkbox toggle
Use a checkbox to toggle a panel without scripts.

```css
.toggle {
  display: none;
}

.toggle:checked + .panel {
  display: block;
}
```

Why it helps: simple disclosure patterns with no JS.
