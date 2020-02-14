## Selectors

__Charm__ uses selectors which are groups of elements defined in `core/selectors`. Styling is nested within the selector and applies to all respective child elements.

```sass
+sections
+headings
+texts
+tables
+lists
+definitions
+inputs
+radios
+buttons
+media

// examples:
// styling applied to (h1, h2, h3, h4, h5, h6) in <section>
section
  +headings
    margin: 1rem 0
    font-size: 1.1em

div
  +inputs
    font-size: .8em
```
