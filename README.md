# SAPTECHS — company site

One self-contained HTML page, served by GitHub Pages from `main`, root folder,
at https://saptechs.co.in.

## Editing

Never edit this repository by hand. The page is generated from the source in the
private `UniverseIt` repository, at `docs/saptechs-site/`:

- `index.html` — the page
- `build-standalone.py` — wraps it in a full HTML document and writes everything here

After editing the source, run `python3 build-standalone.py` and copy the whole of
`dist/` over this repository (it includes `CNAME` and `.nojekyll`).

## Old paths

`careers.html`, `contact.html` and `kirikit-cricket-app.html` forward links from the
former GoDaddy site to the matching section of the page.

## Custom domain

`CNAME` holds `saptechs.co.in`. DNS at GoDaddy: four `A @` records to
185.199.108.153–111.153 and `CNAME www` to `saptechs-private-limited.github.io`.
Leave the MX and TXT records alone — company mail depends on them.
