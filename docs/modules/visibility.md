# Visibility

Hide or unhide an element but make it accessible to screen readers

## Arguments

`$visibility` {string} Required, accets 'visible' or 'hidden'

`$position` {string} Optional, accepts 'absolute', 'relative'...etc, defaults to 'static'

## Usage

```css
@import '~sass-library/mixins/visibility.scss';

.selector {
  @include visibility(hidden);
}
```
