# English Grammar Quest — Mobile App Starter

A self-contained C2 English grammar game with 8 worlds, 40 original multiple-choice questions, explanations, XP, streaks, unlocks, mixed practice, and locally saved progress.

## Quick preview
Open `www/index.html` in a browser. For PWA installation and service-worker caching, serve the `www` folder over HTTPS or localhost.

## Android packaging (requires a computer)
1. Install Node.js LTS and Android Studio with the Android SDK.
2. Extract this folder and open a terminal in it.
3. Run:
   ```bash
   npm install
   npx cap add android
   npx cap sync android
   npx cap open android
   ```
4. In Android Studio, test on an emulator and at least one real device.
5. Create a signed Android App Bundle (AAB) using **Build → Generate Signed Bundle / APK → Android App Bundle**.
6. Upload the AAB to a Google Play Console account, complete the app content, privacy, target audience, data safety and testing requirements, then submit for review.

## Important
This starter project is not published and does not contain a signed APK/AAB. Store publication requires the developer to own and complete the relevant developer account, app listing, declarations, signing and review process. Before release, test offline behavior, accessibility, device layouts, and data persistence; consider adding a privacy policy and analytics only if needed. The game currently stores progress locally on the device and does not require an account or send gameplay data to a server.

## Project structure
- `www/index.html` — game UI and question bank
- `www/manifest.webmanifest` — installable web-app metadata
- `www/sw.js` — offline caching
- `www/icon.svg` — app icon source
- `capacitor.config.json` — Capacitor wrapper configuration
