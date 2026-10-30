# Market Ledger

An offline-first airtime card inventory and sales ledger for MTN, Zain, Glo, and Etisalat.

## Run locally

Open `index.html` in a browser. The app stores its records in that browser on that device. Use **Settings → Download backup** regularly to keep a backup.

## Publish with GitHub Pages

This repository includes a GitHub Actions workflow that publishes the static app whenever code is pushed to the `main` branch.

1. Create a GitHub repository and push these files to its `main` branch.
2. In the repository, open **Settings → Pages**.
3. Set the build and deployment source to **GitHub Actions**.
4. Open the **Actions** tab and wait for **Deploy static app to GitHub Pages** to finish.
5. GitHub will show the site address in the workflow deployment and Pages settings.

## Data and privacy

GitHub Pages hosts the app's static files publicly. Sales, purchase, customer, and inventory records are saved locally in the browser's storage; this app does not upload them to GitHub. Keep the records on the trusted laptop, do not commit backup files, and use the app's backup export to keep a separate copy.

The service worker caches the app shell for offline use after its first successful visit. The hosted app needs an internet connection for its first load and deployment updates.
