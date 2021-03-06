# markdown-it-kbd [![Build Status](https://travis-ci.org/jGleitz/markdown-it-prism.svg?branch=master)](https://travis-ci.org/jGleitz/markdown-it-kbd) [![Dependency Status](https://gemnasium.com/badges/github.com/jGleitz/markdown-it-kbd.svg)](https://gemnasium.com/github.com/jGleitz/markdown-it-kbd) [![npm version](https://badge.fury.io/js/markdown-it-kbd.svg)](https://badge.fury.io/js/markdown-it-kbd) [![Bower version](https://badge.fury.io/bo/markdown-it-kbd.svg)](https://badge.fury.io/bo/markdown-it-kbd)
> [markdown-it](https://github.com/markdown-it/markdown-it) plugin for keystrokes

Renders `[[x]]` as `<kbd>x</kbd>`. ([`<kbd>`](http://www.w3schools.com/tags/tag_kbd.asp) is the tag for keystrokes).

## Usage
```js
const md = require('markdown-it')();
const kbd = require('markdown-it-kbd');

md.use(kbd);
```

This plugin can also be used together with [`markdown-it-attrs`](https://github.com/arve0/markdown-it-attrs/).

## Parsing note

The end tag `]]` must be on the same line as the start tag `[[`.

At the moment, “`[[`” and “`]]`” are not allowed within keystroke tags, because I can't think of a way to handle this that would make sense in all scenarios. If you think you know how it should be done, please file an issue!
