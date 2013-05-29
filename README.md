logos-in-pure-css
=================

![Logos In Pure CSS](https://raw.github.com/bchanx/logos-in-pure-css/master/banner.png)

Company logos created in pure CSS, built in [less](http://www.lesscss.org).  
**See it in action here:** [bchanx.com/logos-in-pure-css-demo](http://www.bchanx.com/logos-in-pure-css-demo)

Usage
-----

The easiest way to use these icons is to import the corresponding .less file in your own .less styling sheet:

```html
@import "relative/path/to/logos-in-pure-css/twitter.less";
```

You can also link the stylesheet via .html (but you'll need a copy of [less.js](https://github.com/cloudhead/less.js/tree/master/dist), tested on > v1.3.3):

```html
<link type="text/less" rel="stylesheet" href="/path/to/logos-in-pure-css/twitter.less">
<script type="text/javascript" src="/path/to/less.js"></script>
```

If you prefer not to use less, you can use the .css file provided:

```html
<link type="text/css" rel="stylesheet" href="/path/to/logos-in-pure-css/twitter.css">
```

Once imported, copy the accompanying logo .html into your own .html file and the icon should display!

```html
<div class="logo-twitter-{{ size }}">                                      
  <div class="body"></div>
  <div class="body-none"></div>
  <div class="beak-bottom"></div>
  <div class="beak-bottom-none"></div>
  <div class="wing-bottom"></div>
  <div class="wing-bottom-none"></div>
  <div class="wing-middle"></div>
  <div class="wing-middle-none"></div>
  <div class="wing-top"></div>
  <div class="wing-top-none"></div>
  <div class="beak-top"></div>
  <div class="beak-top-none"></div>
  <div class="head"></div>
</div>
```

Sizes
-------

By default, `{{ size }}` supports two different keywords: large and small. This in turn produces a 300x300px or 52x52px icon.  
If you're using less, you can modify the sizes by either changing the `@radius` param, or by defining your own class
and calling the logo mixin() with your desired `@radius` size.

Currently, the .css file only supports large and small icon sizes.

License
-------
This software is free to use under the MIT license.

