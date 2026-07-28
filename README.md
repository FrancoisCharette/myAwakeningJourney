# My Awakening Journey

Source for **https://francoischarette.github.io/myAwakeningJourney/** — a living
journal of observations on spirituality, human nature, and technology's effect
on human development.

Built with [Jekyll](https://jekyllrb.com/); GitHub Pages builds it
automatically on every push — **nothing needs to be installed locally**.
Comments are powered by [giscus](https://giscus.app) (GitHub Discussions).

## One-time setup

- [x] **Repo created and pushed** — https://github.com/FrancoisCharette/myAwakeningJourney
- [x] **GitHub Pages enabled** — deploying from `main`, root folder
- [x] **Discussions enabled**
- [x] **giscus IDs filled into `_config.yml`** (`repo_id`, `category_id`, category *Announcements*)
- [ ] **Install the giscus app** — the only remaining step, and it must be done
      from your own GitHub account: visit https://github.com/apps/giscus →
      *Install* → **Only select repositories** → `myAwakeningJourney`. Comments
      go live immediately afterwards; no code change needed.

## Writing a post

1. Copy `_drafts/post-template.md` into `_posts/` and rename it
   `YYYY-MM-DD-short-title.md` (the filename date = publication date).
2. Edit the front matter (title, categories) and write in Markdown.
3. Commit and push. The site rebuilds automatically (~1 minute).

## Revising a post (the whole point of this site)

Edit the post file, then record the evolution in its front matter:

```yaml
updated: 2026-09-15
evolution:
  - date: 2026-09-15
    note: "A reader's comment made me reconsider X — rewrote the second half."
```

The post page will show a *"How my thinking has evolved"* box, and listings
will show the revision date next to the original one.

## Layout

| Path | Purpose |
|---|---|
| `_posts/` | Published posts (Markdown) |
| `_drafts/` | Unpublished drafts + the post template |
| `_layouts/`, `_includes/` | Page templates and the giscus embed |
| `assets/css/style.css` | All styling (light + dark mode) |
| `_config.yml` | Site title, links, giscus settings |
