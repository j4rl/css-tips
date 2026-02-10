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
