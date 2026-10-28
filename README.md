# CycleNourish

Meals that follow your cycle. A single-page app for cycle-synced meal plans, recipes, grocery lists, and nutrition and prenatal logs.

Your data stays on your device and syncs to your own Google Sheet through a Google Apps Script web app. Nothing personal is stored in this repository.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app |
| `favicon.ico`, `icon.svg` | Browser tab icon |
| `apple-touch-icon.png` | iPhone home-screen icon |
| `icon-192.png`, `icon-512.png`, `icon-512-maskable.png`, `site.webmanifest` | Installed web-app icons |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Publish on GitHub Pages

1. Create a repository named `cyclenourish` on GitHub.
2. Upload every file in this folder, including `.nojekyll`, to the repository's main branch.
3. Go to Settings → Pages. Under "Build and deployment," choose **Deploy from a branch**, then **main** and **/ (root)**. Save.
4. After a minute the app is live at `https://<your-username>.github.io/cyclenourish/`.

## Connect your Google Sheet

1. In the sheet, open Extensions → Apps Script and replace the code with `CycleNourish-Sync.gs`. Save.
2. Reload the sheet and choose **CycleNourish → Set up app sync**. Copy the sync key from the App Sync tab.
3. In Apps Script, go to Deploy → Manage deployments → edit → **New version**. Set *Execute as: Me* and *Who has access: Anyone*. Deploy and copy the web app link.
4. In the app, open **Profile → Google Sheet sync**, paste the link and the key, and tap **Connect**.

## Add to your iPhone home screen

Open the app in Safari, tap Share, then **Add to Home Screen**.
