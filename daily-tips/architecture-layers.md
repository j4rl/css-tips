# @layer organization
Use cascade layers to control priority between resets and components.

```css
@layer reset, base, components, utilities;

@layer reset {
  *, *::before, *::after { box-sizing: border-box; }
}
```

Why it helps: predictable overrides without specificity wars.
