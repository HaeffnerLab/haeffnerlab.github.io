# Repository Guidelines

## Project Structure & Module Organization

This repository is a GitHub Pages/Jekyll site for the Haeffner Lab. Top-level Markdown files and directories define public pages: `index.md`, `members/`, `research/`, `publications/`, `presentations/`, `teaching/`, and `visitors/`. Shared layout lives in `_layouts/default.html`, reusable snippets in `_includes/`, and site metadata in `_config.yml`. Styles are compiled from `assets/css/style.scss`. Static assets are grouped by purpose: `images/` for site graphics, `members/pics/` for people and group photos, and `download-area/`, `publications/`, or `presentations/` for PDFs, slides, datasets, and other downloads.

## Build, Test, and Development Commands

- `bundle install`: install the Ruby gems needed by GitHub Pages.
- `bundle exec jekyll serve --livereload`: run the site locally, usually at `http://127.0.0.1:4000`.
- `bundle exec jekyll build`: build the static site into `_site/` and catch Liquid, Markdown, or asset errors.
- `bundle update github-pages`: update the pinned GitHub Pages gem when maintenance requires it.

Simple content edits can be committed directly, but run a local build before larger layout, navigation, or CSS changes.

## Coding Style & Naming Conventions

Use Markdown for content whenever possible and keep page front matter minimal, for example `title: Members`. Match surrounding indentation in existing HTML, Sass, and Markdown blocks; avoid reformatting unrelated files. Use lowercase, hyphenated names for new page directories and assets where practical, such as `research/new-project/index.md`. Always provide descriptive `alt` text for images and prefer semantic HTML (`<figure>`, `<figcaption>`, heading tags) when Markdown is insufficient.

## Testing Guidelines

There is no automated test suite in this repository. Treat `bundle exec jekyll build` as the required smoke test. After publishing or previewing content, verify the changed page visually and check accessibility with WAVE. For navigation or layout changes, confirm keyboard access by tabbing through links and menus.

## Commit & Pull Request Guidelines

Recent history uses short update-style subjects, often naming the changed content, such as `Update index.md` or `Update Bingran You bio/photo and add Integrated Photonics to Trap Technology`. Keep commits focused and descriptive. Pull requests should summarize changed pages, list new or replaced assets, note the local build result, and include screenshots for visual changes. Link related issues when available.

## Security & Configuration Tips

This is a public website repository. Do not commit secrets, private contact details, unpublished data, or credentials. Keep large downloads in the existing download/publication directories and avoid renaming published files unless you also update all links.
