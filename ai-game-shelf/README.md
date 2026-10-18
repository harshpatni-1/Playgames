# The Game Shelf

A static website that presents four standalone browser games with one dedicated page per game.

## Run locally
Open `index.html` in a browser. For best compatibility, run a local static server from this folder, for example:
- `python -m http.server 8000`
- then visit `http://localhost:8000`

## Deploy
Upload the contents of this folder to a static host such as Netlify, Vercel, or GitHub Pages. Keep the directory structure unchanged.

## Project structure
- `index.html` — collection homepage
- `assets/site.css` — shared showcase styling
- `games/<builder>/index.html` — dedicated page and isolated game frame
- `games/<builder>/play.html` — original standalone game HTML

The original games are kept in separate iframe documents so their global CSS, canvas, keyboard handlers, and JavaScript do not collide with each other or the showcase navigation.
