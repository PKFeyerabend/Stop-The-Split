# Stop The Split — Tactical Voting Guide

A small static site that shows, for every GB parliamentary constituency, whether
Reform UK is a close contest and — if so — which other party is best placed to
beat them, based on YouGov's Westminster MRP model (published 24 Sept 2026).

## Files
- `index.html` — the main tool (constituency search + full results table)
- `about.html` — an about/contact page (edit the placeholder sections with your details)

## Deploying
Both files are fully self-contained static HTML (no build step, no server-side code).
Any static host works: GitHub Pages, Netlify, Vercel, Cloudflare Pages, or a plain
web server — just upload the two files.

### GitHub Pages, quickest path
```bash
git remote add origin <your-empty-github-repo-url>
git branch -M main
git push -u origin main
```
Then in the repo's Settings → Pages, set the source to the `main` branch, root folder.

## Google AdSense
Two placeholder ad slots are marked in `index.html` (search for `AD SLOT`), plus a
comment in the `<head>` showing where the AdSense loader script goes. AdSense needs
to review your live domain before ads will actually serve — the placeholders don't
do anything until you paste your own ad unit code in.

## Data sources
See the "How this works, and its limits" section on the page itself — every figure
links back to its source (YouGov MRP, YouGov tactical voting survey, PollCheck).
