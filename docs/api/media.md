## Media Queries

### media
`@media` declarations.
```sass
// media($feature, $value, $type)
// default $type is `screen`

// width
nav
  +media(min, small) //or min-width
  +media(max, 400px) //or max-width

// height
div
  +media(min-height, 800px)
  +media(max-height, 1080px, screen-only)

// color
input
  +media(color)
  +media(min-color, 8)
  +media(max-color, 16)

// hover
button
  +media(hover)
```

### hide
Hides element with `display: none` at breakpoint.
```sass
// hide($feature, $value, $type)
aside
  +hide(max, phone)
```
