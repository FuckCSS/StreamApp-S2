# StreamApp

A static frontend for searching and streaming movies and TV shows.

## Architecture

- **Type**: Pure static site (HTML, CSS, vanilla JavaScript)
- **No build system**: No bundler, package manager, or compilation step
- **Server**: `serve` (npm global package) serves files on port 5000

## File Structure

```
index.html       — Main search page
about.html       — About page
css/styles.css   — All styles (dark theme)
js/app.js        — Search logic, TMDB API calls, modal, player redirect
```

## Key Details

- Uses the **TMDB API** (The Movie Database) for movie/TV metadata. API key is hardcoded in `js/app.js`.
- Videos open via **tmdbplayer.nunesnetwork.com** in a new tab (external provider).
- No backend, no database, no authentication.

## Running

Workflow: `Start application` — runs `npx serve -s . -l 5000`

## Deployment

Configured as a **static** deployment with `publicDir: "."`.
