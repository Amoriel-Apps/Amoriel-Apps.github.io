# Amoriel-Apps.github.io

Static site for **Amoriel Apps**, served by GitHub Pages. No build step, no dependencies.

Owner: Pratik P Shringarpure · Contact: amorielapps@gmail.com

## Layout

```
index.html                      landing page
404.html                        GitHub Pages serves this on any bad URL
projects/index.html             projects listing
projects/quit-munchies/         Quit Munchies: Habit Tracker
  ├─ index.html                 redirects to support.html
  ├─ support.html
  ├─ privacy.html
  └─ terms.html
assets/site.css                 shared stylesheet (light + dark themes)
assets/mark.png                 logo, transparent background — used on every page
assets/og-card.png              1200x630 social preview card
assets/favicon-16/32.png        browser icons
assets/apple-touch-icon.png     180x180 iOS home-screen icon
assets/icon-192/512.png         PWA manifest icons
logo.png                        master logo, 1254x1254, cream background
robots.txt, sitemap.xml, site.webmanifest
```

## App Store URLs

Live at https://amoriel-apps.github.io

| Page | URL |
| --- | --- |
| Support | `https://amoriel-apps.github.io/projects/quit-munchies/support.html` |
| Privacy Policy | `https://amoriel-apps.github.io/projects/quit-munchies/privacy.html` |
| Terms of Use (EULA) | `https://amoriel-apps.github.io/projects/quit-munchies/terms.html` |

## Conventions

- **One stylesheet.** Studio pages (`index.html`, `projects/`, `404.html`) all pull
  `/assets/site.css`. Change a color there and it changes everywhere. The Quit Munchies
  pages deliberately keep their own teal styling to match the app.
- **Themes** come from CSS custom properties under `prefers-color-scheme`. All text/background
  pairs meet WCAG AA (4.5:1) in both themes — check before changing `--solid`, `--link` or `--muted`.
- **Absolute URLs** in `og:` / `twitter:` / `canonical` tags. Social scrapers reject relative ones.
- **Root-relative paths** (`/assets/...`) so pages work at any depth.
- Adding a page? Add it to `sitemap.xml` too.

## Local preview

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Publishing

Push to `main`, then: **Settings → Pages → Source: Deploy from a branch → `main` / `/ (root)`**.
