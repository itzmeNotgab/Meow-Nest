# Meow Nest

![logo](logo.png)

A cute pink pet game: look after Mochi the cat in a cozy room.
One self-contained `index.html` (sprites embedded), no build step. Installable as a fullscreen app (PWA manifest included).

## Features
- Pet, feed (drag food onto Mochi), play with the red dot, throw toys, zoomies, nap spots
- Unlimited furniture: drag to move on a tiny grid, drop on the trash to delete
- Mochi walks around furniture, climbs on it, stretches, naps and more
- Coin shop for furniture and cat outfits (food is unlimited), daily gift, mini-games (Fish Splash, Treat Catch) that earn coins
- Mochi naps in the cat bed, climbs the cat tree and watches the TV or aquarium when they are on
- Day and night follow the phone clock (window sky, lamp and TV glow, sleepier Mochi)
- One continuous home: drag to look around, rooms flow into each other (Living room, Bedroom, Garden), tap a lock to unlock the next one
- Up to 3 cats, each with its own name, coat (10 colours), needs and outfits; tap the chips (bottom left) to switch or add a cat
- 14 foods, crisp vector icons, photo mode with share/save, picture frames that hold your own photos, wall and floor themes per room
- Synthesized sound effects; progress saved in the browser
- Fullscreen landscape layout: menu on the left, item bar on the right

## Run locally
Open `index.html`, or run `python3 -m http.server` and visit http://localhost:8000.

## Deploy to GitHub Pages
1. Push these files to the `main` branch of a new repo.
2. **Settings -> Pages -> Source: GitHub Actions**.
3. Push to `main` (or run the workflow from the Actions tab). The site goes live at `https://<your-username>.github.io/<repo-name>/`.

## Files
- `index.html` the whole game
- `manifest.webmanifest`, `icons/` app icons
- `logo.png` the logo
- `.github/workflows/deploy.yml` Pages deploy
- `assets/` original sprite sheets (reference only)

## Android APK
The workflow `.github/workflows/android-apk.yml` builds a signed `MeowNest.apk` (Actions tab -> latest run -> Artifacts -> MeowNest-apk). Keep the repo private: `release.keystore` is the signing key.
