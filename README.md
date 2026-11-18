# VO2max + weight-loss plan (phone log)

A free, static page for logging your 12-week running and cycling plan. No server, no account.

## Put it on GitHub Pages
1. On github.com click **New repository**, name it (e.g. `vo2max-plan`) and create it.
2. Click **Add file > Upload files**, drag in everything in this folder (`index.html`, `manifest.webmanifest`, `sw.js`, both `icon-*.png`, `README.md`) and commit.
3. Go to **Settings > Pages**, set **Source** to *Deploy from a branch*, choose branch `main` and folder `/ (root)`, then Save.
4. After a minute your page is live at `https://YOUR-USERNAME.github.io/vo2max-plan/`.
5. On your phone open that link, then **Add to Home Screen** (Safari: Share menu; Chrome: three-dot menu). It then opens like an app and works offline.

## Your data
- Sessions and weights are saved **in your phone's browser only**. They are not uploaded to GitHub, so a public repo does not expose them.
- They don't sync between devices. Use **Backup** (downloads a .json) and **Restore** to move them, and **Download CSV** to paste into the Excel workbook.
- Clearing the browser's site data erases the log, so back up regularly.

## Changing the start date
Open `index.html` and edit this line near the top of the script (months count from 0, so November is 10):
`const S=new Date(2026,10,16)`
It must be a Monday. Session text is baked in from the workbook; ask Claude to regenerate the page if you change the plan.
