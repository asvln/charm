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

## Block Tools

#### z-index
accepts integer or map value to set `z-index`
```sass
// z-index($index)
// default map values based on an 8 floor hotel
div
  +z-index(roof)
  +z-index(90)
  +z-index(lobby)
  +z-index(basement)
```

#### underline
creates a custom `border-bottom`
```sass
// underline($color: black, $height: 1px, $width: 100%)
h1, h2
  +underline(orange)
```
