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
| "Of the Month" picks (sidebar card + `/picks/` archive) | `_data/picks.yml` (newest month at the top) |
| Colours and fonts (whole site)     | `_sass/palette.scss` (dark mode: `_sass/palette-dark.scss`) |
| Look of menu / gallery / blog      | `_sass/custom.scss`                    |
| Page layout (sidebar, structure)   | `_layouts/default.html`                |

### About page blocks

Each `## Heading` in `index.md` becomes its own card. Put `{: .half}` on the
line right under a heading to make it half width; two half cards in a row sit
side by side (they stack on phones).

## Ideas for later

- **Showcase / card grid for Projects**, inspired by
  https://luost.me/academic-homepage/showcase : a pinboard of mixed-size cards
  (image or plot, title, one or two lines, links to paper/code/slides), with
  some wide "highlight" cards. Plan: keep publications as a list, turn projects
  into cards, content in a data file (like `_data/art.yml`), plain CSS, no
  extra library. Two or three card sizes at most. Could later host
  interactive simulations inside a card.
- **Hand-drawn menu icons**: already supported, just add drawings (see
  `_config.yml`, `icon:` under each menu item).
- **Editor's Note** for headings, if a web licence is bought
  (self-host the font files in `assets/fonts/`).
- art of the month/image of the month or maths fact of the month 

## Preview locally

```bash
export PATH="/opt/homebrew/opt/ruby/bin:$PATH"   # once per terminal
bundle exec jekyll serve --livereload
```

Open http://localhost:4000. Pages refresh when you save.
Stop with Ctrl+C. Changes to `_config.yml` need a restart.

## Publish

Pushing to `main` updates https://ericatrofi.github.io within a minute or two.
