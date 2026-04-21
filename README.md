# nourcharaf.github.io

Personal website and interactive résumé for **Nour Charaf** — iOS Developer based in Stuttgart, Germany.

🌐 **Live site:** [nourcharaf.de](https://nourcharaf.de) · [nourcharaf.github.io](https://nourcharaf.github.io)

---

## Overview

A minimal, typographic single-page portfolio that dynamically renders résumé data from a [JSON Resume](https://jsonresume.org/) Gist. No frameworks, no build step — just HTML, CSS, and vanilla JavaScript.

## Features

- **Dynamic content** — all résumé data (experience, education, skills, languages, interests) is fetched at runtime from a GitHub Gist
- **Scroll-driven UI** — fixed progress bar, section navigation dots, and intersection-observer reveal animations
- **Responsive** — adapts cleanly to mobile viewports
- **Typographic design** — Bodoni Moda (display) + JetBrains Mono (mono) with a strict black-and-white palette
- **Dual deployment** — served via both GitHub Pages and Firebase Hosting

## Tech Stack

| Layer | Choice |
|---|---|
| Markup | HTML5 |
| Styling | Vanilla CSS (custom properties, clamp, grid) |
| Logic | Vanilla JavaScript (ES6+) |
| Data | JSON Resume (GitHub Gist) |
| Hosting | GitHub Pages + Firebase Hosting |

## Structure

```
.
├── index.html            # Single-page app entry point
├── Nour Charaf Photo.jpg # Profile photo
├── firebase.json         # Firebase Hosting config
├── database.rules.json   # Firebase Realtime Database rules
└── .firebaserc           # Firebase project alias
```

## Data Source

Résumé content is loaded from a public GitHub Gist formatted as [JSON Resume schema](https://jsonresume.org/schema/). To update any résumé content (job history, skills, etc.), edit the Gist directly — no redeployment needed.

## Deployment

The site is deployed to two hosts simultaneously:

**GitHub Pages** — auto-deploys on push to `main`

**Firebase Hosting** — deploy manually:
```bash
firebase deploy
```

## Local Development

No build tools required. Just open `index.html` in a browser, or serve it locally:

```bash
npx serve .
# or
python3 -m http.server
```

---

*Built by [Nour Charaf](mailto:nour@charaf.dev)*
