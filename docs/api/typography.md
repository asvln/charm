## Document Typography
Document typography can be placed in the root of your stylesheet to quickly define a typographic layout

### set-heading-ratio
sets the heading `font-size` ratio
```sass
// set-heading-ratio($ratio)
// default: html5
+set-heading-ratio(minor3)
```

### set-line-heights
sets the `line-height` for text selector groups
```sass
// set-line-heights($heading, $text, $input, $button)
// default: (1.5, $heading, 1.15, 1.15)
// map: $line-heights
+set-line-heights(golden, 1.5)
```

### set-font-weights
sets the `font-weight` for text selector groups
```sass
// set-font-weights($heading, $text, $input, $button)
// default: (bold, regular, $text, $input)
// map: $font-weights
+set-font-weights(semi-bold, normal)
```

### font-response
scales `:root` font-size based on `viewport-width` using `calc()`
```sass
// font-response($start: 48rem, $end: 120em)
// ratio: 1em -> 2em
// default range: 768px -> 1920px
+font-response
```

### font-face
quickly import a font
```sass
// font-face($family, $weight, $url, $style)
// default style: normal
+font-face(Raleway, 400, "fonts/Raleway-Regular.ttf")
+font-face(Raleway, bold, "fonts/Raleway-BoldItalic.ttf")
```

## Block Typography
Block typography is applied directly to a `<block>` element

### line-height
sets the `line-height` allowing custom map values
```sass
// line-height($height)
// map: $line-heights
h1
  +line-height(1.55)
  +line-height(golden)
```

### font-weight
sets the `font-weight` allowing custom map values
```sass
// font-weight($weight)
// map: $font-weights
p
  +font-weight(thin)
```

### font-family
quickly assign backup fonts
```sass
// font-family($family: null, $backup-type: null)
// default: sans-serif
body
  +font-family(Raleway)
  +font-family(Fira Code, mono)
```

## Type Tools
### reverse-indent
utilizes `text-indent` and `margin`
```sass
// reverse-indent($amount)
p
  +reverse-indent(1em)
