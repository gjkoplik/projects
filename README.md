# gjkoplik.github.io/projects

Personal website built with [Zola](https://www.getzola.org/): projects, blog, and CV.

## Layout

- `config.toml`: site config (base URL, social links)
- `content/`: all the words. `_index.md` is the home page, `projects.md` and `cv.md` are standalone pages, `blog/` holds one markdown file per post
- `templates/`: Zola/Tera HTML templates
- `static/`: CSS, images, and other assets, copied verbatim into the built site
- `public/`: build output (gitignored)

## Preview locally

```bash
zola serve
```

Then open <http://127.0.0.1:1111> in any browser. The server live-reloads on file changes, and your browser renders the site in normal light mode (unlike the Claude Code desktop preview panel, which forces dark mode and has no toggle).

`zola build` writes the production site to `public/` if you want to inspect the raw output.

Zola is a single binary; it lives at `~/.local/bin/zola` here. To install or upgrade, download the latest release from [getzola.org](https://www.getzola.org/documentation/getting-started/installation/).

## Add a blog post

Drop a markdown file in `content/blog/`:

```markdown
+++
title = "Post Title"
date = 2026-06-12
summary = "One line shown in the post list."

[extra]
image = "images/blog/post-thumbnail.png"
+++

Post body.
```

`image` is optional and renders as a small thumbnail next to the post in the blog list. The path is relative to `static/`, so the example above points at `static/images/blog/post-thumbnail.png`.

## Add a project

Projects live in `content/projects.md` as one `##` heading per project: title, dates, a short blurb, an image, and a row of links. Images go in `static/images/` and render via the `img` shortcode:

```
{{ img(path="images/my_project.png", class="project-img", alt="description") }}
```

## Deploy

[.github/workflows/deploy.yml](.github/workflows/deploy.yml) builds the site with Zola and publishes it to GitHub Pages on every push to `master`.

One-time setup: in the repo's GitHub settings under Pages, set "Source" to "GitHub Actions". Until that switch is flipped, Pages keeps serving the legacy page from the branch root and the workflow's deploys go nowhere. Flipping it makes the Zola site live at the same URL.

## Archived

`archived/` holds the old Tufte-style projects page (`index.html`, `index.Rmd`) along with its images, widgets, and fonts. The new site copied what it needs into `static/`, so nothing in there is load-bearing; it's kept for posterity.
