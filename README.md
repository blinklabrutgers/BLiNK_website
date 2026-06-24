# BLiNK Lab Website (R Markdown)

A static multi-page website for the BLiNK (Bilingualism: Language in
NeuroKognition) Lab, directed by Dr. Nuria Sagarra at Rutgers University.
Built with R Markdown's site generator and the BLiNK theme (blue / lime / ink).

## Files

```
_site.yml          Site config (output dir, shared header/footer, CSS)
styles.css         The BLiNK theme (colors, type, layout, responsive)
header.html        Top navigation bar (injected on every page)
footer.html        Footer (injected on every page)
index.Rmd          Home (hero + news + contact)
people.Rmd         People (director, PhD students, undergrads, former)
publications.Rmd   Selected publications
participate.Rmd    EEG study recruitment
gallery.Rmd        Lab photo gallery
resources.Rmd      EEG tutorials
location.Rmd       Address + map
images/            Logos, photos (see images/IMAGES_README.txt)
```

## Build it

In R, from this folder:

```r
install.packages("rmarkdown")   # one time
rmarkdown::render_site()
```

This renders the site into the `docs/` folder. Preview with:

```r
browseURL("docs/index.html")
```

To deploy on GitHub Pages: push the repo, then Settings > Pages >
Deploy from a branch > main > /docs.

## Add your images

Photos are referenced from the `images/` folder. Create these subfolders and
drop files in (exact names, lowercase). See `images/IMAGES_README.txt`.

- `images/people/`  headshots (square crop best)
- `images/lab/`     hero tiles (hero1-4) + gallery photos

People without a photo yet fall back to `images/placeholder.svg`.

## Theme

Colors and fonts live at the top of `styles.css` (the `:root` variables:
`--blue #36B3FB`, `--lime #C0FE71`, `--ink #0E1B26`). Fonts: Manrope (Google
Fonts) for text, Space Mono for small labels. The site is responsive (the
hero and grids collapse to a single column on phones).

The lab logo (`images/blink-logo.gif`) is animated; the Rutgers School of Arts
and Sciences lockup sits in the navbar (`rutgers-sas-black.png`) and footer
(`rutgers-sas-white.png`).
