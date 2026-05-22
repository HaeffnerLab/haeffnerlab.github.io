# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

The Haeffner Lab group website, served at https://ions.berkeley.edu via GitHub Pages. It is a Jekyll site — content is mostly Markdown with a thin layer of Liquid templating. Commits to `main` auto-deploy to production within ~5–10 minutes; there is no separate build/CI step to run.

## Local preview (optional)

Most edits don't need a local server — push and check the live site. For non-trivial layout/CSS changes:

```
bundle install         # first time only
bundle exec jekyll serve
```

The pinned `github-pages` gem in `Gemfile` mirrors what GitHub Pages runs in production, so local output should match the deployed site. `_site/` is the build output and is gitignored.

## Architecture

- **No Jekyll theme.** `_config.yml` sets `theme: false`, so every layout, include, and stylesheet is local to this repo. Don't assume theme defaults exist.
- **Single layout, `_layouts/default.html`.** Every Markdown page renders through it (header banner, `_includes/menu.html`, `{{ content }}`, `_includes/foot.html`). Site-wide chrome changes go here, not in individual pages.
- **Navigation is hand-maintained** in `_includes/menu.html`. Adding a research page means editing this file too — there is no auto-generated nav.
- **Styles** live in `assets/css/style.scss` (compiled by Jekyll because of the empty front-matter at the top). The body is a fixed `width: 850px` container; the site is not responsive.
- **Pages by convention** live at `<section>/index.md` (e.g. `members/index.md`, `research/trap-technology/index.md`, `publications/index.md`). Each has YAML front-matter with at least `title:`.
- **Member entries** use the `_includes/member.html` partial. Pass `name`, `title`, `image`, `email_name`/`email_domain`/`email_suffix`, and `bio`. Set `full_row=true` for a wide single-column row (used for the PI and admin). Multiple `{% include member.html %}` calls inside one `<tr>` produce a multi-column row.
- **Email addresses are obfuscated** via the `emicon()` JS in `_includes/e-mail-script.html`, which assembles `mailto:` links from char codes. Always pass emails as the three `email_name`/`email_domain`/`email_suffix` pieces to the include — never hard-code a plaintext `mailto:` in markup.
- **`CNAME`** pins the custom domain `ions.berkeley.edu`. Don't remove or rename it.

## Accessibility (mandatory for this site)

Berkeley/state of California compliance is non-optional. After any content change:

1. Run the page through https://wave.webaim.org/report#/ions.berkeley.edu and fix any errors it reports.
2. If you touched navigation, verify keyboard-only Tab traversal still reaches every link.

Common pitfalls to avoid:
- Every `<img>` and every `image=` passed to `member.html` must have meaningful `alt` text describing the image — don't duplicate a nearby caption.
- Use semantic HTML when dropping out of Markdown: `<h2>`/`<h3>` for headings, `<figure>` + `<figcaption>` for illustrations.
- Prefer plain Markdown to raw HTML wherever possible — fewer accessibility regressions and easier to maintain.
- Video/audio content needs captions.
