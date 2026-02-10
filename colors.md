# Colors
Modern color workflows and contrast-safe choices.

## Different ways to set colors
- Named colors
- Hexadecimal colors 
  - `#RRGGBB` and `#RGB` shorthand
  - If you add alpha, use `#RRGGBBAA` or `#RGBA` shorthand
  (Alpha channel is the transparency component)
- RGB and RGBA
  - `rgb(redvalue, greenvalue, bluevalue)` and `rgba(redvalue, greenvalue, bluevalue, alpha)`
  (values range from 0 to 255 for red, green, and blue; alpha ranges from 0 to 1)
- HSL and HSLA
  - `hsl(hue, saturation, lightness)` and `hsla(hue, saturation, lightness, alpha)`
  (hue ranges from 0 to 360 degrees, saturation and lightness are percentages, alpha ranges from 0 to 1)
- CSS Color Module Level 4 functions like `oklch()` and `oklab()`
  - `oklch(Lightness Chroma Hue)` and `oklab(Lightness a b)` where a and b are color components
  (Lightness, Chroma, and Hue represent perceptual color attributes)
  (Lightness, a, and b represent color components which define color in the Oklab color space)
  Read more here: https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/oklch


## Color spaces
- Prefer `oklch()` and `oklab()` for perceptual consistency
- Convert to `srgb` for broad support if needed

```css
:root {
  --brand: oklch(62% 0.2 250);
}
```

## Contrast
- Check contrast for text and UI controls
- Use `color-contrast()` when available, with fallbacks

## Gradients
- Use gradients to create depth or highlight, not to decorate everything
- Keep gradient angles consistent within a theme

```css
.hero {
  background: linear-gradient(135deg, #0b1c2d, #1b4d8a);
}
```

## Tokens
- Store colors as CSS variables
- Keep a small, curated palette and derive scales

```css
:root {
  --neutral-900: #0f172a;
  --neutral-100: #f8fafc;
}
```
