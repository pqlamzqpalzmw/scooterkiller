# LP60 Geofence

A GitHub Pages-ready prototype for managing an owned LP60-style scooter fleet.

## Current prototype
- Mobile-friendly dashboard
- Web Bluetooth device discovery where supported
- Scooter allowlist/state model
- Configurable 5 mph vs. lock policy
- Browser geolocation fence center
- Event log

## Important integration point
The prototype deliberately does **not** guess or replay proprietary scooter BLE commands. The `app.js` BLE section is the adapter boundary where an authorized LP60 GATT service/characteristic and manufacturer-supported command can be integrated after it has been identified and tested on a stationary scooter.

## GitHub Pages
Upload `index.html`, `style.css`, `app.js`, and `README.md` to a repository, then enable GitHub Pages from the repository's Pages settings.

Web Bluetooth requires HTTPS and browser/device support. GitHub Pages provides HTTPS.
