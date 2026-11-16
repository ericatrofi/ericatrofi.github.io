# ericatrofi.github.io

Personal website, built with Jekyll and the [Minimal Light](https://github.com/yaoyao-liu/minimal-light) theme (CC0), plus a top menu, art gallery and blog.

## Where things are

| To change…                         | Edit                                   |
|-----------------------------------|----------------------------------------|
| Name, position, email, links, menu | `_config.yml`                          |
| Photo                              | replace `assets/img/avatar.png`        |
| About page (bio, interests, news)  | `index.md`                             |
| Publications                       | `_data/publications.yml`               |
| Projects                           | `projects.md`                          |
| Art gallery                        | images in `assets/img/art/` + list in `_data/art.yml` |
| Blog posts                         | one `.md` file per post in `_posts/`   |
| CV                                 | `cv.md` (PDF goes in `assets/files/`)  |
| Colours and fonts (whole site)     | `_sass/palette.scss` (dark mode: `_sass/palette-dark.scss`) |
| Look of menu / gallery / blog      | `_sass/custom.scss`                    |
| Page layout (sidebar, structure)   | `_layouts/default.html`                |

## Preview locally

```bash
export PATH="/opt/homebrew/opt/ruby/bin:$PATH"   # once per terminal
bundle exec jekyll serve --livereload
```

Open http://localhost:4000. Pages refresh when you save.
Stop with Ctrl+C. Changes to `_config.yml` need a restart.

## Publish

Pushing to `main` updates https://ericatrofi.github.io within a minute or two.
