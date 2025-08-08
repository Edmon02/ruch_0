# Ruch_0 website

A small multi-page site (Home, Alex, Lusine, Edmon) refactored for responsiveness using Bootstrap 5, with shared global styles and cleaner page markup.

## What changed
- Added global stylesheet: `assets/css/styles.css` (typography, navbar, sections, skills, footer).
- Simplified page-specific CSS (`home.css`, `lusine.css`) to avoid layout conflicts.
- Migrated all pages to a responsive Bootstrap navbar and grid.
- Added a Skills section to each profile page.
- Made maps responsive with Bootstrap's `ratio` utility.
- Consolidated footers and fixed minor content/label issues.

## Files
- `home.html` – Landing page with animated hero background, team links.
- `alexlusine.html`, `lusinealex.html`, `edmon.html` – Profile pages with intro, skills, contact form, and map.
- `assets/css/styles.css` – Shared, site-wide CSS.
- `home.css` – Home page animated background only.
- `lusine.css` – Visual tweaks for profile pages (no fixed layout).

## Run locally
You can open the HTML files directly in a browser, or start a tiny local server:

```bash
# from the project folder
python3 -m http.server 5500
# then open http://localhost:5500/home.html
```

## Edit notes
- Keep shared styles in `assets/css/styles.css`.
- Add any new page-specific overrides in a small page CSS and include it after the shared styles.
- Prefer Bootstrap grid/classes over manual absolute/fixed positioning for responsiveness.
