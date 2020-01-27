# Sass Library

Sass library is a toolkit of mixins and resources designed to make styling with SCSS as efficient by flexible as possible.

📒 [Documentation](https://docs.sasslibrary.com/)


-----


## Quick start guide

### 1. Add the library to your project

  ```bash
  $ npm install sass-library
  ```

  Alternatively include the files manually if you aren't using a package manager.

### 2. Import as needed into your Sass project

  ```bash
  @import '~sass-library/mixins/prefix.scss';
  @import '~sass-library/mixins/visibility.scss';
  ```

### 3. Use the imported modules in your Sass

  ```bash
  .some-element {
    @include prefix(display, flex, ms webkit);
  }
  ```
