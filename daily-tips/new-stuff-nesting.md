# CSS nesting
Group related selectors without repeating the parent.

```css
.card {
  padding: 1rem;

  & h3 {
    margin-top: 0;
  }

  & .meta {
    color: #64748b;
  }
}
```

Why it helps: clearer structure and fewer selector typos.
