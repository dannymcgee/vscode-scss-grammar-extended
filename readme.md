# SCSS Grammar Extended

This extension adds some additional features and fixes some bugs in VS Code's default SCSS grammar.

**Features:**
* BEM-style `__element` and `--modifier` fragments tokenized as class names (for use with the ampersand, interpolation, etc.)
* `null` and boolean values tokenized as language constants
* Added recognition for Angular-specific pseudo-selectors `:host-context` and `::ng-deep`

**Fixes:**
* Fixed `content` and `cursor` property names being tokenized as tag selectors
* Fixed `background` being tokenized as an invalid/deprecated keyword in certain contexts
* Fixed `color` being tokenized as a property value keyword instead of a property name in certain contexts

**Known issues:**
* CSS3 variable definitions are now erroneously tokenized as class names/BEM modifiers. This is a relatively minor issue in my opinion, since for most use cases Sass variables are preferred over CSS variables.