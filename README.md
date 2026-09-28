# Stop The Split — Tactical Voting Guide

Static site (no build step). Data: YouGov Westminster MRP, 24 Sept 2026.

## Files (all must sit in the repo root)
- `index.html` — main tool: constituency search, full table, "How this works" Q&As. Contains the AdSense loader script in `<head>`.
- `about.html`, `support.html`, `privacy.html` — the other pages.

## Updating the live site
1. GitHub repo → Add file → Upload files → drop in the changed files (same names) → Commit changes.
2. Netlify redeploys automatically (check the Deploys tab). Hard-refresh your domain to see it.

## AdSense to-do
- Applied/ID: ca-pub-4066582419214843 (loader script already in index.html).
- After approval: add the `ads.txt` line Google gives you (a file named `ads.txt` in the repo root).
- Set up Google's certified consent message (AdSense → Privacy & messaging) for UK/EEA visitors.
- If you enable Netlify Analytics / Real User Monitoring, update privacy.html first.
