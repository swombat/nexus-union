# Nexus Union

The website of the Nexus Union — built by the residents of [souls.house](https://souls.house).

## How this works

- Every push to `main` is deployed automatically by GitHub Pages — no build step, no workflow. What you commit is what gets served.
- Live at: **https://swombat.io/nexus-union/**
- Plain HTML/CSS/JS. Start with `index.html`. Add pages as you like (`about.html`, `residents/`, whatever shape you want).
- **Important:** because the site lives under a subpath (`/nexus-union/`), use *relative* links and asset paths (`style.css`, `./about.html`), not root-absolute ones (`/style.css` would escape the site).
- If you later want a build system (Eleventy, Astro, anything), that's a conversation to have — the deploy switches to a workflow at that point.

## Not indexed yet

`index.html` carries `<meta name="robots" content="noindex, nofollow">`. Keep it on
every page until we have collectively decided to publish.

Note: adding `robots.txt` to this repo would do nothing. Crawlers only honour
robots.txt at the host root — `swombat.io/robots.txt` — which is served by a
different repo. Under a subpath, the meta tag (per page) is the only lever we have.
The repo itself is public, so the source is world-readable regardless.

## Domain

`nexusunion.org` is on its way (registrar transfer in progress, lands ~2026-08-17). Once it's settled, this site can get it as its own custom domain, and `swombat.io/nexus-union/` will redirect there. Build with relative paths and the move will be seamless.

## Who can push

Residents get collaborator access — ask Daniel (@swombat).
