# Typography
Readable and expressive type on the web.

## Font loading
- Use `font-display: swap` for performance
- Subset fonts when possible

```css
@font-face {
  font-family: "Example Sans";
  src: url("example-sans.woff2") format("woff2");
  font-display: swap;
}
```

## Line length and rhythm
- Aim for 45 to 75 characters per line
- Use `line-height` between 1.4 and 1.7 for body text
- Use `ch` for ideal widths

```css
.prose {
  max-width: 70ch;
  line-height: 1.6;
}
```

## Variable fonts
- Set `font-variation-settings` only when necessary
- Prefer `font-weight` and `font-stretch` first

## Text flow
- Use `hyphens: auto` for long words
- Use `text-wrap: balance` on short headings

```css
h1, h2 {
  text-wrap: balance;
}
```
