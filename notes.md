# World Cup Tracker — Project Notes

## Status
- 2026 tournament: **complete**
- Netlify site: **deleted** (Sept 2026)
- GitHub repo (tlorents/world-cup): **deleted** (Sept 2026)
- Next deploy: **Vercel** (same single-file approach)

## ESPN Links Issue
All ESPN match/player links went dead after the 2026 tournament ended.
ESPN uses dynamic routing tied to live tournament state — once the event closes, those URLs 404.

**Fix for next time:** At the end of the tournament (finals day), do a Save As → complete webpage or manually snapshot each ESPN link to its final destination URL. Don't rely on ESPN's live routing surviving off-season.

## Reuse Plan for 2030
The code is reusable as-is. Steps for next tournament:

1. Open `index.html` locally and update:
   - Team names, flags/images, group assignments
   - Match schedule and results as games are played
   - Scorers, stats, any embedded data
2. Replace player images (currently `spainplayer.png`, `argentinaplayer.png`)
3. Snapshot ESPN/external links before the tournament ends
4. Connect repo to Vercel for deploy (no config needed for static HTML)

## Local Files
- `index.html` — main site, all-in-one
- `spainplayer.png`, `argentinaplayer.png` — player images from 2026 final

## Lesson Learned
> "Save the site as dynamic as soon as the world cup is over" — meaning freeze/snapshot all external links and live data at tournament close, before they go stale.
