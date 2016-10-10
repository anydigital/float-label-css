Float Label CSS-only
====================

Bulletproof CSS-only implementation of Float Label pattern with automatic fallback for ANY non-supporting browser.

<img src="https://cdn.rawgit.com/tonystar/float-label-css/master/float-label-css.gif" width="460"/>


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

**NOTE:** `label` should go after `input`! This is the only drawback of this method.


## Browser support

Any browser with `:placeholder-shown` CSS pseudo-class: http://caniuse.com/#feat=css-placeholder-shown.

All non-supporting browsers will fall back to the static layout (w/o animation).

=> Can be used in ANY browser *as is*!
