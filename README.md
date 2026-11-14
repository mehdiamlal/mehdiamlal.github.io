# Personal site

A plain [Jekyll](https://jekyllrb.com) site, built and hosted for free by GitHub Pages.
No themes, no JavaScript: one stylesheet and three small layouts.

## What to edit

| To change…                 | Edit                                   |
|----------------------------|----------------------------------------|
| Bio                        | `index.md`                             |
| Links (email, Scholar, …)  | `_config.yml` → `links`                |
| News                       | `_data/news.yml` (newest first)        |
| Publications               | `_data/publications.yml`               |
| Photo                      | replace `images/profile.png`           |
| Fonts, colors, spacing     | `style.css`                            |

## Writing a blog post

Create `_posts/YYYY-MM-DD-short-title.md`:

```markdown
---
layout: post
title: "My post title"
---

Write in Markdown here.
```

It shows up under **Writing** on the home page, at `/blog/short-title/`, and in the RSS feed (`/feed.xml`).
Put unfinished posts in `_drafts/` (not published). Images go in `images/`.

## Publishing (once)

1. Create a GitHub repository named `<your-username>.github.io` and push this folder to it.
2. In the repository: **Settings → Pages → Source: Deploy from a branch → `main` / root**.
3. Set `url` in `_config.yml` to `https://<your-username>.github.io`.

After that, every push updates the site within a minute or two.

## Previewing locally (optional)

Needs a recent Ruby (`brew install ruby`), then:

```bash
bundle install
bundle exec jekyll serve
```

and open http://localhost:4000.
