# MLAB blog

Source of the MLAB blog. It is a [Jekyll](https://jekyllrb.com/) site built on the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme.

## Run locally

You need Ruby 3.x with Bundler.

```
bundle install
bundle exec jekyll serve --livereload
```

The site is then served at <http://127.0.0.1:4000>.

## Write a post

Add a Markdown file to `_posts/` named `YYYY-MM-DD-title.md`:

```yaml
---
title: "Post title"
date: 2026-01-31 10:00
author: jakub-kakona
categories: Modules
tags: Sensors I2C
excerpt: "One or two sentences shown in the post list, in search results and when the post is shared."
toc: true
---
```

- `date` sets the date shown on the post and its position in the list. It takes precedence over the date in the file name.
- `author` is a key from `_data/authors.yml`. Without it the post is attributed to MLAB.
- `toc: true` adds a table of contents built from the headings.
- `mathjax: true` enables LaTeX formulas in the post.

## Add an author

Add an entry to `_data/authors.yml` and put the photo in `assets/images/authors/`:

```yaml
jane-doe:
  name: "Jane Doe"
  bio: "Role in the company"
  avatar: "/assets/images/authors/jane-doe.jpg"
  links:
    - label: "GitHub"
      icon: "fab fa-fw fa-github"
      url: "https://github.com/jane-doe"
```

## Related blogs

The same setup is used for the blogs of the sister projects:

- MLAB: <https://github.com/cisar2218/blog> (this repository)
- ThunderFly: <https://github.com/ThunderFly-aerospace/blog>
- UST: <https://github.com/UniversalScientificTechnologies/blog>
