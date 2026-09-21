[← Back to README](../README.md) · [Daily tips index](../css_tip_of_the_day.md)

# Split color and type tokens
Keep color and typography variables in separate files.

```css
/* colors.css */
:root {
  --surface: #ffffff;
  --text: #0f172a;
}

/* typography.css */
:root {
  --font-body: "IBM Plex Sans", sans-serif;
  --font-size-1: 1rem;
}
```

Why it helps: clearer ownership and easier theming.
