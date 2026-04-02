# 🥷 Pure-CSS Float Label. Finally. <sup>![](https://img.shields.io/github/v/release/anydigital/float-label-css?label=&color=black&include_prereleases)</sup>

[![](https://img.shields.io/badge/Demo_&_Docs-darkslategray?style=for-the-badge)](https://blades.ninja/css/float-label/)
[![](https://img.shields.io/github/stars/anydigital/float-label-css?label=Star&labelColor=gainsboro&color=silver&style=for-the-badge)](https://github.com/anydigital/float-label-css)

<!--section:summary-->

Bulletproof CSS-only implementation of Float Label pattern with automatic fallback for ANY non-supporting browser.

<!--section:gh-only-->

<img src="https://cdn.rawgit.com/tonystar/float-label-css/9dd8582/float-label-css.gif" width="400"/>

## Demo

<!--section:docs-->

- [Float Label CSS **only**](https://codepen.io/tonystar/pen/JRLaKw) (without any framework)
- [**Pico** + Float Label via Blades CSS](https://blades.ninja/css/float-label/#demo)
- [**Bootstrap v4** + Float Label CSS](https://codepen.io/tonystar/pen/LRdpYZ)
<!-- - [Tailwind v4 + Float Label CSS](https://codepen.io/tonystar/pen/ALaZrV) -->

---

## Killer features

- No JS — pure CSS
- No hacks with `required` and `:valid`  
  ↳ HTML5 validation support
- Compatible with `<select>` and `<textarea>` fields
- No need to define `for="..."` attribute on `<label>`
- <mark>NEW</mark> in **v2:** Finally, the text label can be placed BEFORE the input field!
- <mark>NEW</mark> in **v2:** Class-less!

---

## Install

<mark>Via CDN:</mark>

Just **Float Label CSS**:

<!--prettier-ignore-->
```html
<link href="https://cdn.jsdelivr.net/npm/@anydigital/blades@^0.27.0-beta/assets/float-label.min.css" rel="stylesheet" />
```

Or with all [CSS Blades](https://blades.ninja/css/) included:

<!--prettier-ignore-->
```html
<link href="https://cdn.jsdelivr.net/npm/@anydigital/blades@^0.27.0-beta/assets/blades.min.css" rel="stylesheet" />
```

<mark>Via npm:</mark>

```sh
npm install @anydigital/blades
```

Then import just **Float Label CSS**:

```css
@import "@anydigital/float-label";
```

Or with all [CSS Blades](https://blades.ninja/css/) included:

```css
@import "@anydigital/blades";
```

---

## Usage

Simply place `<input>` inside `<label>` to enable float label:

```html
<label>
  <span>Email</span>
  <input type="email" placeholder="email@example.com" />
</label>
```

> **NOTE:** W3C [allows this](http://www.w3.org/TR/html401/interact/forms.html#edef-LABEL)!

<div><hr></div>

Alternatively wrap `<label>` and `<input>` inside `.has-float-label`:

```html
<div class="has-float-label">
  <label for="email">Email</label>
  <input id="email" type="email" placeholder="email@example.com" />
</div>
```

> **NOTE**: `for="..."` attribute is required on `<label>` in this case

---

## Credits

- Matt D. Smith for [original pattern](https://dribbble.com/shots/1254439--GIF-Float-Label-Form-Interaction)
- Emil Björklund for [`:placeholder-shown`](https://thatemil.com/blog/2016/01/23/floating-label-no-js-pure-css/)
- [Anton Staroverov](https://x.com/AntonStarovero_) for `:has(*:placeholder-shown:not(:focus)) label`
  - to finally support labels before input fields
  - instead of [`input:focus + label`](https://css-tricks.com/float-labels-css/) used previously

---

## Browser support

Any browser with https://caniuse.com/css-placeholder-shown, https://caniuse.com/css-has and https://caniuse.com/css-nesting.

All non-supporting browsers should gracefully fall-back to the default layout.

=> Can be used in ANY browser _as is_!

---

Featured by:

- https://github.com/pryley/float-labels.js
- https://github.com/uptonking/note4yaoo/blob/main/toc/toc-lib-css-only.md#css-tools
- https://github.com/bcgov/moh-fpcare `package.json`
