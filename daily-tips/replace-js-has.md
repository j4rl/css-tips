# Replace JS with :has()
Style a parent based on its children without JavaScript.

```css
.field:has(input:invalid) {
  border-color: #b91c1c;
}
```

Why it helps: fewer scripts, clearer state styling.
