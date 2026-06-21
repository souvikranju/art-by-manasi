# art-by-manasi

**আঁকিবুকি - By Manasi** is a simple static art gallery. Tap/click any thumbnail to open a zoomed modal view.

> **License:** This project is privately licensed. See `LICENSE` for terms (no copy, no edit).


## Demo / How to run
This project requires no build step.

1. Open `index.html` in your browser.
2. Click/touch an image thumbnail to zoom.

## Controls
- **Open zoom**: click/touch any thumbnail.
- **Close zoom**: click the **×** button at the top-right of the modal.

## Project structure
- `index.html` - gallery UI + modal logic
- `jquery.min.js` - local jQuery used by `index.html`
- `src/` - assets for thumbnails and the background
  - `src/bg.jpg` - page background
  - `src/Img00001.jpg` … `src/Img00082.jpg` - thumbnail images
- `src/full/` - full-size images used for the zoom view
  - `src/full/Img00001.jpg` … `src/full/Img00082.jpg`
- `src/loading.gif` - loading image shown briefly when closing

> Note: The zoom image path is computed by replacing `/src` with `/src/full`.

## Adding more artworks
1. Add a new thumbnail image named like `Img00083.jpg` into `src/`.
2. Add the matching full-size image named `Img00083.jpg` into `src/full/`.
3. Add a corresponding `<img class="myImg" ...>` line in `index.html` (following the existing sequence).

