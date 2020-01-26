# Getting started

### 1. Add the library to your project

{% tabs %}
{% tab title="NPM" %}
```text
$ npm install sass-library
```
{% endtab %}

{% tab title="Manual" %}
Manually download and add the modules you require to your project.
{% endtab %}
{% endtabs %}

### 2. Import as needed into your Sass project

```css
@import '~sass-library/mixins/prefix.scss';
@import '~sass-library/mixins/visibility.scss';
```

### 3. Use the imported modules in your Sass

```css
.some-element {
  @include prefix(display, flex, ms webkit);
}
```

