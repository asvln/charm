## Block
`$top` has single value aliases to place element:
```sass
$top: top | right | bottom | left | fill
```

### block
define and position `display: block`
```sass
// block($position, $top, $right, $bottom, $left)
// default: 'display: block'
div
  +block(sticky, top)
```

### inline-block
define and position `display: inline-block`
```sass
// inline-block($position, $top, $right, $bottom, $left)
// default: 'display: inline-block'
div
  +inline-block(relative, 5px, 5px)
```

### inline
define and position `display: inline`
```sass
// inline($position, $top, $right, $bottom, $left)
// default: 'display: inline-block'
div
  +inline
```

## Block Positions

### sticky
define and position a block with `display: sticky`
```sass
// sticky($top, $right, $bottom, $left)
div
  +sticky(bottom)
```

### fixed
define and position a block with `display: fixed`
```sass
// fixed($top, $right, $bottom, $left)
div
  +fixed(right)
```

### absolute
define and position a block with `display: absolute`
```sass
// absolute($top, $right, $bottom, $left)
div
  +absolute(null, 0, 0)
```

### relative
define and position a block with `display: relative`
```sass
// relative($top, $right, $bottom, $left)
div
  +relative(1em)
```

## Block Tools

### z
accepts integer or map value to set `z-index`
```sass
// z($index)
// default map values based on an 8 floor hotel
div
  +z(roof)
  +z(90)
  +z(lobby)
  +z(basement)
```

### hr
creates a custom `border-bottom`
```sass
// hr($color, $height, $width)
h1, h2
  +hr(orange)
```
