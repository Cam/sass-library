# Media Query

Generates media queries

## Arguments

`$media` - Optional {string}, media type to target. Defaults to `screen`

`$min` - Optional {string}, minimum media width to target. Accepts various unit types (px, em, rem...)

`$max` - Optional {string}, max media width to target. Accepts various unit types (px, em, rem...)

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
