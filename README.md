# The Day

A small offline-first web app: a daily activity menu sorted by energy level,
a simple log, a twelve-month view, and an appointment summary generator.

Static site — no build step, no server, no accounts. All data is stored in the
browser's own localStorage on the device that entered it. Nothing is uploaded
anywhere, and there is no backend to read it.

## Deploying

Serve the folder as static files. On GitHub Pages: Settings → Pages →
Deploy from a branch → `main` → `/ (root)`.

## Updating

After editing `index.html`, bump the `CACHE` constant at the top of `sw.js`
(e.g. `the-day-v1` → `the-day-v2`). Installed copies will keep serving the old
cached version until that value changes.
