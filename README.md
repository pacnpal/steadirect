# Steam URL Converter

A simple, standalone web app that converts Steam URLs to shareable HTTPS links. Perfect for sharing Steam lobby links on platforms like Discord where steam:// URLs are not clickable.

## Deployment

The app is completely self-contained in a single `index.html` file. You can host it anywhere:

- GitHub Pages
- Netlify
- Vercel
- Any web hosting service that can serve static files

## How it Works

1. When hosted (e.g., at `https://yourdomain.com/`), the app will generate links like:
   ```
   https://yourdomain.com/?url=steam%3A%2F%2Fjoinlobby%2F1131190%2F109775241747665514
   ```

2. When someone clicks the generated link, the app automatically redirects them to the original Steam URL:
   ```
   steam://joinlobby/1131190/109775241747665514
   ```

## Examples

Original Steam URL:
```
steam://joinlobby/1131190/109775241747665514
```

Generated shareable link (if hosted on example.com):
```
https://example.com/?url=steam%3A%2F%2Fjoinlobby%2F1131190%2F109775241747665514
```

The app will work the same way regardless of where it's hosted - it automatically uses whatever domain it's running on to generate the correct links.

## Features

- No external dependencies
- Single file deployment
- Works on any hosting platform
- Automatic URL parameter handling
- Client-side only (no server required)