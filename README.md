# Captain’s log

[live demo](http://mashlo.github.io/captains-log/)

Captain’s log is a minimalistic & responsive theme for [Jekyll](https://jekyllrb.com/). It has several color scheme options and is em/rem based, so it's ~~should be~~ easy to customize it to your own taste!

![screenshot](https://raw.githubusercontent.com/mashlo/captains-log/gh-pages/assets/preview.png)

This theme is made by [Masha Safina](http://masha.space) for blogging porpoises.

## Get Started
Fork repository first 👆 Instal jekyll, clone repo & start jekyll server.

```
$ gem install jekyll
$ git clone git@github.com:mashlo/captains-log.git
$ cd captains-log
```

## Update `_config.yml`

Don't forget to update `_config.yml` file located in the root of the theme (to not have my email and twitter linked)

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

### Run Jekyll

```
$ jekyll serve --watch
```

View your site localy at `localhost:4000` ✨  

## Style Customization

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

To customize it further tweak the following vars in `_sass\themes\_default.scss` (or create a separate file).

```
$font-size-base:   18px;     // base body font size, the rest are REM based
$line-height-base: 1.5;      // base line height
$font-size-mobile: 14px;     // font size after break point 

$text-color:       #fff;                     // main copy color
$text-color-light: rgba($text-color, 0.4);   // dates & footer copy
$title-color:      #0dccd1;                  // post title color on post page

$background-color: #3b3056;   // main background color

$brand-color-base: #f76067;   // main accent color
$brand-color-sub:  #0dccd1;   // secondary accent color
```

Ta-da! 🎉

