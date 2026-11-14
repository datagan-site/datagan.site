# datagan.site blog

Quarto website. Source is `.qmd` files. `quarto render` builds into `docs/`.
GitHub Pages serves `main:/docs` at https://datagan.site (no CI build).

## Sections

| Folder | Section | Use for |
|---|---|---|
| `systems/` | Systems | Engineering, observability, data, cloud, book notes on tech |
| `money/` | Money | Markets, F&O, investing, US markets |
| `body/` | Body | Health, food, fitness, weight |
| `mind/` | Mind | Inner peace, family, meditation |
| `notes/` | Notes | Everything else |

## New post

File name: `<section>/<short-slug>.qmd` (lowercase, hyphens). Front matter:

```yaml
---
title: "Post title"
description: "One line summary shown in listings."
date: YYYY-MM-DD
categories: [tag1, tag2]
draft: true   # remove to publish
---
```

- Images go in `<section>/assets/` and are linked as `assets/name.png`.
- Every `money/` post ends with: "This is my personal journal, not investment advice."
  Never write buy or sell calls or price targets for others (SEBI finfluencer rules).
- Keep the author's voice. Fix grammar and structure only when asked.

## Publish

1. `quarto render`
2. `git add -A && git commit -m "Post: <title>"`
3. Ask the author before `git push` (push changes the live site).

`quarto preview` gives a live local preview. It shows drafts.
