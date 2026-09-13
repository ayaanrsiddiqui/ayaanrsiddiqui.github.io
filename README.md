# ayaanrsiddiqui.github.io

Source for my personal site, live at **[ayaanrsiddiqui.github.io](https://ayaanrsiddiqui.github.io)**.

One static page, no build step and no dependencies: `index.html` holds the markup, the
stylesheet and the whole design system inline. The only external request is the Google
Fonts stylesheet. `resume.pdf` is the copy the masthead button links to.

## Structure

| File | What it is |
| --- | --- |
| `index.html` | The entire site — markup plus inlined CSS custom-property theme |
| `resume.pdf` | Current résumé, linked from the masthead |

## Design notes

Every substantive claim on the page carries a **receipt** underneath it: a monospace line
naming the file, measurement or date the claim rests on, so a reader can check it rather
than take it. That constraint is the reason the page is written the way it is — if a
sentence can't be sourced to something specific, it doesn't go on the site.

Colours are CSS custom properties declared on `:root`, redefined under both
`@media (prefers-color-scheme: dark)` and `:root[data-theme="dark"]`, so the page follows
the reader's system theme and still responds to an explicit override.

## Local development

No tooling required.

```sh
git clone https://github.com/ayaanrsiddiqui/ayaanrsiddiqui.github.io.git
cd ayaanrsiddiqui.github.io
open index.html          # or: python3 -m http.server 8000
```

Pushes to `main` deploy automatically through GitHub Pages.

## Contact

- **Email** — [ayaanrsiddiqui@virginia.edu](mailto:ayaanrsiddiqui@virginia.edu)
- **LinkedIn** — [linkedin.com/in/ayaanrsiddiqui](https://www.linkedin.com/in/ayaanrsiddiqui/)
