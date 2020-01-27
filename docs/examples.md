# Examples

### Simple responsive layout

Using a combination of mixins, we can create custom responsive layouts with ease.

{% code title="index.html" %}
```markup
<div class="container">
  <div class="column1">
    Grid-like element
  </div>
  
  <div class="column2">
    Grid-like element
  </div>
  
  <div class="column3">
    Grid-like element
  </div>
</div>
```
{% endcode %}

{% code title="variables.scss" %}
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
```
{% endcode %}

{% code title="app.scss" %}
```css
@import 'variables.scss';

.container {
  @include container(70em, 20px);
  @include prefix(display, flex, webkit ms);
  
  > div {
    @include prefix(flex, 1, webkit ms);
  }
  
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
{% endcode %}

