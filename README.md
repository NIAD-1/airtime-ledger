# Market Ledger

Offline-first airtime inventory and sales app for MTN, Zain, Glo, and Etisalat.

## Install on her laptop

1. Publish the site with the GitHub Pages workflow and open its HTTPS address in Chrome while online.
2. In Chrome, choose **Install page as app** (or use the install icon in the address bar).
3. Open the installed app and create a local username and password.
4. Add purchase and sales records. The app encrypts its saved ledger in this Chrome profile and works offline after the first visit/cache.

## Local storage and login

There is no Firebase or cloud account. The username and password exist only on this laptop. The password derives an encryption key for the saved ledger; the password itself is not saved. The installed PWA and Chrome share the same local site storage when used in the same Chrome profile.

If the password is forgotten, the encrypted ledger cannot be recovered. Export a backup regularly from **Settings** and keep it somewhere safe. Backup exports are ordinary JSON files and are not encrypted by the app.

## Publish with GitHub Pages

The `main` branch workflow deploys the static site files. In the repository, set **Settings → Pages → Build and deployment → Source** to **GitHub Actions**. The app files do not include customer or transaction records.
