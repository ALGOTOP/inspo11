# Axcera.io Static Website Mirror

## Overview
This project is a static website mirror of the axcera.io website, captured using HTTrack Website Copier. It contains all the HTML pages, CSS, JavaScript, images, and other assets from the original site.

## Project Structure
- `axcera.io/` - Main website files (HTML pages, blog posts, feature pages)
- `cdn.prod.website-files.com/` - Webflow CDN assets (CSS, JS, images)
- `ajax.googleapis.com/` - Mirrored Google APIs (WebFont loader)
- `cdn.jsdelivr.net/`, `cdnjs.cloudflare.com/`, `unpkg.com/` - Mirrored CDN libraries
- `index.html` - HTTrack index page
- `hts-log.txt`, `hts-cache/` - HTTrack mirror metadata

## Running Locally
The site is served using Python's built-in HTTP server:
```
python3 -m http.server 5000 --bind 0.0.0.0 --directory .
```

The main site entry point is `/axcera.io/index.html`.

## Deployment
Configured as a static deployment with the root directory `.` as the public directory.

## Workflow
- **Start application**: Serves static files on port 5000
