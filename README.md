# MapFly project website

[Project page](https://GuYan66.github.io/MapFly-Website/) · [Code repository](https://github.com/GuYan66/MapFly) · [Dataset](https://huggingface.co/datasets/EzGuYan/MapFly) · [UE environments](https://huggingface.co/datasets/EzGuYan/MapFly_DataGen)

Research code is maintained separately in **GuYan66/MapFly**.

## Publishing

Edit the website on `main`. GitHub Actions copies the static site to `gh-pages`,
which GitHub Pages publishes from its root directory. Do not edit the generated
`gh-pages` branch directly.

This follows OpenFly's organization: separate code and website repositories,
with the website's main branch automatically publishing to gh-pages. This site
uses plain HTML/CSS/JavaScript and does not require a Vue/Vite build.

## Local preview

```bash
python -m http.server 8765
```

Open <http://localhost:8765/>.

## Editing

- `index.html`: title, authors, resource buttons, navigation and footer.
- `site-config.js`: author details, resource links and citation.
- `static/js/mapfly.js`: content, scene gallery, videos and PDF reader.
- `static/css/editorial.css`: typography and responsive layout.
- `assets/`: paper, figures, videos, icons and fonts.

Replace `assets/MapFly.pdf` to update the paper. Preserve relative asset URLs.
The demonstration videos are already at 10× speed. Anonymous author details and
the provisional citation are retained from the supplied manuscript.

## License

Adapted from Eliahu Horwitz's Academic Project Page Template, under CC BY-SA 4.0.
See [TEMPLATE-NOTICE.md](TEMPLATE-NOTICE.md). Research media and third-party
components retain their respective rights; font and icon licenses are in assets.
