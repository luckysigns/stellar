# Stellar

Daily astrology readings from a real natal chart. Static frontend + one Vercel serverless function that proxies to Anthropic so your API key stays server-side.

## Structure

```
stellar/
  index.html        the whole app (chart math, wheel, lucky timing, UI)
  api/reading.js    serverless proxy -> Anthropic (holds your key)
  vercel.json       function config
  package.json      ES module flag
```

## Deploy (two ways)

### A. Vercel CLI (fastest)
```bash
npm i -g vercel        # if you don't have it
cd stellar
vercel                 # first run: link/create the project, accept defaults
vercel env add ANTHROPIC_API_KEY    # paste your key, choose Production (and Preview)
vercel --prod          # deploy to the live URL
```

### B. GitHub + Vercel dashboard (matches your usual flow)
1. Make a repo (e.g. `github.com/luckysigns/stellar`) and push these files.
2. In Vercel: New Project -> import the repo -> Framework Preset = "Other" -> Deploy.
3. Project -> Settings -> Environment Variables -> add `ANTHROPIC_API_KEY` = your key (Production + Preview) -> redeploy.

That's it. The frontend calls `/api/reading`; the function adds the key and model and returns just the text.

## Get an API key
console.anthropic.com -> API Keys -> Create Key. Paste it into the env var above. Never put it in `index.html` or commit it.

## Local testing
```bash
cd stellar
vercel dev             # runs the function + static site at localhost:3000
```
Plain `open index.html` won't power readings (no function), but the chart, transits, and lucky windows all work offline.

## Cost note
Each reading is one Sonnet call (~1–1.5k output tokens). For friend-testing that's pennies. If you want to cap spend, add a simple per-IP rate limit in `api/reading.js` or set a usage limit on the key in the Anthropic console.

## What's accurate
- Planet positions: Astronomy Engine (real ephemeris), validated against a reference chart.
- Ascendant / Midheaven / Placidus house cusps: validated to <1° against Cafe Astrology.
- Lucky timing: Midheaven-anchored, weighting benefics (Jupiter/Venus) to the MC and natal Venus.
