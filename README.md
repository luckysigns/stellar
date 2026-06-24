# Stellar

Daily astrology readings from a real natal chart. 100% client-side — no API, no key, no billing. Just static files.

## Files
- `index.html` — the whole app (chart math, wheel, lucky timing, readings, UI)
- `vercel.json` / `package.json` — minimal config

## Deploy
Drop the folder on any static host. For Vercel: import the repo, Framework Preset "Other", Deploy. No environment variables needed.

To update after a change: re-upload `index.html` (or push to the connected repo).

## What it does
- Planet positions from a real ephemeris (Astronomy Engine), validated against a reference chart.
- Ascendant / Midheaven / Placidus houses, validated to <1° against Cafe Astrology.
- Natal + daily readings assembled from a built-in interpretation library (no AI service).
- Lucky timing anchored to the Midheaven, weighting benefics (Jupiter/Venus) to the MC and natal Venus.

Everything runs in the browser. Works offline once loaded.
