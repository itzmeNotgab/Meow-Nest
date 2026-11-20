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
- Up to 3 cats, each with its own name, breed, needs and outfits; tap the chips (bottom left) to switch or add a cat
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

## v14 additions
- Minimal screen: only Menu, coins, cat button and one round ✨ button show. Meters appear as a small alert only when a stat is low; cat name tags show only on the selected cat; the menu closes after you pick something and the ✨ button hides while panels are open.

## v13 additions
- The bottom buttons now live behind one "✨ Tools" button that opens a row; your cats live behind a "🐱 name" button that opens a row of cats. Both close after you pick something.

## v12 additions
- Cleaner layout: menu, coins and live hunger/fun/energy meters top-left; mode buttons (House, Human/Spectator, Me, Edit, Photo) in a dock at the bottom; the menu is grouped into Care, Shop and More; messages appear at the top.
- Food tiles show price and how much hunger they fill, with a heart on your cat's favourite. Eating now makes crumbs in the food's colour, a floating +hunger number and hearts for favourites.
- Soft vignette and panel animations for a cosier feel.

## v11 additions
- Human is now a bigger pixel character in the animated-base style (dark outline, large head, tall eyes) with 4 directions and a walk cycle. Customise skin, eyes, hair style and colour, top (T-shirt, long sleeve, hoodie) and colour, bottoms (long, shorts, skirt) and colour.
- House view is a square cutaway: tap a room to select it first, then Go in, Walls or Resize. In Resize, drag the pink handle on the room's right edge (or use - / +). Rooms go from 45% to 100% width.
- Walls: separate Floors and Walls pickers per room, plus ready-made themes.
- Human mode: double-tap a cat and your character walks over and lifts it overhead. Tap the cat or press "Put down" to let go. Holding a cat still works (long-press and drag, also in House view).
- Spectator mode: no character on screen, for editing and watching. Editing switches to it automatically.
- Breeds instead of colours: Persian, Maine Coon, Norwegian Forest, Ragdoll and friends get fluffy outlines, Munchkin and Abyssinian differ in size and coat, plus British Shorthair, American Shorthair, Burmese, Siamese, Bengal, Sphynx and more. Old pink, purple and mint cats became real breeds.

## v10 additions
Square house view (tap House), tap a room then Go in, Walls or Resize; hold a cat to pick it up; Human or Spectator mode, character creator (Me); cat breeds.

## v9 additions
Cat personalities and favourite foods, cats hang out together, kittens that grow, garden weather and bird visitors, daily quests, food combos, Kitchen and Rooftop rooms, cat book with photo gallery and save code.

## v15 clean layout
- Top left: round menu button, coins and the cat chip. Bottom: three small round buttons (house view, brush, camera).
- The brush button is edit mode. Rotate, colour, photo and put-down appear above it only while editing.
- Menu is six tiles: Feed, Play (laser dot, toys, zoomies, games), Home (furniture, decor, rooms, day/night), Style (outfits, cats, you), Rest (sleep, nap spot), Book.

## v16 bathroom, kitchen, shower
- All rooms are open from the start (no unlocking). New 6th room: Bathroom (house view, bottom right).
- New furniture (shop sections Bathroom / Kitchen / Cat bowls): bathtub, shower, toilet, sink, washing machine, towel rack, bath mat, laundry basket, rubber duck, towels, soap; stove, counter, kitchen sink, upper cabinet, microwave, kettle, toaster, coffee maker, fruit bowl, pot; food and water bowls.
- Cats get a Clean stat that slowly drops. Menu -> Care -> Shower walks the selected cat to a Shower (or Bathtub) and washes it (+3 coins).
- Foods: bell pepper and potato replaced by Kibble and Egg.
