# Sheetly: legal & support pages

Static site with Sheetly's [Privacy Policy](privacy.html), [Terms of Use](terms.html), and [Support](support.html) pages, plus a small [landing page](index.html).

No build step: plain HTML with inline CSS, all links relative. To publish: push this folder to its own GitHub repo and enable **Settings → Pages → Deploy from branch** (main, root). The pages will be live at `https://<user>.github.io/<repo>/privacy.html` etc.

Before launch, replace the placeholder App Store link in `index.html`.

## Keeping the mirror in sync

The policies live at www.trysheetly.com (repo loveranmar/sheetly-site). Edit `site/privacy.html` and
`site/terms.html` there first, then regenerate this mirror with `python3 mirror.py /path/to/site` (default
`../site`) and commit. `support.html` has its own layout here and is updated by hand.
