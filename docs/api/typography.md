## Document Typography

Document typography can be placed in the root of your stylesheet to quickly define a typographic layout

#### set-heading-ratio
sets the heading `font-size` ratio
```sass
// set-heading-ratio($ratio: html5)
// default: html5
+set-heading-ratio(minor3)
```

#### set-line-heights
sets the `line-height` for text selector groups
```sass
// set-line-heights($heading: 1.5, $text: $heading, $input: 1.15, $button: 1.15)
//(heading, texts, inputs, buttons)
// default: (1.5, 1.5, 1.15)
+set-line-heights(1.62, 1.5)
```

#### set-font-weights
sets the `font-weight` for text selector groups
```sass
// set-font-weights($heading: regular, $text: $heading, $input: $text, $button: $input)
// (heading, texts, inputs, buttons)
// default: regular
+set-font-weights(semi-bold, normal)
```

#### font-response
scales `:root` font-size based on `viewport-width`
```sass
// font-response($start: 48rem, $end: 120em)
// ratio: 1em -> 2em
// default range: 768px -> 1920px
+font-response
```

#### font-face
quickly import a font
```sass
// font-face($family, $weight, $url, $style: normal)
// default style: normal
+font-face(Raleway, 400, "fonts/Raleway-Regular.ttf")
```


## Block Typography
Block typography is applied directly to a `<block>` element

#### line-height
sets the `line-height` allowing custom map values
```sass
// line-height($height)
// reads custom values from 'core/maps'
h1
  +line-height(1.55)
  +line-height(golden)
```

#### font-weight
sets the `font-weight` allowing custom map values
```sass
// font-weight($weight)
// sets the font weight using conventional font weight names
// reads custom values from 'core/maps'
p
  +font-weight(thin)
```

#### font-family
quickly assign backup fonts
```sass
// font-family($family: null, $type: null)
// default: sans-serif
body
  +font-family(Raleway)
```

### Type Tools
#### reverse-indent
utilizes `text-indent` and `margin`
```sass
// reverse-indent($amount: .62em)
p
  +reverse-indent(1em)
