## Block
Quickly define `display`, `position`, and place positioned elements with `offset`.

### offset
```sass
// offset($arg)
// sides: (top, right, bottom, left)
// keywords: (auto, initial, inherit, unset, 0)
// default value: `0`

div
  +offset(top)
  // div { top: 0; }
  +offset(top 2em)
  // div { top: 2em; }
  +offset(bottom auto right)
  // div { bottom: auto; right: 0; }
```

### block
```sass
// block($position, $offset)
// default: 'display: block'
div
  +block(sticky, top)
```

### inline-block
```sass
// inline-block($position, $offset)
// default: 'display: inline-block'
div
  +inline-block(relative, top 5px left 5px)
```

### inline
```sass
// inline($position, $offset)
// default: 'display: inline-block'
div
  +inline(relative, bottom 2em)
```

## Position
Quickly define `position` and optional `offset`.

### sticky
```sass
// sticky($offset)
div
  +sticky(bottom)
```

### fixed
```sass
// fixed($offset)
div
  +fixed(right)
```

### absolute
```sass
// absolute($offset)
div
  +absolute(right bottom 2em)
```

### relative
```sass
// relative($offset)
div
  +relative(left 2em right 1em)
```

### static
```sass
// static
div
  +static
```

## Block Tools

### z
Accepts integer or map value to set `z-index`.
```sass
// z($index)
div
  +z(overlay)
  // z-index: 300
  +z(modal)
  // z-index: 200
  +z(fixed)
  // z-index: 100
  +z(50)
  // z-index: 50
```

### hr
Creates a custom `border-bottom`.
```sass
// hr($color, $height, $width)
h1
  +hr
  +hr(orange, 2px, 80%)
```

### scroll
Sets `height` or `width` and applies respective `overflow: scroll`.
```sass
// hide($value, $feature, $display: block)
div
  +scroll                 // `overflow: scroll`
  +scroll(400px)          // `overflow-x: scroll` with height of 400px
  +scroll(desktop, width) // `overflow-y: scroll` with width of 1200px
```
