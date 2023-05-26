## Desc

the hugo module based on `hugo-enterprise` for website: `zeeis.netlify.app`

---

## Use module

config in your website project:


`./config/_default/config.yaml`

```yaml
module:
  imports:
    - path: github.com/zeeis/hugo-zeeis-theme
    - path: github.com/zeeis/hugo-enterprise
```

`./go.mod`

```mod
require	github.com/zeeis/hugo-zeeis-theme v0.1.9
require	github.com/zeeis/hugo-enterprise v0.1.20
```

---

## Publish new package

git tag a commit of `hugo-zeeis-theme` with version (eg: `v0.2.0`), then push.

config `go.mod` of your website project to use specific version module

```mod
require github.com/zeeis/hugo-zeeis-theme v0.2.0
```

---

## Content

- themes
  - `data/theme/zeeis.yaml`
- [widgets](./docs/widgets.md)
  - zs.hero
- [views](./docs/views.md)
  - zs.card
- [layouts](./docs/layouts.md)
  - zs.services
  - zs.products
