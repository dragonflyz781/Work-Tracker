# Round Tracker — GitHub Pages setup

This is a single self-contained web app (`index.html`) — a live GPS route
tracker with a schedule of drop times and a passenger on/off counter.
It already has the 360 (AM) and 360 (PM) routes built in.

Once hosted on GitHub Pages (rather than inside Claude), **real street
map tiles will load normally** — there's nothing else to configure.

## Put it on GitHub Pages (5 minutes)

1. Go to https://github.com/new and create a new **public** repository
   (e.g. `round-tracker`). You don't need to add a README or license.
2. On the new repo's page, click **"uploading an existing file"**
   (or drag-and-drop) and upload `index.html` from this package.
   Commit it to the `main` branch.
3. Go to the repo's **Settings → Pages**.
4. Under "Build and deployment", set **Source: Deploy from a branch**,
   **Branch: main**, folder **/ (root)**. Click **Save**.
5. Wait about a minute, then refresh that Pages settings screen — it
   will show your live URL, something like:
   `https://<your-username>.github.io/round-tracker/`
6. Open that link on your phone. For quickest access, use your
   browser's "Add to Home Screen" option so it opens like a normal app.

## Notes

- **Routes/data**: new GPX files you upload are saved in that device's
  browser storage (not shared between devices) unless you're opening
  this through Claude's artifact link, which can sync routes across
  devices. On GitHub Pages, each device/browser keeps its own uploads
  and passenger counts.
- **Updating it later**: if you want a newer version of the app (new
  features, a fixed bug), just re-upload a replacement `index.html`
  to the same repo — GitHub Pages updates automatically within a
  minute or two of the commit.
- **Passenger counts & GPS**: both work the same as before — nothing
  else to set up.
