## Flexbox
Quickly define `display: flexbox` and set positioning.

#### $flex-positioning

```bash
# aliases for `justify-content`, `align-items`, and `align-content`
flex-start    | start   | top     | left
flex-end      | end     | bottom  | right
space-between | between
space-around  | around
```

### flexbox

```sass
// flexbox($direction, $wrap, $justify-content, $align-items, $align-content)
// default: 'display: flex'
div
  +flexbox(row, wrap, around, center, end)
```

### row
Quickly define `flexbox(row)` and position.

```sass
// row($justify-content, $align-items)
div
  +row(between)

// row-reverse($justify-content, $align-items)
div
  +row-reverse(start)

// row-wrap($justify-content, $align-items, $align-content)
div
  +row-wrap(center, bottom, bottom)

// row-reverse-wrap($justify-content, $align-items, $align-content)
div
  +row-reverse-wrap(start, center)

```

### col
Quickly define `flexbox(column)` and position.

```sass
// col($justify-content, $align-items)
+col(center)

// col-reverse($justify-content, $align-items)
+col-reverse(center)

// col-wrap($justify-content, $align-items, $align-content)
+col-wrap(between, center, start)

// col-reverse-wrap($justify-content, $align-items, $align-content)
+col-reverse-wrap(between, start, end)

```
