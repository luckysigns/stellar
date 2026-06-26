# Stellar — project context

Single-file astrology web app. Read this before editing anything.

## What it is
- Personal astrology dashboard: daily readings, lucky days, monthly/yearly horoscopes, an astrocartography map (Atlas), a natal chart, a live tri-wheel, tarot, and chart-to-chart comparison (synastry).
- Everything is computed client-side. No backend, no database, no build step.

## Architecture / conventions (do not break these)
- **One file.** The whole app is `index.html` (delivered/worked on as `stellar.html`, then renamed to `index.html` in the repo). Vanilla JS, no framework, no bundler. All HTML, CSS, and JS live in that single file.
- **Ephemeris:** uses Astronomy Engine, loaded via CDN. All planet positions and chart angles come from it.
- **Output convention:** when editing, always return the complete working file, not a diff or a fragment.
- **Style:** casual tone in code comments and UI copy. No em dashes anywhere.
- **Always verify changes** (syntax-check the JS, sanity-check any math) before presenting.

## Key data structures & helpers
- **Multi-profile system.** Each profile = `{id, name, date, time, lat, lng, tzOffset, placeName}`. `profiles` array + `activeId` + `profile` (the active one). Persisted to localStorage.
- `buildBirthDate(profile)` → the UTC birth instant.
- `computeChart(date)` → `{planetKey: eclipticLongitude}` for all planets.
- `computeAngles(date, lat, lon)` → `{asc, mc, cusps}` in ecliptic-longitude degrees.
- `computeChartData()` fills `cachedNatal` + `cachedAngles`, stamps `_cacheProfileId`.
- `eclipticLon(body, date)`, `signFromLon(lon)` → `{sign, glyph, index, degInSign}`, `norm360`, `gmstDeg(jd)`, `julianDay(date)`, `posLabel(lon)`.
- `drawWheelInto(svgId, natal, angles)` draws a chart wheel; used by BOTH the natal wheel and the dashboard "sky now" wheel.
- `drawTriWheel(...)` draws the three-ring natal/progressed/transit wheel; it ticks live every second via `startTriWheelLive` / `stopTriWheelLive`.

## Pages / views
- **Onboard** → enter birth details.
- **Natal page** (`#natal`) → birth chart wheel + summary + an in-depth report that includes the live tri-wheel.
- **Dashboard** (`#dash`) → tabs: Today / Lucky days / Month & Year / Atlas. Atlas is the astrocartography map and lives as a TAB inside the dashboard; it must never replace or hide the rest of the app.

## Astrocartography (Atlas) — keep the math
- For each of 10 natal planets, four world lines (MC/IC/AC/DC) on an equirectangular map (lon -180..180 → x 0..360, lat 90..-90 → y 0..180).
- RA/Dec from `Astronomy.GeoVector(body, date, true)` (equator-of-date). MC line = meridian at lon = RA - GST; IC = MC+180; AC/DC = horizon curves where cos(H) = -tan(lat)*tan(Dec). Curves split at the dateline and circumpolar gaps.
- This math is verified correct. Do not change it. The map has filter chips (all + one per planet), tap-a-line-to-focus, a fullscreen overlay with pinch/scroll zoom + drag pan + reset, and power-spot crossings shown only on the "all" tab.

## Owner's reference chart (the correct one)
- 27 July 1994, 1:32 PM (13:32), Brisbane, Queensland, Australia. lat -27.47, lon 153.02, UTC+10, no DST.
- True angles: **Ascendant 14°24′ Sagittarius, Midheaven 28°30′ Leo.**
- Note: an old astrocartography PDF report was generated for 2:32 PM (one hour late), so its line positions are shifted ~15° of longitude east of the real chart. The PDF is wrong, the app is right. Use the PDF only for interpretive text/structure, never for exact line positions.

## Deploy
- Repo: `luckysigns/stellar`. Live at `stellar-three-phi.vercel.app`.
- Deploy = replace `index.html` in the repo (the working file is named `stellar.html`, rename it to `index.html`). Vercel auto-redeploys on push.
- After deploy, hard-refresh or use a private window to beat the browser cache.

## Repo layout
- `index.html` — the entire app (this is what ships)
- `CONTEXT.md` — this file
- `README.md`
- `package.json`, `vercel.json` — minimal config
- `assets/`, `data/`, `docs/`, `samples/` — supporting folders

## Gotchas
- Don't upload/edit a stale copy. The deployed `index.html` is the source of truth — start from it.
- The dashboard "sky now" wheel needs a location to compute angles; it falls back to the birth location if no separate "now location" is set.
- Don't run two tools editing the same file at once (e.g. a chat session and Claude Code) — you'll get conflicting versions.
