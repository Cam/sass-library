# Examples

### Simple responsive layout

Using a combination of mixins, we can create custom responsive layouts with ease.

{% code title="index.html" %}
```markup
<div class="container">
  <div class="show-medium-up">
    Grid-like element
  </div>
  
  <div class="hide-medium">
    Grid-like element
  </div>
  
  <div class="show-medium-down">
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
  
  .show-medium-up {
    @include media-query($small-screens) {
      display: none;
    }
  }

  .hide-medium {
    @include media-query($medium-screens) {
      display: none;
    }
  }

  .show-medium-down {
    @include media-query($large-screens) {
      display: none;
    }
  }
}
```
{% endcode %}

