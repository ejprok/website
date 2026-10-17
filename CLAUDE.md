# CLAUDE.md

Personal website for EJ Prokopik (ejprok.com): part portfolio, part just for fun. Hosted as static files (see `CNAME`), deployed from `main`.

## Principles

- **Simple and ultra lightweight above all.** Plain hand-written HTML, no build step, no framework, no package manager.
- **Avoid JS and CSS when possible.** Not never, just sparingly. Reach for semantic HTML first; add CSS only when HTML can't do it, and JS only when there's no other way. Keep any JS inline and tiny, with no libraries.
- No external fonts, trackers, CDNs, or images unless there's a good reason. Pages should stay a few KB.
- Keep the monospace, minimal look. Prefer less over more when in doubt.

## Layout

- `index.html`: home page
- `main.css`: the one shared stylesheet (light and dark mode via `prefers-color-scheme`; warm off-white and warm charcoal)
- `apps/`: per-app pages (`dothis/`, `quadratic/`, `app-support.html`)
- `blog/`: blog posts
- `my-configs.html`: personal configs page

## Working here

- Preview by serving the folder (`python3 -m http.server 8000`); opening files directly doesn't load `main.css` in the in-app browser.
- Check changes in both light and dark mode.
- Commits go straight to `main` when asked; there's no CI.
