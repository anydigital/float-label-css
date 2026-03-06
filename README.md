---
permalink: /
---

# 🥷 *Blade*switch

![](https://img.shields.io/github/v/release/anydigital/bladeswitch?color=black&label=%20)
![](https://img.shields.io/github/deployments/anydigital/bladeswitch/github-pages?logo=jekyll&label= "Bladeswitch using Jekyll on GitHub Pages")
![](https://img.shields.io/netlify/ec716489-5d5d-43cb-9fa1-892f8479436e?logo=eleventy&label= "Bladeswitch using 11ty on Netlify")
[![](https://img.shields.io/github/stars/anydigital/bladeswitch?label=GitHub)](https://github.com/anydigital/bladeswitch)

<big>Ultra-lightweight starter compatible with _BOTH_ Jekyll ⇋ and ⇋ Build Awesome (11ty) at the same time.</big>

## Killer _switch_ features

Easy to start, easy to switch:

It allows you to develop locally without [Ruby friction](https://any.digital/tricks/ruby/) (thanks to 11ty), and deploy natively to GitHub Pages using built-in Jekyll engine — no GitHub Actions required!

Now, also includes [Sveltia CMS](https://github.com/sveltia/sveltia-cms). All of this — with only <big>3</big> direct dependencies:

## Light dependencies

<table class="borderless">
  <tr>
    <th>
      🥷 × <big>Jekyll</big>&nbsp;
      <sup><a href="https://anydigital.github.io/bladeswitch/" target="_blank">PREVIEW</a></sup>
    </th>
    <th>
      🥷 × <big>Build Awesome / 11ty</big>&nbsp;
      <sup><a href="https://bladeswitch.netlify.app/" target="_blank">PREVIEW</a></sup>
    </th>
  </tr>
  <tr>
    <td>
      <pre><h3>1. <a href="https://github.com/github/pages-gem" target="_blank">pages-gem<small>-jekyll</small></a></h3><sup
      >via <a href="https://github.com/anydigital/bladeswitch/blob/main/Gemfile" target="_blank">Gemfile</a></sup></pre>
    </td>
    <td>
      <pre><h3>1. <a href="https://github.com/anydigital/eleventy-blades" target="_blank">eleventy-blades</a></h3><sup
      >via <a href="https://github.com/anydigital/bladeswitch/blob/main/package.json" target="_blank">package.json</a></sup></pre>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <pre><h3>2. <a href="https://github.com/anydigital/blades" target="_blank">blades<small>-theme</small></a></h3><sup
      >as remote_theme via <a href="https://github.com/anydigital/bladeswitch/blob/main/_config.yml#L1" target="_blank">_config.yml</a
      > or via <a href="https://github.com/anydigital/bladeswitch/blob/main/package.json" target="_blank">package.json</a> for 11ty</sup></pre>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <pre><h3>3. <a href="https://github.com/picocss/pico" target="_blank">pico<small>.css</small></a> <small>optional</small></h3><sup
      >from CDN via <a href="https://github.com/anydigital/bladeswitch/blob/main/_data/site.yml#L3" target="_blank">_data/site.yml</a></sup></pre>
    </td>
  </tr>
</table>

---

## Quick start

<div class="grid"><div>

###### <mark>A.</mark> Natively, w/o GitHub Actions:

<p><a href="https://github.com/new?template_name=bladeswitch&template_owner=anydigital" target="_blank" role="button" class="contrast">
  Using Jekyll on GitHub Pages
</a></p>

1. Click ↑ to init your own repo.
2. Go to ⚙️ _Settings → Pages_.
3. Set _Branch_ to `main` and _Save_.

</div><div>

###### <mark>B.</mark> Fully preconfigured:

<a href="https://app.netlify.com/start/deploy?repository=https://github.com/anydigital/bladeswitch" target="_blank" role="button" class="contrast">
  Using 11ty (Build Awesome) on Netlify
</a>

</div></div>

---

## All you need

<div class="breakout-item" data-theme="dark">

```treeview
_includes/
└── default.liquid    # YOUR layout template
_data/site.yml        # YOUR site-wide metadata
*.md                  # YOUR content (editable via CMS!)
```

</div>

Under the hood:

```treeview
_config.yml           # Jekyll config
Gemfile               # Jekyll gems
package.json          # 11ty packages
admin/                # Sveltia CMS configs
```

---

## More info

<big>Repo: https://github.com/anydigital/bladeswitch</big>

Featured in:

- https://11tybundle.dev/starters/
- https://www.11ty.dev/docs/starter/
- https://sveltiacms.app/en/docs/start & [11ty](https://sveltiacms.app/en/docs/frameworks/eleventy) & [Jekyll](https://sveltiacms.app/en/docs/frameworks/jekyll)
- https://any.digital/tricks/build-awesome-11ty/#min-starters
- https://github.com/anydigital/awesome-11ty-build-awesome
