
## Daily new leads
Each batch comes as a small JSON file (`leads-YYYY-MM-DD.json`, same format as the seed: `{"leads":{"<id>":{...}}}`).
Import it once on any device: Settings → Backup → "Restore or add leads from JSON file".
Existing leads (and their stage/notes) are never overwritten by an older copy; sync then spreads the new leads to all devices.

## Automatic lead batches (v22+)
`leads.json` in this repo holds the latest published leads. The app checks it on start and every 30 minutes,
adds any lead it has not seen before (never re-adds one you deleted), then sync spreads them to all devices.
