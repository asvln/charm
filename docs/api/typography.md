## Document Typography
Document typography can be placed in the root of your stylesheet to quickly define a typographic layout

#### $heading-ratios
```bash
# defines the `font-size` for h1-h6.

# html defaults
html5
html4
# linear
linear-small
linear
linear-medium
linear-large
# pentatonic
minor2
major2
minor3
major3
perfect4
aug4
dim5
perfect5
dim6
# golden ratio
golden
golden-large
```
### set-heading-ratio
Sets the heading `font-size` ratio.
```sass
// set-heading-ratio($ratio)
// default: html5
+set-heading-ratio(minor3)
```

### set-line-heights
Sets the `line-height` for text selector groups.
```sass
// set-line-heights($heading, $text, $input, $button)
// default: (1.5, $heading, 1.15, 1.15)
// map: $line-heights
+set-line-heights(golden, 1.5)
```

### set-font-weights
Sets the `font-weight` for text selector groups.
```sass
// set-font-weights($heading, $text, $input, $button)
// default: (bold, regular, $text, $input)
// map: $font-weights
+set-font-weights(semi-bold, normal)
```

### apply-font-response
Scales `:root` font-size based on `viewport-width` using `calc()`.
```sass
// apply-font-response($start: 48rem, $end: 120em)
// ratio: 1em -> 2em
// default range: 768px -> 1920px
+apply-font-response
```

### font-face
Quickly import a font.
```sass
// font-face($family, $weight, $url, $style)
// default style: normal
+font-face(Raleway, 400, "fonts/Raleway-Regular.ttf")
+font-face(Raleway, bold, "fonts/Raleway-BoldItalic.ttf")
```

## Block Typography
Block typography is applied directly to any block `<element>`.

### line-height
Sets the `line-height` allowing custom map values.
```sass
// line-height($height)
// map: $line-heights
h1
  +line-height(1.55)
  +line-height(golden)
```

### font-weight
Sets the `font-weight` allowing custom map values.
```sass
// font-weight($weight)
// map: $font-weights
p
  +font-weight(thin)
```

### font-family
Quickly assign backup fonts.
```sass
// font-family($family: null, $backup-type: null)
// default: sans-serif
body
  +font-family(Raleway)
  +font-family(Fira Code, mono)
```

## Type Tools

### reverse-indent
Utilizes `text-indent` and `margin`.
```sass
// reverse-indent($amount)
p
  +reverse-indent(1em)
