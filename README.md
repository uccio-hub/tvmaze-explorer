# Scene — TV Show Explorer

A responsive, dependency-free web app that searches TV shows through the free public TVmaze REST API.

## Features

- Fuzzy show search using `/search/shows?q=`
- Genre, status and language filters
- Sorting by relevance, rating, premiere date or name
- Complete show detail view
- Seasons and full episode guide, including specials
- Cast, characters, crew, alternate titles and image gallery
- External IDs, schedule, network/web channel and official links
- Raw combined JSON view so every returned API field remains accessible
- Deep-linkable searches through the URL hash
- Responsive layout and keyboard-accessible modal

## Run locally

Open a terminal in this folder and run:

```powershell
py -m http.server 5500
```

Then visit:

```text
http://localhost:5500
```

No API key or environment file is required. The browser connects directly to `https://api.tvmaze.com`, which supports CORS.

## Files

- `index.html` — page structure
- `styles.css` — visual design and responsive layout
- `app.js` — API integration, filters and detail views

## API endpoints used

- `/search/shows?q=:query`
- `/shows/:id`
- `/shows/:id/episodes?specials=1`
- `/shows/:id/seasons`
- `/shows/:id/cast`
- `/shows/:id/crew`
- `/shows/:id/akas`
- `/shows/:id/images`
- `/shows/:id/alternatelists`

Data and images are provided by TVmaze.
