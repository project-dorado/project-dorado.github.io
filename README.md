# project-dorado.github.io

The Dorado organization website, served at **[dorado.org.uk](https://dorado.org.uk)**.

A hand-crafted static site — no build step, no framework. GitHub Pages publishes
straight from the `main` branch (legacy branch deployment).

## Structure

```
.
├── index.html               # landing page
├── projects/                # one page per project
│   ├── dorado.html
│   ├── dorado-hd.html
│   ├── dorado-emu.html
│   └── dorado-cloud.html
├── about/index.html         # mission, canon, licensing, acknowledgements
├── 404.html
├── assets/
│   ├── css/site.css         # Zune "Metro" design tokens + layout
│   ├── js/site.js           # mobile nav + reveal-on-scroll (no dependencies)
│   └── img/                 # brand marks, banner, favicon, social image
├── CNAME                    # dorado.org.uk
├── sitemap.xml · robots.txt
└── .nojekyll
```

## Deploying

Pages is configured for **branch deployment** from `main` at the repository root.
Pushing to `main` republishes the site. The custom domain is declared in `CNAME`
and configured in **Settings → Pages**; HTTPS is enforced there.

## Editing

All pages share the same header, footer and design tokens. To add a project page,
copy an existing `projects/*.html`, update the masthead, and add a card to
`index.html` plus an entry to `sitemap.xml`.

Brand palette: `#E91E63 → #FF5722 → #FFC107` on matte black `#0D0D0F`.
Design canon: content before chrome, zero corner radius, opacity carries state.

## Licence

MIT. Zune, Zegoe, Zune HD and Microsoft are trademarks of Microsoft Corporation.
Dorado is an independent, non-affiliated homage.
