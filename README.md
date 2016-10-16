Pure-CSS Float Label. Finally.
==============================

[![npm version](https://img.shields.io/npm/v/float-label-css.svg)](https://www.npmjs.com/package/float-label-css)
[![Twitter URL](https://img.shields.io/twitter/url/http/shields.io.svg?style=flat&label=retweet)](https://twitter.com/tonystarring/status/787217405827317762)

Bulletproof CSS-only implementation of Float Label pattern with automatic fallback for ANY non-supporting browser.

* No JS!
* No hacks with `required` and `:valid`!
* => HTML5 validation support
* => `<select>` fields support

<img src="https://cdn.rawgit.com/tonystar/float-label-css/9dd8582/float-label-css.gif" width="400"/>


## Demo

No-dependencies demo: https://codepen.io/tonystar/pen/JRLaKw.

Bootstrap 3 demo: https://codepen.io/tonystar/pen/ALaZrV.

Bootstrap 4 demo: https://codepen.io/tonystar/pen/LRdpYZ.


## Usage

Include `float-label.min.css`:
```html
<link rel="stylesheet" href="https://cdn.rawgit.com/tonystar/float-label-css/v1.0.0/dist/float-label.min.css"/>
```

Wrap `input` and `label` by `.has-float-label`:
```html
<span class="has-float-label">
  <input class="form-control" id="email" type="email" placeholder="box@example.com"/>
  <label for="email">Email</label>
</span>
```

**NOTE:** `label` should go after `input`! This is the only drawback in this method.


### Quick use: Bootstrap

Instead of `float-label.min.css` just include pre-built `bootstrap-float-label.min.css`:
```html
<!-- Bootstrap v4 -->
<link rel="stylesheet" href="https://cdn.rawgit.com/tonystar/bootstrap-float-label/v4.0.0/dist/bootstrap-float-label.min.css"/>

<!-- Bootstrap v3 -->
<link rel="stylesheet" href="https://cdn.rawgit.com/tonystar/bootstrap-float-label/v3.0.0/dist/bootstrap-float-label.min.css"/>
```

Markup is the same. For more details see: https://github.com/tonystar/bootstrap-float-label.


## Credits

* [@mds](https://twitter.com/mds) for the [original pattern](http://mds.is/float-label-pattern/)
* [@chriscoyier](https://twitter.com/chriscoyier) for the [`input:focus + label`](https://css-tricks.com/float-labels-css/)
* [@thatemil](https://twitter.com/thatemil) for the [`:placeholder-shown`](https://thatemil.com/blog/2016/01/23/floating-label-no-js-pure-css/)


## Browser support

Any browser with `:placeholder-shown` CSS pseudo-class: http://caniuse.com/#feat=css-placeholder-shown.

All non-supporting browsers will fall back to the static layout (w/o animation).

=> Can be used in ANY browser *as is*!
