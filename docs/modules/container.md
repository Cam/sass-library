# Container

Layout container generator

### Dependencies

Globally applied `border-box: box-sizing;`

### Arguments

`$max-width` {string} Grid width variable, accepts various unit types \(px, em, rem...\)

`$gutter` {string} The margins around your element, accepts various unit types \(px, em, rem...\)

### Usage

```css
@import '~sass-library/mixins/container.scss';

.selector {
  @include container($grid-large, 4rem 2rem);
}
```

{% hint style="info" %}
Author: Cam Gould  
Source: [https://github.com/cam/sass-library](https://github.com/cam/sass-library)  
License: Copyright © 2020 Cam Gould. The MIT License \(MIT\)
{% endhint %}

