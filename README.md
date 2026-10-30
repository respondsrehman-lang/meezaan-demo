# Meezaan — Fine-Dining Courtyard Concept (Demo)

An original multi-page concept site for **Meezaan**, a fictional fine-dining, multi-cuisine courtyard restaurant in DHA Phase V, Karachi.

**Live demo:** https://respondsrehman-lang.github.io/meezaan-demo/

## Pages

| Page | Contents |
|---|---|
| `index.html` | Home — hero, stats, chef's signatures, ambiance strip, explore cards, reviews, reservation band |
| `menu.html` | Full interactive menu — 12 categories / ~120 dishes with tabbed browsing, sticky category strip and dish thumbnails |
| `events.html` | Celebrations — birthday evenings, corporate events, nikkah & private gatherings, iftar buffet |
| `visit.html` | Find us & reservations — address, hours, phone/WhatsApp, map, socials, reservation card |

## Design

- **Ivory & gold bright theme** — warm cream base with gold/terracotta accents and an original red-and-white flower-petal logo (`assets/logo.svg`, `assets/favicon.svg`).
- **Glassmorphic cards everywhere** — frosted-white glass (`backdrop-filter: blur + saturate`) layered over food/interior photography. An `@supports` fallback keeps things readable where blur isn't supported.
- **Interactive menu** — 12 categories / ~120 dishes as a tappable category browser with a sticky tab strip, per-category counts, and a representative photo thumbnail per dish (graceful lettered-tile fallback if an image fails).

## Assets

- **Logo & favicon** — original SVG artwork (six red/white petals in a gold ring). No third-party brand assets used.
- **Imagery** — all food and interior photos are stock images hotlinked from [Unsplash](https://unsplash.com) (Unsplash License — free for commercial and noncommercial use, no permission needed).

**All business details on the site — phone number, WhatsApp number, email, address, stats, ratings and reviews — are illustrative placeholders for the concept, not a real business.**

## Stack

Four self-contained HTML pages — each page carries its own inline CSS/JS, no build step, no dependencies. Google Fonts (Cormorant Garamond + Jost), inline SVG icons, vanilla JS (menu tabs + thumbnails, scroll reveal, mobile nav). Reduced-motion and keyboard-accessible.

## Deploy (GitHub Pages)

```bash
git init
git add .
git commit -m "Meezaan concept demo"
git remote add origin https://github.com/respondsrehman-lang/meezaan-demo.git
git push -u origin main
```

Pages is served from the repo `Settings → Pages` (branch: `main`, root).
