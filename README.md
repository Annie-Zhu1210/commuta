# Commuta — Exhibition site

A four-page static site for the Commuta project: a portable IoT air quality monitor for the London Underground. MSc Connected Environments dissertation, CASA, UCL, 2026.

## Pages

- `index.html` — Home (what the QR code points to)
- `device.html` — Hardware, PCB, enclosure, BLE
- `app.html` — Companion app features
- `about.html` — Dissertation, aim, GitHub link
- `styles.css` — Shared stylesheet

Fonts are loaded from Google Fonts (Fraunces, Inter, JetBrains Mono). No build step, no framework, no dependencies.

## Deploy to GitHub Pages (5-minute version)

1. Create a new public repo on GitHub, e.g. `commuta-site` or `commuta`.
2. Upload every file in this folder to the repo root (drag-and-drop in the GitHub web UI works fine).
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, select **Deploy from a branch**.
5. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
6. Wait 1–2 minutes. Your site will be live at `https://<your-username>.github.io/<repo-name>/`.

That URL is what you'll turn into the QR code. It won't change when you edit content later, so it's safe to submit tomorrow and keep refining the page all week.

## Custom domain (optional, later)

If you eventually want a shorter URL like `commuta.io`, GitHub Pages supports custom domains via a `CNAME` file — not needed for the exhibition.

## Editing content

Everything is plain HTML with clearly-named sections. To swap in real photos:

1. Add image files to an `images/` folder in the repo.
2. Find the `<div class="media …">` blocks in the HTML and replace them with `<img src="images/your-photo.jpg" alt="…" />`.
3. Commit and push — GitHub Pages redeploys automatically in about a minute.

## Structure and placeholders

Placeholder blocks are marked `coming soon` or wrapped in `<em>— Placeholder —</em>` comments so they're easy to find and replace.

Real content is on the Home page. Device / App / About pages have the correct structure but need photos and, on the About page, your personal bio.