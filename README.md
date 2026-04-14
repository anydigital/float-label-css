# 🥷 Classless CSS-only Float Label. Finally.

<!--section:summary-->

Bulletproof classless CSS-only implementation of Float Label pattern with automatic fallback for ANY non-supporting browser.

![](https://img.shields.io/github/v/release/anyblades/float-label-css?label=&color=darkslategray&style=for-the-badge&include_prereleases)
[![](https://img.shields.io/badge/Code-gainsboro?logo=github&logoColor=black&style=for-the-badge)](https://github.com/anyblades/float-label-css)
[![](https://img.shields.io/github/stars/anyblades/float-label-css?label=Star&labelColor=gainsboro&color=silver&style=for-the-badge)](https://github.com/anyblades/float-label-css)

<!--section:gh-only-->

## [Demo & docs ↗](https://blades.ninja/css/float-label/#demo)

[<img src="float-label-css-v2.gif" width="600">](https://blades.ninja/css/float-label/#demo)

<!--section:docs-demo-install-->

Examples:

- [**Pico + *Bl*ades** with Float Label CSS v2 included](https://blades.ninja/css/float-label/#demo)
- [**Tailwind v4** + Float Label CSS v2](https://codepen.io/tonystar/pen/ALaZrV)
- [**Float Label CSS v2 only**](https://codepen.io/tonystar/pen/JRLaKw) (no CSS frameworks)

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

## Install <!-- same as https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md -->

###### <mark>Via CDN</mark>

<!--prettier-ignore-->
```html
<link rel="stylesheet" href="
  https://cdn.jsdelivr.net/npm/@anyblades/blades@^0.28.0-alpha/assets/float-label.min.css
">
```

###### <mark>Via npm</mark>

```sh
npm install @anyblades/blades
```

Then in your `.css`:

```css
@import "@anyblades/float-label";
```

###### <mark>Prepackaged</mark>

- Blades: https://github.com/anyblades/blades
- Pico: https://github.com/anyblades/pico

<!--section:docs-->

---

## Usage

Simply place `<input>` inside `<label>` to enable float label:

```html
<label>
  <span>Email</span>
  <input type="email" placeholder="email@example.com" />
</label>
```

**NOTE:** W3C [allows this](http://www.w3.org/TR/html401/interact/forms.html#edef-LABEL)!

<div><hr></div>

Alternatively wrap `<label>` and `<input>` inside `.has-float-label`:

```html
<div class="has-float-label">
  <label for="email">Email</label>
  <input id="email" type="email" placeholder="email@example.com" />
</div>
```

**NOTE**: `for="..."` attribute is required on `<label>` in this case

---

## Credits

- [Matt D. Smith](https://x.com/mds) for [original pattern](https://dribbble.com/shots/1254439--GIF-Float-Label-Form-Interaction)
- Emil Björklund for [`:placeholder-shown`](https://thatemil.com/blog/2016/01/23/floating-label-no-js-pure-css/)
- [Anton Staroverov](https://x.com/AntonStarovero_) for [`:has(*:placeholder-shown:not(:focus)) label`](https://blades.ninja/css/float-label/#how)
  - to finally support labels before input fields
  - instead of [`input:focus + label`](https://css-tricks.com/float-labels-css/) used previously

---

## Browser support

Any browser with https://caniuse.com/css-placeholder-shown, https://caniuse.com/css-has and https://caniuse.com/css-nesting.

All non-supporting browsers should gracefully fall-back to the default layout.

=> Can be used in ANY browser _as is_!

---

Featured by:

- https://github.com/dbohdan/classless-css
- https://github.com/pryley/float-labels.js
- https://github.com/uptonking/note4yaoo/blob/main/toc/toc-lib-css-only.md#css-tools
- https://github.com/bcgov/moh-fpcare `package.json`

<!--section:gh-only-->

---

## PS: [How it works?](https://blades.ninja/css/float-label/#how)
