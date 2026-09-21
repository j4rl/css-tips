[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Scope
Limit selector reach to a subtree with `@scope`.

```css
@scope (.card) {
  h3 {
    margin-top: 0;
  }
}
```

Why it helps: fewer long selectors and safer overrides.
