## Element
These mixins take html `<elements>` or `".classes"` as arguments and apply styling to that child.

### fix
fixes an element to the specific location and offsets `:root`
```sass
// fix($element, $location: top, $size: 3em)
+fix(header, top)
