# VA151-ACF Charlottesville Virginia — Chapter Website

Static website for VA151-ACF Charlottesville Virginia, a chapter of the American Culinary Federation. Hosted free on GitHub Pages.

## Structure

| Path | What it is |
|---|---|
| `index.html` | Public **Coming Soon** page (what visitors see at the domain today) |
| `preview/index.html` | Full site in progress — reachable at `/preview/`, hidden from search engines |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |
| `CNAME` | Custom domain (added once GitHub Pages is pointed at the domain) |

## Going live with the full site

When the full site is ready to replace the Coming Soon page:

1. Move `preview/index.html` to `index.html` (overwriting the Coming Soon page)
2. Remove the `<meta name="robots" content="noindex, nofollow">` line from it
3. Commit and push — GitHub Pages redeploys within a minute or two

## Sections currently hidden (commented out in the full site)

- **Events** — re-enable once events are scheduled
- **News** — re-enable once certifications and events get rolling

Search the file for `<!--` to find them; remove the comment markers to bring them back.

## Planned additions

- `events/events.json` — table-driven events calendar
- `blog/` — one markdown file per post
- `gallery/gallery.json` + `gallery/photos/` — photo gallery (compress images to ~1600px wide before adding)
