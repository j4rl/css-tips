[← Back to README](README.md)

# Glossary

Common CSS terms, with a bit more practical context.

- Cascade: The process CSS uses to resolve conflicts between multiple rules. The cascade considers origin, importance, specificity, and source order, which is why a later rule can override an earlier one when the selectors are equally specific.
- Specificity: A value that helps browsers decide which selector wins when several rules target the same element. In practice, IDs are strongest, then classes and attributes, then elements and pseudo-elements. Specificity is one of the reasons it is often better to write clear selectors and use layers instead of relying on overly specific rules.
- Inheritance: The way some CSS properties are passed from parent elements to their children. Text-related properties such as color, font, and line-height commonly inherit, while box layout properties like width, margin, and padding usually do not.
- Formatting context: The layout rules that a block or inline formatting context imposes on its children. Understanding formatting context helps explain why floats, flex containers, grid containers, and block formatting contexts behave differently from normal flow.
- Stacking context: A hierarchy created by elements that affect painting order, such as positioned elements with z-index, transforms, opacity, and certain filters. Stacking contexts help determine which elements appear above or below others in overlapping layouts.
- Containing block: The nearest ancestor box that defines the coordinate system and size context for positioned descendants. It is important when working with absolute and fixed positioning, and it affects how percentages and offsets are resolved.
- Replaced element: An element whose rendered output is controlled by an external resource instead of its HTML content, such as `img`, `video`, `iframe`, or `input`. These elements have intrinsic sizing and often need special handling in layout and styling.
- Intrinsic size: The natural size an element wants to be based on its content or external resource, before CSS layout constraints are applied. Images, media, and text-based elements often have useful intrinsic dimensions that influence the layout before explicit widths or heights are set.
- Box model: The mental model for how an element's content, padding, border, and margin combine into its total size. The default box-sizing behavior is content-box, which can make widths confusing, so `box-sizing: border-box` is often used to make sizing more predictable.
- Normal flow: The default layout behavior in CSS where block elements stack vertically and inline elements flow horizontally. Normal flow is the baseline that flexbox, grid, absolute positioning, and float layouts build on.
- Relative unit: A unit whose value is computed from another measure, such as `em`, `rem`, `%`, or viewport units. These units help maintain proportional sizing and make components more adaptable across contexts.
- Min/max sizing: CSS functions and properties that constrain a value between a lower and upper bound, such as `min()`, `max()`, and `clamp()`. They are useful for flexible typography, responsive spacing, and making layouts adapt without jumping between breakpoints.
- Layout algorithm: The CSS system used to place and size elements, such as block layout, flex layout, grid layout, or multicolumn layout. Each algorithm has different rules for alignment, spacing, and sizing, which is why picking the right one matters.
- Pseudo-class: A selector keyword that matches elements based on state or relation, such as `:hover`, `:focus`, `:nth-child()`, or `:checked`. Pseudo-classes are a core part of modern CSS and allow styling without changing the HTML structure.
- Pseudo-element: A virtual element created by CSS to style part of an existing element, such as `::before`, `::after`, or `::first-line`. They are useful for decorative or structural details that do not require extra markup.
- Aspect ratio: The relationship between an element's width and height, expressed as `width / height`. CSS `aspect-ratio` lets you maintain a consistent shape for media and cards without manually calculating height.
- Accessibility tree: The logical structure that assistive technologies use to interpret and navigate a page. CSS can affect visual presentation without changing the accessibility tree, so semantics and focus states still matter.
