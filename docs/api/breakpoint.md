## Breakpoints

#### breakpoint
a verbose `@media` min or max declaration
```sass
// breakpoint($width, $limit)
// accepts map key for
nav
  +breakpoint(small, min)
    display: none

div
  +breakpoint(400px, max)
    font-size: .9em
```

#### at
`min-width` breakpoint
```sass
// at($width)
article
  +at(small)
    font-size: 1.1em
```

#### to
`max-width` breakpoint
```sass
// to($width)
section
  +to(600px)
    font-size: .9em
```

#### hide
hide with `display: none` and optionally define shown `display` type
```sass
// hide-at($width, $display: block)
// `min-width` breakpoint
div
  +hide-at(300px)

// hide-to($width, $display: block)
// `max-width` breakpoint
div
  +hide-to(phone, flex)
```

#### show
reverse of `hide()`
```sass
// show-at($width, $display: block)
// `min-width` breakpoint
div
  +show-at(large, inline-block)

// show-to($width, $display: block)
// `max-width` breakpoint
div
  +show-to(desktop)

```

#### scroll-at
sets `height` of element and applies `overflow: scroll`
```sass
// scroll-at($height: null)
//
+scroll-at(400px)
```

## Device Orientation
#### landscape
```sass
// landscape styling
main
  +landscape
    margin-left: auto
```

#### portrait
```sass
// portrait styling
div
  +portrait
    margin: 1em
```
