# ParkRadar

Know before you park. A campus parking app with enforcement reports, lot availability, zone rules and walking directions on the Ole Miss parking map.

## Files

- `index.html` is the whole app.
- `map.webp` is the campus map picture. `index.html` loads it by name and tells the browser to fetch it first. If you rename it, update the two places in `index.html` that say `map.webp`.
- `manifest.webmanifest` and the icons let people add it to their home screen.

## Running it

It's hosted with GitHub Pages at https://harlanyerger.github.io/ParkRadar/. To update the app, upload the changed files (`index.html`, and `map.webp` if the map changed) to this repository.

## Note

On this site each phone keeps its own reports. Shared, live reports between users need a backend such as Firebase.
