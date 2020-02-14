# charm
<img align="right" height="100" src="docs/images/charm.svg">

**charm** is an atomic Sass framework with:

- Simple [typographic](docs/api/typography.md) layouts
- Single-line [flexbox](docs/api/flex.md) and [block](docs/api/block.md) declarations
- Intuitive [media queries](docs/api/media.md)
- Extensible [default styling](https://charmingsass.com/defaults.html)
- [Resets](https://github.com/asvln/fern) that standardize results across browsers

## Sample Usage
```sass
@import charm/charm

+set-heading-ratio(minor3)
+set-line-heights(1.55em)
+set-font-weights(semi-bold, thin)

body
  font-size: 1em
  +font-family(Raleway)

+headings
  margin: 1rem
  +hr

section
  +col(between)
  +media(min, small)
    +row-wrap(around, center)

article
  +scroll(5em)
```

## Installation
1. [`Download`](https://github.com/asvln/charm/releases/latest/) or clone to your project's SASS folder

```bash
git clone https://github.com/asvln/charm
```

2. Import `charm/charm` into your main SASS/SCSS file

```sass
@import charm/charm
```

3. **charm** is now accessible

```sass
+set-heading-ratio(golden)
```

## Documentation
Documentation can be found in [`charm/docs`](docs/index.md).

## Release Cycle
API is currently being developed and there may be breaking changes. It is currently considered beta for requests, commentary, and contributions.

## Sponsor
[Sponsors](https://patreon.com/charmingsass) help support the creation of new features such as...

- Animations
- Color scheming
- Grid Implementation
- Specialized components

## License
This project is licensed under the MIT License
