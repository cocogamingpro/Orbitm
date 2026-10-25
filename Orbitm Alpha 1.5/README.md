# Orbitm — Alpha 1.5

A browser sandbox that simulates gravity. Place stars, planets, asteroids and black holes, then watch them move.

## Run locally
Open `index.html` in a browser. No build step, no dependencies.

## Menus
- The **main menu** has Play, Dictionary, Version history and Settings.
- In the game, press **Esc** (or the Menu button) for Resume, Save, Load, Settings and Quit to main menu.

## Controls
- **Point placement**: the object starts at rest and falls toward nearby mass.
- **Orbit placement**: click the object to orbit, then move and click. A line shows the distance, and a dotted path shows the orbit. The "Orbit speed" slider makes it circular (1.00), elliptical (below 1) or open (above 1.41).
- **Launch**: in Point placement, drag before releasing to give the object a velocity. A gold arrow and dotted path show where it will go.
- **Inspect**: click an object to see its live orbit (dotted white line), rename it, change its mass, size or colour, drag it somewhere else, set its velocity, stop it or delete it.
- **Project**: Save file, Load file, and Share link (the whole system is stored in the link after the `#`, so nothing needs a server).
- **Physics and realism** (panel toggles): tidal breakup of planets that get too close to a heavy body, habitable zones and planet temperatures, Lagrange points for the selected object, black hole lensing, spinning disk and jets, and real units (AU, solar masses, km/s, years).
- **Graphs**: Inspect an object to see live graphs of its distance, speed and orbital energy.
- **Challenges**: seven guided goals (open from the panel), with progress saved in your browser.
- **Hover tooltips** on controls link straight to the dictionary.
- **Settings**: menu theme, graphics quality, sound effects, ambient sound and volume. On touch screens, pinch to zoom and use two fingers to move.
- **Follow camera**: lock the view on the selected object or on the centre of mass (Follow button).
- **Undo** (Ctrl+Z) and **Rewind**: scrub back through the last 60 seconds of simulation, then press Play from here.
- **Presets**: demo, solar system, binary star, figure-eight orbit, rogue black hole, Trojan asteroids, blank sandbox.
- **Language**: English or French (Settings). The game picks French automatically if your browser is set to French.
- **Dictionary**: explains every object and bit of physics in the game. "Learn about this" opens the entry for the selected object.
- Scroll to zoom, right-drag or middle-drag to move, Space to pause, Esc to cancel.
- Objects that touch merge and conserve momentum. Black holes swallow what they touch.

## Publish
1. Push to GitHub: `git init && git add . && git commit -m "Orbitm phase 1" && git branch -M main && git remote add origin <your-repo-url> && git push -u origin main`
2. On render.com choose **New → Static Site** and connect the repo.
3. Leave Build Command empty and set Publish Directory to `.`, then click **Create Static Site**.
