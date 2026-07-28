# My Awakening Journey

Source for **https://francoischarette.github.io/myAwakeningJourney/** — a living
journal of observations on spirituality, human nature, and technology's effect
on human development.

Built with [Jekyll](https://jekyllrb.com/); GitHub Pages builds it
automatically on every push — **nothing needs to be installed locally**.
Comments are powered by [giscus](https://giscus.app) (GitHub Discussions).

## One-time setup

1. **Create the GitHub repo** — on github.com, create a new public repository
   named `myAwakeningJourney` (no README/license — this folder already has them),
   then from this folder:

   ```
   git remote add origin https://github.com/francoischarette/myAwakeningJourney.git
   git push -u origin main
   ```

2. **Enable GitHub Pages** — repo → Settings → Pages → under *Build and
   deployment*, set Source to **Deploy from a branch**, branch `main`, folder
   `/ (root)`. A minute or two later the site is live.

3. **Enable Discussions** — repo → Settings → General → Features → check
   **Discussions**.

4. **Configure giscus** — install the giscus app at
   https://github.com/apps/giscus (grant it just this repo), then go to
   https://giscus.app, enter `francoischarette/myAwakeningJourney`, pick the
   **Announcements** category and *Discussion title contains page pathname*.
   From the generated snippet copy `data-repo-id` and `data-category-id` into
   the `giscus:` section of `_config.yml`. Push — comments appear under every
   post.

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
