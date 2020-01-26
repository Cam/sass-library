# Examples

### Simple responsive layout

```markup
<div class="container">
  <div class="column1">
    This content is in a responsive element using the container mixin.
  </div>
  
  <div class="column2">
    This content is in a responsive element using the container mixin.
  </div>
  
  <div class="column3">
    This content is in a responsive element using the container mixin.
  </div>
</div>
```

```css
$small-screens: (
  max: 70em
);

$medium-screens: (
  min: 70.1em,
  max: 90em
);

$large-screens: (
  min: 90.1em
);

.container {
  @include container(50em, 20px);
  @include prefix(display, flex, webkit ms);
  
  .column-1 {
    @include media-query($small-screens) {
      display: none;
    }
  }

  .column-2 {
    @include media-query($medium-screens) {
      display: none;
    }
  }

  .column-3 {
    @include media-query($large-screens) {
      display: none;
    }
  }
}
```

