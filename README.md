# System Thinking Lab — landing

Static landing page. No build step, no dependencies.

## Structure

```
system-thinking-lab/
├── index.html          # markup
├── css/
│   └── styles.css      # all styles; design tokens in :root
├── assets/
│   └── favicon.svg     # M mark
├── robots.txt
└── README.md
```

## Run locally

Open `index.html` in a browser, or serve the folder:

```
npx serve .
```

## Deploy

The folder is the site root — publish it as is.

- **GitHub Pages**: push to a repo, Settings → Pages → deploy from branch, folder `/ (root)`.
- **Netlify / Vercel / Cloudflare Pages**: no build command, output directory `.`.

All paths are relative, so it also works from a subpath (e.g. `user.github.io/repo/`).

## Before going live

- Replace the `href="#join"` on the "Join the lab" buttons with the real signup link (marked with a TODO in `index.html`).
- Add `og:image` and `og:url` meta tags once the domain and a share image exist.
- Fonts load from Google Fonts (Archivo, Cormorant Garamond, JetBrains Mono).

## Theming

Colors, fonts and spacing are CSS variables at the top of `css/styles.css`. The accent is `--accent`.
