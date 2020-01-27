# Prefixer

Generates vendor prefixes for any CSS property

## Arguments

`$property` {string} Property to prefix

`$value` {string} Value to use

`$prefixes` {list} Vendor prefixes to output \(moz, webkit, o, ms...\)

Usage:

```css
@import '~sass-library/mixins/prefix.scss';

.element {
   @include prefix(appearance, none, webkit moz));
 }
```

{% hint style="info" %}
Author: Hugo Giraudel
Source: [https://github.com/thoughtbot/bourbon](https://github.com/thoughtbot/bourbon)
License: Bourbon is copyright © 2011-2019 thoughtbot, inc. It is free software, and may be redistributed under the terms specified in the license.
{% endhint %}
