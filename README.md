# GV70 Companion v1.1

An installable, offline-capable Progressive Web App for the 2023 Genesis Electrified GV70. Vehicle readings are **manual**, not live. Remote controls are disabled.

## Upgrade your existing GitHub Pages site (Pixel 7 Pro)

1. Extract `GV70_Companion_v1_1.zip` in Files by Google.
2. Open your existing GitHub repository in Chrome (not the GitHub Android app).
3. Use **Add file > Upload files**. Upload the seven files **inside** the extracted folder to the repository **root**, not the folder itself. Existing `index.html`, `README.md`, and `icon.svg` should be replaced by the new versions. Commit changes to `main`.
4. Keep Settings > Pages configured to deploy `main` and `/ (root)`.
5. After the Pages deployment completes, open your original GitHub Pages URL in Chrome and refresh. The heading will say `v1.1`.
6. In Chrome menu, choose **Add to Home screen > Install**. Remove the old shortcut after confirming the new app works.

## Important

The app uses the **same origin and localStorage key** as v1, so existing battery/range values and charging logs should persist if you update the same repository and open it in the same Chrome profile. However, browser storage is not a reliable backup. Export charging history before upgrading; snapshot values can be noted manually.

The PWA requires HTTPS, a valid manifest, PNG icons and a registered service worker. Chrome's install behavior varies by version. If install is not offered, confirm all files are in the root, refresh the page, and wait for the new service worker to activate.

Offline access is available after the app has loaded online and its assets are cached. The app does not contact Genesis or upload your vehicle data. Clearing site storage may erase it. No credentials should be committed to public GitHub.
