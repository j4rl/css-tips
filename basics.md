# Basics
Core concepts that make everything else work.

## The cascade
- Origin and importance: user agent < user < author, and `!important` only when required (use @layers instead)
- Specificity: inline > IDs > classes/attributes/pseudo-classes > elements
- Order: later rules win when specificity matches

## Inheritance
- Many text properties inherit (font, color), layout generally does not
- Use `inherit`, `initial`, `unset`, and `revert` intentionally

## Box model
- Content, padding, border, margin
- Prefer `box-sizing: border-box` for predictable sizing

```css
*, *::before, *::after {
  box-sizing: border-box;
}
```

## Display
- `block` and `inline` define formatting context
- `inline-block` respects width and height but flows inline
- `none` removes element from layout and accessibility tree

## Units
- `px` for borders and hairlines 
  (1px = 1 device pixel)
- `em` and `rem` for typography and component sizing 
  (em is relative to the parent, rem is relative to the root)
- `vw`, `vh`, `dvw`, `dvh` for viewport-based layout 
  (viewport width and height, dynamic viewport width and height)
- `ch` for line length and `lh` for vertical rhythm 
  (ch is the width of the "0" character, lh is the line height)

## Sizing
- Use `min()`, `max()`, and `clamp()` for fluid sizing
 - `min()`, `max()` works like this: `min(value1, value2, ...)` and `max(value1, value2, ...)`
    (the 'max' in the function max refers to the maximum value among the arguments, the other way with 'min')
 - `clamp()` works like this: `clamp(minimum, preferred, maximum)`
- Pair `min-width` and `max-width` to constrain layouts

```css
.content {
  width: min(70ch, 90vw);
}
```

## The containing block
- Many properties resolve against the nearest containing block
- `position: relative` on a parent sets a containing block for absolute children

## Stacking context
- Created by `position` plus `z-index`, `opacity < 1`, `transform`, and others
- Keep `z-index` scales documented to avoid conflicts
