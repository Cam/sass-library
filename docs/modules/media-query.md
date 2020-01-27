# Media Query

Generates media queries

## Arguments

`$media` {string} Optional media type to target, defaults to `screen`

`$min` {string} Optional minimum media width to target, accepts various unit types (px, em, rem...)

`$max` {string} Optional max media width to target, accepts various unit types (px, em, rem...)

## Usage

```css
@import '~sass-library/mixins/media-query.scss';

$medium-screens: (
  media: screen,
  min: 701px,
  max: 1000px
);

.selector {
  @include media-query($medium-screens) {
    display: none;
  }
}
```

-----

Author: Cam Gould
