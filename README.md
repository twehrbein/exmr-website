# ExMR project page

Static project page for *ExMR: Extremity Motion Refinement for Monocular Human Motion Capture*
(Tom Wehrbein and Bodo Rosenhahn). Plain HTML/CSS with no build step; served by GitHub Pages.

## Preview locally

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

## Deploy (GitHub Pages)

```sh
gh repo create twehrbein/exmr-website --public --source=. --push
gh api -X POST repos/twehrbein/exmr-website/pages -f "source[branch]=main" -f "source[path]=/"
```

The page is then served at https://twehrbein.github.io/exmr-website/ (like the FootMR page).

## To do when available

Search `index.html` for `TODO`:
- Code button URL.

## Assets

- `static/images/teaser.jpg`, `qualitative.jpg`, `sam3d.jpg`: Figs. 1, 4 and S1 of the paper,
  rendered without captions from the LaTeX sources.
- `static/images/method.jpg`: Fig. 2 (`wehrbein-fig2.pdf`).
- `static/videos/exmr_video.mp4`: the 29 MB supplementary video (2560x720, 3:51), same content
  as the video submitted to TPAMI.
