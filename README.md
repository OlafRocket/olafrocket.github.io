# olafrocket.github.io

Sources of the web site "It's not Rocket Science Lab". Static site built
with [Hugo](https://gohugo.io) and the
[Hextra](https://github.com/imfing/hextra) theme.

| Path | Content |
|---|---|
| `hugo.yaml` | Site configuration, menu, repository URL |
| `.github/workflows/site.yml` | Build and deployment to GitHub Pages |
| `assets/css/custom.css` | Colour palette |
| `layouts/shortcodes/repo.html` | `repo` shortcode: URL of a file in the lang_python repository |
| `content/_index.md` | Home page |
| `content/docs/` | Introduction, getting started, reference links |
| `content/demos/` | One page per demo |
| `content/blog/` | Blog posts |
| `archetypes/blog.md` | Template for new blog posts |
| `layouts/_partials/navbar-title.html` | Theme override: no site name in the navbar of the home page |
| `static/fonts/` | Display font Fraunces (SIL Open Font License) |
| `static/images/authors/` | Author pictures |
| `themes/hextra/` | Theme, git submodule pinned to v0.13.0 |

## Requirements

Hugo 0.146.0 or later.

## Theme checkout

```sh
git submodule update --init
```

## Preview

```sh
hugo server
```

The site is served at <http://localhost:1313/>.

## New blog post

```sh
hugo new blog/<slug>.md
```

The file is created from `archetypes/blog.md`:

```markdown
---
title: Post title
date: 2026-11-23
draft: true
tags: []
authors:
  - name: Olaf Razzoli
    link: https://github.com/OlafRocket
    image: /images/authors/olaf.png
---

Summary paragraph.

<!--more-->

Body.
```

| Field | Meaning |
|---|---|
| `draft` | A draft is shown by `hugo server -D` only and is not deployed. Remove the line to publish |
| `authors` | Name, link and picture shown under the post title. One entry per author; pictures are in `static/images/authors/` |

## Links to repository files

```markdown
[USAGE.md]({{< repo "USAGE.md" >}})
[examples]({{< repo "examples" "tree" >}})
```

## Deployment

`.github/workflows/site.yml` builds the site and deploys it to GitHub
Pages. The workflow is started manually (Actions, "Deploy site", Run
workflow). GitHub Pages must be enabled for the repository with source
"GitHub Actions".
