# URL Protocol Converter

A simple, standalone web app that converts protocol URLs (like steam://) to shareable HTTPS links that work on any platform. Perfect for sharing URLs that normally aren't clickable on social media, chat platforms, or other websites.

**🌐 Live at: [https://steadirect.com](https://steadirect.com)**

## Deployment

The app is completely self-contained in a single `index.html` file. You can host it anywhere:

- GitHub Pages
- Netlify
- Vercel
- Any web hosting service that can serve static files

## Features

- No external dependencies
- Single file deployment
- Works on any hosting platform
- Automatic URL parameter handling
- Client-side only (no server required)
- Easy copying with dedicated copy button
- Dark mode support:
  - Automatically detects system theme preference
  - Manual theme toggle button
  - Remembers user's preferred theme
  - Smooth theme transitions
- Accessibility:
  - Screen reader compatible
  - ARIA labels and roles
  - Semantic HTML structure
  - Keyboard navigation support
- Privacy focused:
  - All URL conversion is done locally in the browser
  - No data collection or logging
  - No external requests or tracking

## How it Works

1. Using the web interface at [steadirect.com](https://steadirect.com), or by creating URLs directly:
   ```
   https://steadirect.com/?url=steam://joinlobby/1131190/109775241747665514
   ```

2. When someone clicks the generated link, the app automatically redirects them to the original protocol URL:
   ```
   steam://joinlobby/1131190/109775241747665514
   ```

## Examples

The converter works with any protocol URL, for example:

```
steam://joinlobby/1131190/109775241747665514
discord://discord.com/channels/123456789
```

Generated shareable link:
```
https://steadirect.com/?url=steam://joinlobby/1131190/109775241747665514
```

The app can also be self-hosted - it will automatically use whatever domain it's running on to generate the correct links.

## Disclaimer

This is an independent tool and is not endorsed by or affiliated with Valve Corporation or any other platform. Steam® and the Steam logo are registered trademarks of Valve Corporation. This tool simply facilitates the conversion of URLs and performs all operations locally in your web browser without collecting or logging any data.

## Links

- [PacNP.al](https://pacnp.al)
- [@pacnp.al on Bluesky](https://bsky.app/profile/pacnp.al)