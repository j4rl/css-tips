# :has() and :is()
Use `:is()` to reduce selector repetition and `:has()` for parent state.

```css
.card :is(h2, h3, h4) {
  margin-top: 0;
}

.field:has(input:invalid) {
  border-color: #b91c1c;
}
```

Why it helps: cleaner selectors and state-driven styles.
