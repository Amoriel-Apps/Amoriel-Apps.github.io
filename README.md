# Amoriel-Apps.github.io

Static site for **Amoriel Apps**, served by GitHub Pages. No build step.

```
index.html                      landing page
projects/index.html             projects listing
projects/quit-munchies/         Quit Munchies: Habit Tracker
  ├─ index.html                 redirects to support.html
  ├─ support.html
  ├─ privacy.html
  └─ terms.html
logo.png                        master logo (1254x1254)
logo-512.png                    web-sized logo used by the pages
favicon.png                     64x64 browser icon
```

Contact: amorielapps@gmail.com · Owner: Pratik P Shringarpure

## App Store URLs

Live at https://amoriel-apps.github.io

| Page | URL |
| --- | --- |
| Support | `https://amoriel-apps.github.io/projects/quit-munchies/support.html` |
| Privacy Policy | `https://amoriel-apps.github.io/projects/quit-munchies/privacy.html` |
| Terms of Use (EULA) | `https://amoriel-apps.github.io/projects/quit-munchies/terms.html` |

## Local preview

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Publishing

Push to `main`, then in the repo: **Settings → Pages → Source: Deploy from a branch → `main` / `/ (root)`**.
