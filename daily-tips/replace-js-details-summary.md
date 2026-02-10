# Replace JS with details/summary
Use native disclosure widgets and style them.

```css
details {
  border: 1px solid #e2e8f0;
  border-radius: 0.5rem;
  padding: 0.75rem 1rem;
}

details[open] {
  border-color: #94a3b8;
}
```

Why it helps: built-in keyboard and screen reader support.
