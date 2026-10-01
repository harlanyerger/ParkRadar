# ParkRadar

Know before you park. A campus parking app with enforcement reports, lot availability, zone rules and walking directions on the Ole Miss parking map.

## Files

- `index.html` is the whole app, with the campus map image built in. It also shows Mapbox street and satellite maps; the layers button under the zoom buttons switches between Streets, Satellite and the Ole Miss parking map.
- `manifest.webmanifest` and the icons let people add it to their home screen.

## Running it

It's hosted with GitHub Pages at https://harlanyerger.github.io/ParkRadar/. To update the app, upload a new `index.html` to this repository.

On an iPhone, open the link in Safari, tap Share, then Add to Home Screen. ParkRadar then opens full screen, like an app.

## Shared reports

Reports and lot updates are shared live between everyone using the site and the ParkRadar iPhone app, through Firebase (anonymous sign-in plus Cloud Firestore). The security rules are in `firestore.rules` in the project folder. Each person's permit, vehicle and saved car stay private to them. If Firebase can't be reached, the site falls back to keeping reports on that device.
