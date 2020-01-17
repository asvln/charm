## Media Queries

### media
`@media` declarations
```sass
// media($value, $feature, $type)
nav
  +media(min, small) //min-width
  +media(max, desktop) //max-width
  +media(min-height, 400px)
  +media(max-height, 800px)
  +media(portrait)
  +media(landscape)
  +media(hover)
  +media(color)
```

### hide
hides element with `display: none`
```sass
// hide($value, $feature, $type)
aside
  +hide(max, phone)
```

### scroll
sets `height` or `width` and applies the `overflow: scroll`
```sass
// hide($value, $feature, $display: block)
div
  +scroll                 // `overflow: scroll`
  +scroll(400px)          // scroll at height of 400px
  +scroll(desktop, width) // scroll at width of 1200px
```
