# threatner.github.io: instructions for Claude

Public pages for threatner's projects, served by GitHub Pages (Jekyll). Today:
Reading Pencil's help page (`reading-pencil/index.md`) and privacy policy
(`reading-pencil/privacy.md`), linked from its Chrome Web Store listing.

## Rules

1. **This repo is public, history included.** Commit only as
   `threatner <86233333+threatner@users.noreply.github.com>` (GitHub's no-reply
   address). Check with `git config user.email` before every commit; never
   commit with a personal email.
2. **No email address on any page.** The contact is @threatner_ on X
   (https://x.com/threatner_).
3. **It must stay public**: GitHub Pages on a free account only serves public
   repos, and the store listing's privacy and support links point here.
4. `reading-pencil/privacy.md` is a copy of `PRIVACY.md` from the (private)
   `threatner/reading-pencil` repo, with front matter on top. Change the
   policy there first, then copy it here; never edit only one of them.
5. Plain words for readers who aren't technical; no em dashes.
6. Nothing goes out (push, publish) without the owner's yes.

## Layout

- `_layouts/page.html`: the one page design (paper look, the pencil logo).
- `index.html`: the home page, one card per extension (Reading Pencil, SnapTabs),
  standalone (not the Reading Pencil layout); `icons/` holds SnapTabs' icon.
- `googlee16cd5b2f22df300.html`: Google Search Console's ownership file, which
  makes this site the verified Official URL on both store listings. Never
  delete it (Google re-checks it).
- `_config.yml` excludes `README.md` and this file from the site, and turns
  on `jekyll-seo-tag` (`{% seo title=false %}` in each page's head: its
  description, canonical address and share card) and `jekyll-sitemap`
  (`/sitemap.xml`, submitted in Search Console). Every page shares
  `reading-pencil/share.png` (1200×630, drawn by the extension repo's
  `npm run store`) unless its front matter names another `image`.
- `reading-pencil/pdf.md`: "A reading ruler for PDFs", one page per
  question people search for (research in the extension repo,
  `docs/research/store-seo-2026-10-15.md`). Keep it true of the current
  build, like the help page.
- Every link to a Chrome Web Store listing carries UTM tags
  (`?utm_source=threatner.github.io&utm_medium=website&utm_campaign=<where>`,
  written `&amp;` in HTML): `home`, `help-page`, `footer`, `goodbye`. The
  Developer Dashboard's Impressions tab shows store page views by them.
  Nothing on this site tracks anyone; tag any new store link the same way.

After a push, wait for the Pages build and check both pages load
(`curl -sI https://threatner.github.io/reading-pencil/privacy/`).
