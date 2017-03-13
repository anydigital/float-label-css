Pure-CSS Float Label. Finally.
==============================

[![CDNJS](https://img.shields.io/cdnjs/v/float-label-css.svg)](https://cdnjs.com/libraries/float-label-css)
[![npm version](https://img.shields.io/npm/v/float-label-css.svg)](https://www.npmjs.com/package/float-label-css)
[![retweet](https://img.shields.io/badge/re-tweet-00bfff.svg)](https://twitter.com/tonystarring/status/787217405827317762)
[![dribbble](https://img.shields.io/badge/dribbble-%E2%99%A5-ff1493.svg)](https://dribbble.com/shots/3018466-Float-Label-CSS-only)
[![codepen](https://img.shields.io/badge/code-pen-d3d3d3.svg)](https://codepen.io/tonystar/pen/JRLaKw)

> Now hosted on [CDNJS](https://cdnjs.com/libraries/float-label-css)! • And shipped with [Bootstrap Kit](https://bootstrap-kit.com/)!

Bulletproof CSS-only implementation of Float Label pattern with automatic fallback for ANY non-supporting browser.

* No JS! Pure CSS!
* No hacks with `required` and `:valid`!
* ↳ HTML5 validation support!
* Compatible with `<select>` and `<textarea>` fields!
* No need to define `for="..."` attribute on `<label>`! <sup>**v1.0.1+**</sup>

<img src="https://cdn.rawgit.com/tonystar/float-label-css/9dd8582/float-label-css.gif" width="400"/>


## Demo

* [No-dependencies demo](https://codepen.io/tonystar/pen/JRLaKw)
* [Bootstrap 3 demo](https://codepen.io/tonystar/pen/ALaZrV)
* [Bootstrap 4 demo](https://codepen.io/tonystar/pen/LRdpYZ)


## Usage

Include `float-label.min.css`:
```html
<link rel="stylesheet" href="https://cdn.rawgit.com/tonystar/float-label-css/v1.0.2/dist/float-label.min.css"/>
```

Use `<label>` with `.has-float-label` class as a wrapper for `<input>` <sup>**v1.0.1+**</sup>:
```html
<label class="has-float-label">
  <input type="email" placeholder="email@example.com"/>
  <span>Email</span>
</label>
```
**NOTE**:

1. W3C [allows this](http://www.w3.org/TR/html401/interact/forms.html#edef-LABEL).
2. `<span>` should go after `<input>`.

***

Alternatively wrap `<input>` and `<label>` by `.has-float-label`:
```html
<div class="has-float-label">
  <input id="email" type="email" placeholder="email@example.com"/>
  <label for="email">Email</label>
</div>
```
**NOTE**:

1. W3C [allows this](http://www.w3.org/TR/html401/interact/forms.html#edef-LABEL) as well.
2. `<label>` should go after `<input>`.
3. `for="..."` attribute is required on `<label>`.


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
