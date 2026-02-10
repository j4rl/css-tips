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
