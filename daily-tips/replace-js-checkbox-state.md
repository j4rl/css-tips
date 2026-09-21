[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Checkbox state to style siblings
Use sibling selectors to toggle styles without JS.

```css
input[type="checkbox"] {
  display: none;
}

input[type="checkbox"]:checked + .panel {
  max-height: 12rem;
  opacity: 1;
}
```

Why it helps: simple state-driven UI with pure CSS.
