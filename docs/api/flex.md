## Flexbox

#### flexbox
Quickly define and position `display: flexbox`
```sass
// flexbox($direction: row, $wrap: wrap, $justify-content: null, $align-items: null, $align-content: null)
// default: 'display: flex'
+flexbox(row, nowrap, around, center)
```

##### Flex Positioning
`justify-content`, `align-items`, and `align-content` values.
```bash
flex-start    | start   | top       | left
flex-end      | end     | bottom    | right
space-between | between
space-around  | around
baseline      | base
````

#### flat
`flexbox(row)`
```sass
// flat($justify-content: null, $align-items: null)
+flat(between)

// flat-reverse($justify-content: null, $align-items: null)
+flat-reverse(start)

// flat-wrap($justify-content: null, $align-items: null, $align-content: null)
+flat-wrap(center, bottom, bottom)

// flat-reverse-wrap($justify-content: null, $align-items: null, $align-content: null)
+flat-reverse-wrap(start, center)

```

#### stack
`flexbox(column)`
```sass
// stack($justify-content: null, $align-items: null)
+stack(center)

// stack-reverse($justify-content: null, $align-items: null)
+stack-reverse(center)

// stack-wrap($justify-content: null, $align-items: null, $align-content: null)
+stack-wrap(between, center, start)

// stack-reverse-wrap($justify-content: null, $align-items: null, $align-content: null)
+stack-reverse-wrap(between, start, end)

```

## Flex

#### flex
defines `flex: $value`
```sass
// flex($value: initial)
// allows use of custom map values or standard flex values
div
  +flex(1 1 200px)

article
  +flex(fill)

section
  +flex(auto)
```

##### Flex Aliases
```bash
fill:   1
shrink: 0
```
