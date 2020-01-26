# Getting started

### 1. Add the library to your project

```css
$ npm install sass-library
```

Alternatively include the files manually if you aren't using a package manager.

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

