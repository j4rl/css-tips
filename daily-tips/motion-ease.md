[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Better easing curve
Use a custom cubic-bezier for snappier UI motion.

```css
.button {
  transition: transform 180ms cubic-bezier(0.2, 0.8, 0.2, 1);
}
```

Why it helps: avoids slow, mushy transitions.
