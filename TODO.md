# Follow-ups

Flagged during the site audit/upgrade pass — not urgent, revisit when convenient.

- **Google Maps API key exposed in `config/_default/params.toml`** (`map_api_key`). Currently unused (`map = 2` selects OpenStreetMap instead), but it's sitting in plaintext in a public GitHub repo. Confirm whether it's actually a live key of yours — if so, rotate/restrict it in Google Cloud Console and scrub it from git history; if it's not yours or already dead, just delete the line.
- **`googleAnalytics = "#####"` is a dead placeholder** in `config/_default/hugo.toml`. It also sits in the wrong config location to ever work (the theme reads `site.Params.GoogleAnalytics`, not the top-level key), so it's currently inert either way. Decide: wire up real analytics (move it under `[params]`) or delete the placeholder line.
- **Disqus is configured with the theme vendor's demo shortname** (`themefisher-template` in `config/_default/hugo.toml`), not a real account. It's currently disabled on the only page that would show it (privacy policy), but fix the shortname before enabling comments/blog posts anywhere else — otherwise any comments posted go to the theme vendor's forum, not you.
- **Orphaned images in `static/img/`**: `user.jpg` and `user-full-2.jpg` aren't referenced anywhere in content, but still get deployed to production. Decide whether to keep (for future use) or delete.
- **No custom HTTP security headers** (CSP, X-Frame-Options, etc.) — GitHub Pages doesn't support setting these at all. Not fixable without switching hosts; low priority for a static portfolio with no login/user data.
- **Bootstrap 4 → 5 upgrade**. `package.json` declares `bootstrap ^4.3.1`, but the theme actually vendors its own Bootstrap 4 source directly (`themes/academia-hugo/assets/sass/vendor/bootstrap`), built on Bootstrap 4 conventions throughout. Upgrading would be a real theme-wide rewrite, not a quick bump — only worth it alongside a bigger redesign push.
