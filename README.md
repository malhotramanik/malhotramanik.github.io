# malhotramanik.github.io

Personal site of Manik Malhotra, a Senior Software Engineer at Porter working on backend systems, distributed platforms and database performance.

Live at **https://malhotramanik.github.io**

## What's on the page

- **Hero** with an interactive `psql` console. Click a preset query to see it typed out and its result.
- **Now at Porter**, the work in progress this year.
- **Experience**, a delivery-route timeline whose stops expand to show details.
- **Toolkit** and working principles.
- **Contact** through LinkedIn and X.

## How it's built

A single static `index.html` with inline CSS and a small script for the console. There's no framework, build step or dependencies. Fonts (Archivo and IBM Plex Mono) load from Google Fonts.

```
index.html                  the whole site
assets/img/profile-img.jpg  portrait used in the nav
assets/img/favicon.svg      browser icon, with favicon.png as fallback
assets/img/apple-touch-icon.png
```

It supports light and dark mode (following the system setting), works down to phone widths, and respects reduced-motion preferences.

## Running locally

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Deploying

GitHub Pages serves the `master` branch. Merging to `master` publishes the site.
