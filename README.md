# Khata — install as a mobile app

This folder is a complete, installable app (a "PWA"). Once it's hosted on any
HTTPS site, you can add it to your phone's home screen and it will:
- open full-screen with no browser bar, like a real app
- keep working with no internet connection
- keep all your data only on your own phone (nothing is uploaded anywhere)

## Fastest way to host it: GitHub Pages (free, permanent)

1. Go to https://github.com and sign in (or create a free account).
2. Click the **+** in the top right → **New repository**. Name it `khata` (or anything). Keep it Public. Create it.
3. On the new repo page, click **Add file → Upload files**.
4. Drag in all the files from this folder: `index.html`, `manifest.json`,
   `service-worker.js`, and the whole `icons` folder. Commit the changes.
5. Go to the repo's **Settings → Pages**. Under "Build and deployment",
   set **Source** to "Deploy from a branch", branch **main**, folder **/(root)**. Save.
6. Wait ~1 minute, then GitHub will give you a URL like:
   `https://yourusername.github.io/khata/`
7. Open that link on your phone:
   - **Android (Chrome)**: tap the **⋮** menu → **Add to Home screen** (or you'll
     see an automatic "Install app" prompt).
   - **iPhone (Safari)**: tap the **Share** icon → **Add to Home Screen**.
8. Open Khata from your home screen icon — it now behaves like a normal app.

## Notes

- Your data lives in the browser's local storage on your device only — there's
  no server, no account, no syncing. Uninstalling the app or clearing site
  data will erase it, so use the **Export backup (.json)** button occasionally
  to keep a copy.
- If you ever want to update the app, just re-upload the changed files to the
  same GitHub repo (Add file → Upload files again) — your existing data on
  your phone is untouched, since it's stored locally, not in the repo.
- Any static host works the same way (Netlify, Vercel, Cloudflare Pages) if
  you'd rather use one of those instead of GitHub Pages.
