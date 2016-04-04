# Captain’s log

[live demo](http://dsdsd)

Captain’s log is a minimalistic & responsive theme for Jekyll. It has several color scheme options, but it's _should be_ easy to create your own!

![screenshot]()

This theme is made by [Masha Safina](http://masha.space)

## Customization

The `_default.scss` located in the `_sass\themes` directory contains default variables for the base b/w color scheme. 

```
_sass
  |-- themes
    |-- _default.scss
    |-- _data-dreams.scss
    |-- _sweet-like-will.scss

css
  |-- main.scss

```

and imported as a partial in `main.scss` before everything else.

```
// theme variables go first
@import 'themes/default';

@import 'reset';
@import 'base';
...
```

To use one of the preset color schemes simply replace `_default.scss` partial with desired from `_sass\themes` directory:

```

// theme variables go first
@import 'themes/sweet-like-will';

@import 'reset';
@import 'base';
...

```

Ta-da! 🎉

