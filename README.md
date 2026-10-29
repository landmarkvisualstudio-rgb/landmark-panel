# Landmark Estate Films panel

Single-page panel (Persian/English) for leads, cold outreach, projects and payments.
No server, no build step: `index.html` is the whole app (PWA, works offline).

## Use
- Open the GitHub Pages URL on laptop or phone, then "Add to Home Screen / Install".
- **Download**: Settings → Backup → "Save updated copy with data" produces one self-contained HTML file.
- **Data is NOT in this repo.** On first run import `landmark-seed-data.json` (Settings → Backup → Restore JSON).

## Device sync (private GitHub Gist)
1. Create a *classic* token with only the `gist` scope: https://github.com/settings/tokens/new?scopes=gist
2. First device: Settings → Device sync → paste token → "Create new sync space".
3. Other devices / teammates: first device → "Show connect code", paste it on the other device → "Connect".
Data lives in a secret Gist of the account that owns the token; each device merges by last-edit time and syncs every minute and after each change.
Treat the connect code like a password (it contains the token).
