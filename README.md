# ParkRadar

Know before you park. A campus parking app with enforcement reports, lot availability, zone rules and walking directions on the Ole Miss parking map.

## Files

- `index.html` is the whole app.
- `map.webp` is the campus map picture. `index.html` loads it through Netlify Image CDN (`/.netlify/images?url=/map.webp`), which sends each browser the smallest format it supports (AVIF or WebP). If that address isn't available (for example on GitHub Pages, or when opening the file straight from your computer), the page loads `map.webp` directly instead.
- `netlify.toml` tells browsers they can keep the map for a year. If you change the map, give the new file a new name (like `map-2.webp`) and update the two places in `index.html` that say `/map.webp` plus the `for =` line in `netlify.toml`. Otherwise returning visitors keep the old map.
- `manifest.webmanifest` and the icons let people add it to their home screen.

## Running it

To update the app, upload the changed files (`index.html`, and `map.webp` if the map changed) to this repository. The Netlify features (Image CDN and the one-year caching rule) only work when the site is hosted on Netlify.

## Note

On this site each phone keeps its own reports. Shared, live reports between users need a backend such as Firebase.
