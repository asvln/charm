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

### flat
Quickly define `flexbox(row)` and position.

```sass
// flat($justify-content, $align-items)
div
  +flat(between)

// flat-reverse($justify-content, $align-items)
div
  +flat-reverse(start)

// flat-wrap($justify-content, $align-items, $align-content)
div
  +flat-wrap(center, bottom, bottom)

// flat-reverse-wrap($justify-content, $align-items, $align-content)
div
  +flat-reverse-wrap(start, center)
```

### stack
Quickly define `flexbox(column)` and position.

```sass
// stack($justify-content, $align-items)
div
  +stack(center)

// stack-reverse($justify-content, $align-items)
div
  +stack-reverse(center)

// stack-wrap($justify-content, $align-items, $align-content)
div
  +stack-wrap(between, center, start)

// stack-reverse-wrap($justify-content, $align-items, $align-content)
div
  +stack-reverse-wrap(between, start, end)
```
