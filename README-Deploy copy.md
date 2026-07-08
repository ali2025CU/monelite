# Monelite Web — Deploy to GitHub Pages (no coding, ~10 minutes)

## What you're deploying

6 files: `index.html` (the entire app), `manifest.json`, `sw.js` (offline support), and 3 icon PNGs (your Design 3 logo). No expiry, no Mac needed after setup, $0 forever.

## Step 1 — Create a GitHub account

Go to **github.com** → Sign up (free). Skip if you have one.

## Step 2 — Create the repository

1. Click the **+** (top right) → **New repository**.
2. Name: `monelite` · visibility: **Public** (required for free Pages; the page URL is obscure and your financial data is NOT in these files — data lives only on your phone).
3. Check **"Add a README file"** → **Create repository**.

## Step 3 — Upload the app files

1. In your new repo, click **Add file → Upload files**.
2. Drag all 6 files from this folder in.
3. Click **Commit changes**.

## Step 4 — Turn on GitHub Pages

1. Repo → **Settings** tab → **Pages** (left sidebar).
2. Under "Build and deployment": Source = **Deploy from a branch**, Branch = **main**, folder **/ (root)** → **Save**.
3. Wait ~1 minute, refresh — you'll see your URL:
   `https://YOUR-USERNAME.github.io/monelite/`

## Step 5 — Install on your iPhone

1. Open that URL in **Safari** on your iPhone.
2. Tap **Share** (square with arrow) → **Add to Home Screen** → Add.
3. Done. Full-screen app, your logo, works offline, never expires.

## Using it

- Same layout as the native app: Dashboard / Expenses / Wishlist / Debts / Savings tabs; Income, Categories, Review, and Backup live behind the chips on the Dashboard.
- **Wishlist verdicts** come from the rule engine instantly (works offline).
- **Debt reminders:** Dashboard → Backup → "Debt due dates → Calendar" downloads an .ics file; open it and add to your iPhone Calendar. Calendar then reminds you 3 days before each due date, every month.
- **Back up monthly:** Dashboard → Backup → Export. Browser data survives normal use but is wiped if you ever clear Safari website data — a backup file makes that a non-event. Import restores everything.

## Updating the app later

When I give you a new `index.html`: repo → click the file → pencil icon → paste → Commit. Also edit `sw.js` and change `monelite-v1` to `v2` so phones fetch the update. Changes appear within a couple of minutes; reopen the app twice to see them.

## Moving from the native app

The iPhone app and web app store data separately. If you've built up real data in the native app, tell Claude — a small export feature can be added to the iOS app to carry it over.
