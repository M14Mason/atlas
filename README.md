# ATLAS download site (GitHub Pages)

Static site: hero page + download dashboard. No build step.
- `index.html` : the whole page (detects Mac/Windows/phone and offers the right download)
- `version.json` : version, release notes, file sizes and SHA-256. The ATLAS app checks this file for updates.
- `downloads/` : the three zips (Windows zip is ~32 MB, under GitHub's 100 MB file limit)
- `assets/` : screenshots and icon

Publish: put these files at the root of a GitHub repo named `atlas`, then Settings > Pages > Deploy from branch > main / root.
The site will be at https://m14mason.github.io/atlas/ (the URL the app's update check expects).
New release: replace the zips in downloads/, update version.json (version, notes, bytes, sha256).
