# Animated border
Animate a gradient border with `background-size`.

```css
.glow {
  border: 2px solid transparent;
  background:
    linear-gradient(#0b1220, #0b1220) padding-box,
    linear-gradient(120deg, #22d3ee, #a78bfa, #f472b6) border-box;
  background-size: 100% 100%, 200% 200%;
  animation: border-shift 6s linear infinite;
}

@keyframes border-shift {
  0% { background-position: 0 0, 0 0; }
  100% { background-position: 0 0, 200% 0; }
}
```

Why it helps: flashy borders without extra elements.
