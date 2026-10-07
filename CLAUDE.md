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
- `index.html`: forwards the root to `/reading-pencil/`.
- `_config.yml` excludes `README.md` and this file from the site.

After a push, wait for the Pages build and check both pages load
(`curl -sI https://threatner.github.io/reading-pencil/privacy/`).
