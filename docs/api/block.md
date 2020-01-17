## Block

#### block
define and position `display: block`
```sass
// block($position: null, $top: null, $right: null, $bottom: null, $left: null)
// $top single value aliases: (top, right, bottom, left)
// default: 'display: block'
div
  +block(sticky, top)
```

#### inline-block
define and position `display: inline-block`
```sass
// inline-block($position: null, $top: null, $right: null, $bottom: null, $left: null)
// $top single value aliases: (top, right, bottom, left)
// default: 'display: inline-block'
div
  +inline-block(relative)
```

#### inline
define and position `display: inline`
```sass
// inline($position: null, $top: null, $right: null, $bottom: null, $left: null)
// $top single value aliases: (top, right, bottom, left)
// default: 'display: inline-block'
div
  +inline(relative)
```

### Block Positions

#### relative
define and position a block with `display: relative`
```sass
// relative($top: null, $right: null, $bottom: null, $left: null)
div
  +relative(1em)
```

#### absolute
define and position a block with `display: absolute`
```sass
// absolute($top: null, $right: null, $bottom: null, $left: null)
div
  +absolute(null, 10px)
```

#### fixed
define and position a block with `display: fixed`
```sass
// fixed($top: null, $right: null, $bottom: null, $left: null)
div
  +fixed
```

### Block Tools
#### z
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

#### underline
creates a custom `border-bottom`
```sass
// underline($color: black, $height: 1px, $width: 100%)
h1, h2
  +underline(orange)
```
