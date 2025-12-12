# My Project Showcase

A minimal, polished landing page that curates and links to my portfolio, apps, frameworks, websites, games, and fun utilities — all in one place. Built with vanilla HTML, modern CSS, and a single line of JavaScript.

## Highlights
- Clean card-based layout with section accents for quick scanning
- Responsive grid that adapts from mobile to desktop (`styles.css`:72)
- Accessible external links with `target="_blank"` and `rel="noopener"` (`index.html`:23)
- Design tokens for easy theming (`styles.css`:1)
- Subtle motion and hover effects, with reduced-motion support (`styles.css`:191)

## Tech Stack
- HTML5 (`index.html`)
- CSS3 with custom properties and gradients (`styles.css`)
- JavaScript (minimal; helper function defined in `script.js`:1)

## Directory
- `index.html` — Page markup and curated project links
- `styles.css` — Global styles, tokens, responsive grid, card UI
- `script.js` — Minimal utility; `openProject(url)` (`script.js`:1)

## Quick Start
- Open `index.html` in any modern browser
- No build step, no dependencies

## Customize
- Add a project card:
  - Duplicate an existing `<a class="card">...</a>` block inside the desired section (e.g., Featured, Apps) and change the `href`, icon, title, and meta (`index.html`:22).
- Add a new section:
  - Create a new `<section class="section section--yourname">` with a `.section-title` and a `.cards` grid (`index.html`:20).
  - Define section accent colors by overriding `--accent` and `--accent-2` for `.section--yourname` in `styles.css` (see examples at `styles.css`:197).
- Tweak theme:
  - Update global design tokens in `:root` (`styles.css`:1) for colors/contrast.
  - Change typography via the Google Fonts import (`index.html`:10).

## Deployment
- Static hosting options: GitHub Pages, Vercel, Netlify, or any static server
- Steps (generic):
  - Push the three files (`index.html`, `styles.css`, `script.js`) to your repository
  - Point your host to the repository root; no build is required

## Notes
- Cards use a consistent UI with gradient accents and hover lifts (`styles.css`:113)
- The decorative icon in each card is marked `aria-hidden="true"` for clarity (`index.html`:24)
- Footer credits indicate authorship and year (`index.html`:220)

## Sections Overview
- Featured — portfolio and top-level links (`index.html`:20)
- Apps — small web apps (Todo, Weather, Notes, BMI, Calculator) (`index.html`:44)
- Frameworks — starter deployments (Next.js, Angular, Nuxt, Svelte) (`index.html`:98)
- Websites — community and org sites (`index.html`:128)
- Games — simple browser games (Dodge, Snake, Ping Pong, Tic Tac Toe) (`index.html`:158)
- Fun — randomizers and utilities (Coin Flip, Dice, Jokes, Clock) (`index.html`:188)

