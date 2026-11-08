# GV70 Companion v1

A phone-first progressive web app for a 2023 Genesis Electrified GV70. It does not connect to the car. Vehicle values are entered manually. Charging sessions and costs are saved in browser localStorage, with CSV export.

## Publish with GitHub Pages (phone only)
1. Create a new **public** GitHub repository named `gv70-companion`.
2. Upload the four files in this folder to the repository root (not inside a subfolder).
3. Open repository **Settings > Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`, then save.
4. Once deployment completes, visit `https://YOUR_USERNAME.github.io/gv70-companion/` in Chrome on Android.
5. Open Chrome menu and choose **Add to Home screen** or **Install app**.

No secrets or Genesis account credentials should be committed to the repository. Public GitHub Pages is suitable only for this local-data prototype. Data entered into the app stays in the phone browser storage; the source code is public. Clearing site storage may delete data.

## Notes
- Rates are manually entered in USD/kWh.
- Charging cost is energy × rate, excluding additional fees and charging losses not included in entered energy.
- Remote control buttons are disabled because there is no authenticated vehicle API integration.
