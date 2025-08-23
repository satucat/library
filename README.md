# Saturn's Library (Self-hostable)
A tiny static site that lists and launches web games defined in `/games.json`.

## Quick start
1. Put the folder on any static host (GitHub Pages, Netlify, Vercel, S3, nginx, IIS, etc.).
2. Edit `/games.json` to add your games. Icons go in `/icons/`.
3. Open the site in a browser.

### games.json format
```json
[
  {
    "title": "My Game",
    "description": "What it is.",
    "url": "https://example.com/my-game",
    "icon": "/icons/my-game.svg",
    "tags": ["puzzle", "casual"]
  }
]
```
- `icon` can be `.svg`, `.png`, or `.jpg`. Put the file in `/icons/`.
- If `icon` fails to load, the site falls back to `/icons/saturn.svg`.

## Dev tips
- You can't just double click the HTML.
- If you double click the HTML, it will try and get games from index.html/games.json (??)
- Instead, use any host you want, like GitHub, Vercel, or just use python -m http.server.
- Totally up to you.
