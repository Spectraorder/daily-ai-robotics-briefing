# Daily AI Robotics Briefing

A daily briefing on AI, robotics, VLA (vision-language-action) models, and world models — new arXiv papers, hot discussions, and podcast updates.

**Read it here:** https://spectraorder.github.io/daily-ai-robotics-briefing/

Updated every day at 2:00 PM ET. Published automatically via GitHub Pages from the `main` branch.

## How the site is organized

- `reports/YYYY-MM-DD.md` — one Markdown file per issue. Each file holds that day's full briefing: a `#` title line, then `## Papers`, `## Hot Discussions`, and `## Podcast Updates` sections, with paper images referenced from `../assets/`.
- `reports/index.json` — the issue manifest, newest first: `[{"date": "2026-10-19", "title": "Daily AI Robotics Briefing — October 19, 2026"}, ...]`. The sidebar is built from this file.
- `index.html` — a lightweight shell (Poppins, blue/orange/purple section styling, week-grouped sidebar). It loads the manifest, builds the archive navigation grouped by week, fetches the selected day's Markdown file, and renders it in the browser. `#/YYYY-MM-DD` in the URL selects an issue; the latest issue loads by default.
- `assets/` — paper images referenced by the reports.
- `favicon.svg` — the site icon.

## Adding a new issue

1. Add `reports/YYYY-MM-DD.md` for the new day (same section structure as existing reports).
2. Prepend `{"date": "YYYY-MM-DD", "title": "Daily AI Robotics Briefing — <Month D, YYYY>"}` to `reports/index.json`.
3. Commit and push to `main` — GitHub Pages republishes automatically.
