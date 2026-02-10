# Advanced
Modern and emerging CSS features.

## Cascade layers
- Use layers to control priority between resets, components, and utilities

```css
@layer reset, base, components, utilities;

@layer reset {
  *, *::before, *::after { box-sizing: border-box; }
}
```

## Scope
- `@scope` limits selector reach within a subtree
- Use it to reduce long selector chains

## Subgrid
- Use `subgrid` to align nested layouts

```css
.grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
}

.child {
  display: grid;
  grid-template-columns: subgrid;
}
```

## :has()
- Use parent state styling without JavaScript

```css
.field:has(input:invalid) {
  border-color: #b91c1c;
}
```

## CSS Houdini
- Use `paint()` for custom effects
- Prefer progressive enhancement
