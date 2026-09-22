# Low Fuel Monitoring Dashboard — Static Export

This is a self-contained, framework-free export of the dashboard mockup.
No Claude account, login, or JavaScript runtime is required — it's just
plain HTML/CSS. Any static host works (GitHub Pages, Netlify, S3, a plain
web server, or just opening index.html locally).

Files:
- index.html   → the Fleet Overview page
- detail.html  → the Site Detail page
- logo-icon.png → the logo mark used in the header

## Deploy with GitHub Pages (no git command line needed)

1. Go to https://github.com/new and create a new repository
   (e.g. "low-fuel-dashboard"). Public repos get free Pages hosting.
2. On the new repo's page, click "uploading an existing file".
3. Drag in all three files from this folder (index.html, detail.html,
   logo-icon.png) and click "Commit changes".
4. Go to the repo's Settings tab → Pages (left sidebar).
5. Under "Build and deployment" → Source, choose "Deploy from a branch",
   branch "main", folder "/ (root)", then Save.
6. GitHub will give you a live URL after a minute or two, in the form:
   https://<your-username>.github.io/low-fuel-dashboard/
   That link works for anyone, no Claude or GitHub account required to view it.

## Notes
- The two pages link to each other by relative filename
  (index.html ↔ detail.html), so they must stay in the same folder.
- Fonts load from Google Fonts (fonts.googleapis.com) — the only
  external dependency. Everything else is inline HTML/CSS.
- This is a static mockup: buttons, filters, and dropdowns are visual
  only and don't run any logic.
