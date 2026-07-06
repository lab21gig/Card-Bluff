# Card Bluff — Play it on the web (GitHub Pages)

This folder is the whole Card Bluff web app (a PWA). Put these files in a
GitHub repo, turn on GitHub Pages, and you get a free public link anyone
can open in a browser — and install to their home screen like a real app.
No app store, no Mac, no build tools.

Everything is self-contained: the rendering engine is bundled in, so it
works even on networks that block Google's CDN, and it works offline after
the first load.

---

## Easiest way (all in the browser, ~5 minutes)

1. Go to https://github.com and sign in (create a free account if needed).
2. Click the **+** (top right) → **New repository**.
   - Name it whatever you like, e.g. `card-bluff`.
   - Set it to **Public**.
   - Click **Create repository**.
3. On the new empty repo page, click **uploading an existing file**.
4. **Drag in EVERYTHING from this folder** — `index.html`, `main.dart.js`,
   `flutter_bootstrap.js`, the `assets`, `canvaskit`, and `icons` folders,
   `manifest.json`, `.nojekyll`, all of it. (You can drag the files and
   folders straight from your unzipped folder.)
   - Tip: if the drag-and-drop won't take folders, drag the files in
     batches, or use GitHub Desktop, or zip-free just select all.
5. Click **Commit changes**.
6. Go to the repo's **Settings** → **Pages** (left sidebar).
7. Under **Build and deployment → Source**, choose **Deploy from a
   branch**. Set branch to **main** and folder to **/ (root)**. Save.
8. Wait ~1 minute, refresh the Pages settings page, and it shows your live
   URL, like `https://YOURNAME.github.io/card-bluff/`.

Open that link — Card Bluff loads and plays. Share it with anyone.

## Installing it like an app

- **On Android/Chrome:** open the link, then menu → **Install app** (or
  "Add to Home screen").
- **On iPhone/Safari:** open the link, tap **Share** → **Add to Home
  Screen**. It launches full-screen with the Card Bluff icon, no browser
  bars.

## A note on the URL path

The app is built to work at **any** address automatically — whether that's
`YOURNAME.github.io/card-bluff/` (a normal repo) or `YOURNAME.github.io/`
(if you name the repo exactly `YOURNAME.github.io`). You don't have to
change anything either way.

## What works on the web version

Everything single-device: Practice vs AI, Pass & Play, the full rules,
stats, XP, achievements, sounds, animations — all identical to the phone
app. The only thing missing is **Play on Wi-Fi** (browsers can't open the
direct device-to-device network connections it needs), so that button is
shown greyed-out on the web version. Use the Android/iPhone app for Wi-Fi
multiplayer.

## Updating it later

Rebuild the web app and replace the files in the repo (drag the new ones
in, commit). GitHub Pages redeploys automatically within a minute.
