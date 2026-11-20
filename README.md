# SIGMA Lots Calculator

A lightweight, mobile-first position-size calculator packaged as an installable Progressive Web App (PWA).

## Publish with GitHub Pages

1. Create a new **public** GitHub repository, for example `sigma-lots-calculator`.
2. Upload the contents of this folder to the repository's root. `index.html`, `manifest.webmanifest`, `sw.js`, and both icon files must be at the top level.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then Save.
6. Wait for GitHub Pages to publish. Your site will be at `https://YOUR-USERNAME.github.io/sigma-lots-calculator/`.

GitHub Pages serves the site over HTTPS, which is required for service workers and PWA installation.

## Install on Android

1. Open the published HTTPS address in **Google Chrome** (not the GitHub file preview and not the ZIP file).
2. Wait a few seconds for the page and service worker to finish loading. If needed, refresh once while online.
3. Open Chrome's **⋮** menu. Choose **Install app** if shown. On some Chrome versions it may appear as **Add to Home screen**; if it only offers a shortcut, check that the site is the published HTTPS Pages URL and that `manifest.webmanifest` and `sw.js` are present at the repository root.
4. Confirm installation. SIGMA should open in its own app window.

## Updating

Upload the changed files to the same repository. The service worker cache is versioned; when the cache version changes, the old app shell is replaced. If the old version remains visible, close the app, open the site in Chrome, refresh, then reopen the installed app.

## Important

This is an installable web app (PWA), **not a native APK**. GitHub Pages does not compile Android APKs. A separately built and signed APK would require an Android wrapper/build workflow.

Position-size outputs are estimates. Verify contract size, lot minimum and lot step, quote-currency conversion, spread, commission and slippage with the broker before placing a live order.
