# Snohomish EMS Study — PWA

A Progressive Web App converted from the native SwiftUI study app. It is designed for iPhone Safari and can be installed with **Share → Add to Home Screen** after it is hosted on HTTPS.

## Included
- Full searchable protocol library from the supplied V7 education draft
- Medication formulary with indications, contraindications, routes, administration/dosing, and notes
- Dose drills
- Protocol recall drills
- Protocol-recognition scenarios
- Spaced-repetition scheduling
- Favorites and progress stored locally on the iPhone
- Offline caching after first successful load
- Weight conversion practice tool

## Important
The supplied source PDF is explicitly marked EDUCATION DRAFT ONLY / NOT FOR PATIENT CARE. This application repeats that status and must not be used as an approved clinical reference.

## Deploy without a Mac
The app is static HTML/CSS/JavaScript. Upload this folder to any HTTPS static host such as GitHub Pages, Cloudflare Pages, Netlify, or similar. No server database is required.

Once deployed, open the HTTPS site in Safari on the iPhone, tap Share, then Add to Home Screen. Open it once while online so the service worker can cache all app files for offline study.


## v1.1 GitHub Pages fix
Runtime study data is embedded in `app.js`, so the app no longer depends on separate JSON fetches. A `.nojekyll` file is included for static GitHub Pages deployment. Replace all existing repository files with this version, then hard-refresh/reopen the installed app.
