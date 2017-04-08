# ninja syntax

Synxtax highlighting for [ninja](https://github.com/ninja-build/ninja) build files adapted from [SublimeNinja](https://github.com/pope/SublimeNinja).

## Features

Direct port of [SublimeNinja](https://github.com/pope/SublimeNinja), with minor fixes.


## Release Notes

### 1.0.0

* Tweak regex to not match comments following declarations.

  Even though the ninja manual does not explicitly state this,
  * Comments cannot follow variable declarations (since the `#` will simply be part of the string)
  * Comments cannot follow rule declarations (parser errors occur)

  Change regex so these are not mistakenly highlighted as comments.

* Configure line comment symbol (`#`) so `editor.action.commentLine` etc. will work properly.
