# Ninefold site

Landing page for Ninefold, a free collection-tracking app for the Riftbound trading card game. Hosted on GitHub Pages at [ninefold.gg](https://ninefold.gg).

## Files

- `index.html` - the page, with all CSS inline. No build step. Its header carries the brand mark from `brand/mark.html`.
- `CNAME` - custom domain for GitHub Pages.
- `riot.txt` - empty placeholder for Riot Games domain verification.
- `404.html` and `b/index.html` - the shared binder page, rendered from the app repo ([seanfoleydesigns/ninefold](https://github.com/seanfoleydesigns/ninefold), `site/shared-binder.html`, through `npm run site:render`). Do not edit them here; change the source in the app repo, re-render, and copy the files across. GitHub Pages serves `404.html` for `https://ninefold.gg/b/<token>`, and `b/index.html` answers `https://ninefold.gg/b/?t=<token>`.
- `brand/` - the brand mark from the same render: `favicon.svg`, `favicon.png` (32px), and `mark.html`, the inline `<svg class="mark">` snippet (the 9 in `currentColor`, the tip in teal). Do not edit here either; the source is `assets/brand` in the app repo.

## Publishing

Push to `main`. In the repository settings, enable GitHub Pages from the `main` branch root and point the `ninefold.gg` DNS records at GitHub Pages.

Ninefold was created under Riot Games' "Legal Jibber Jabber" policy using assets owned by Riot Games. Riot Games does not endorse or sponsor this project.
