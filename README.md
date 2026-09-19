# Railway Atlas

Responsive, self-contained static 3D explorer for the three user-supplied railway drawings: CBS-0046, CBS-0045 and B-221-2024. Open the original PDFs, inspect the corresponding boards and rotate each interpretive model.

## Run

Serve this directory with `python3 -m http.server 4173` and open `http://localhost:4173`. No build or API keys required. `npm run check` validates JavaScript syntax. Three.js r170 and OrbitControls are vendored; see vendor/THIRD_PARTY_LICENSES.txt. Google Fonts is optional; system fonts work offline.

## Publish

In GitHub Settings → Pages, deploy from branch `main`, folder `/ (root)`. All asset links are relative and support `/railway-site/`. `.nojekyll` is included. This project contains no server, trackers, sign-in or external data requests.

## Controls

Choose any of the three drawings. Drag to orbit; wheel/pinch to zoom; use camera presets, dimension and overhead-equipment toggles. Tap the visualisation board to enlarge and zoom. The blue-and-white Vande Bharat-inspired eight-coach train starts a pass every 30 seconds while the page is active. Each pass lasts 14 seconds. Pause and Run now are available. Reduced-motion preference pauses autoplay initially; background tabs do not advance animation time.

## Scope and source truth

The PDFs in assets are the original supplied bytes. Visualisation boards are generated interpretations. 3D models are simplified illustrations, not structural, load, fabrication or clearance verification. Indian broad-gauge geometry uses 1.676 m nominal gauge (between rail-head inner edges), with sleepers, steel rails and illustrative overhead electrification. The train shape, equipment, supports outside specified details, scenery and operating speed are illustrative. Animation does not assert that this rolling stock is approved for the bridges.

CBS-0046 lists generic span options; the model uses a 30.5 m illustrative span. Its conflicting plate notes remain visible. CBS-0045 is marked provisional; the unprovided refuge dimensions are illustrative. Ladder height and surrounding bridge span for B-221-2024 remain explicitly unspecified; an illustrative height is used only for the 3D scene.

Uploaded railway drawings retain their original ownership and notices; this independent visual study is not an official Indian Railways or RDSO website.
