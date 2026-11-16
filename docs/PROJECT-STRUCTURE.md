# Project structure

## Current source

- `index.html` — the complete game. It currently includes the HTML interface, CSS styling, JavaScript game logic, WebGL shaders/rendering, and synthesized audio logic in one file.
- `README.md` — project overview, run instructions, and repository map.
- `docs/OFFLINE-ANDROID.md` — notes for packaging the game as an offline Android app.

## Why the game remains a single HTML file

The supplied source is self-contained and has no external asset or library references. Keeping it intact avoids breaking relative paths and makes it straightforward to copy into an Android app's local assets folder.

If the project later grows separate images, music, fonts, or scripts, add dedicated folders such as `assets/images/`, `assets/audio/`, `assets/fonts/`, and `src/`, then update references in `index.html`.
