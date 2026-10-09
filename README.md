# ParkRadar

Know before you park. A campus parking app with enforcement reports, lot availability, zone rules and walking directions on Mapbox street and satellite maps.

## Files

- `index.html` is the whole app. It shows Mapbox street and satellite maps (the layers button under the zoom buttons switches between them), but only after the visitor taps Allow on the consent banner. Without that, the lots are drawn on a plain background.
- `manifest.webmanifest` and the icons let people add it to their home screen.

## Running it

It's hosted with GitHub Pages at https://parkradarapp.com/. To update the app, upload a new `index.html` to this repository.

On an iPhone, open the link in Safari, tap Share, then Add to Home Screen. ParkRadar then opens full screen, like an app.

## Shared reports

Reports and lot updates are shared live between everyone using the site and the ParkRadar iPhone app, through Firebase (anonymous sign-in plus Cloud Firestore). The security rules are in `firestore.rules` in the project folder. Each person's permit, vehicle and saved car stay private to them. If Firebase can't be reached, the site falls back to keeping reports on that device.
