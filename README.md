# Captain’s log

[live demo](http://mashlo.github.io/captains-log/)

Captain’s log is a minimalistic & responsive theme for Jekyll. It has several color scheme options, but it's ~~should be~~ easy to create your own!

![screenshot](https://raw.githubusercontent.com/mashlo/captains-log/gh-pages/assets/preview.png)

This theme is made by [Masha Safina](http://masha.space)

## Update `_config.yml`

Don't forget to update `_config.yml` file located in the root of the theme

```
# Site settings
title:       Captains-log
author:      Masha Safina
description: ":rocket: A responsive Jekyll theme based on my personal internet site"
baseurl:     "" 
url:         "https://your.site" 

# Social Links
email:            your_email@example.com
twitter_username: username
github_username:  username

# Build settings
markdown: kramdown
permalink: pretty

```

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

and is imported as partial in `main.scss` before everything else.

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

