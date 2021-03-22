# Haeffner Lab group website ([https://ions.berkeley.edu](https://ions.berkeley.edu))

This repo contains the Haeffner Lab group website.

To update the website, simply commit your changes to the appropriate file.
The changes will be automatically deployed to the live website
at [https://ions.berkeley.edu](https://ions.berkeley.edu), typically within 5-10 minutes.

## Website structure

Here are some of the important files:

### Global website layout
- Site properties: [_config.yml](_config.yml)
- Global page layout: [_layouts/default.html](_layouts/default.html)
- Global navigation menu: [_includes/menu.html](_includes/menu.html)
- Global page footer: [_includes/foot.html](_includes/foot.html)
- CSS styles: [assets/css/style.scss](assets/css/style.scss)

### General website pages
- Home page: [index.md](index.md)
- Group members page: [members/index.md](members/index.md)
- Publications page: [publications/index.md](publications/index.md)
- Visitor information page: [visitors/index.md](visitors/index.md)

### Research pages
- CCT: [research/quantum-electronics/index.md](research/quantum-electronics/index.md)
- Electron: [research/electron-trap/index.md](research/electron-trap/index.md)
- Lattice: [research/quantum-simulation/index.md](research/quantum-simulation/index.md)
- Spacetime: [research/ring-trap/index.md](research/ring-trap/index.md)
- SQIP: [research/surface-treatment/index.md](research/surface-treatment/index.md)
- STAQ: [research/staq/index.md](research/staq/index.md)

## Accessibility

We have a responsibility to the scientific community (as well as to the university and the state of California) to comply with basic web accessibility standards. This means ensuring the site is usable by vision-impaired, hearing-impaired, and motor-impaired users.

After making changes, *please* verify that the WAVE report for your new content shows no errors:
1. Go to https://wave.webaim.org/report#/ions.berkeley.edu.
1. Navigate to the page you changed.
1. If there are any errors, fix them.

If you made changes to navigation (such as the global menu), please ensure that keyboard accessibility still works. To verify this, instead of using a mouse, use "Tab" on your keyboard to cycle through the page. Ensure that all of the links on the page can be accessed.

Some tips to avoid the most common issues:
1. Use standard Markdown syntax when possible. It's easier to read, easier to edit in the future, and less likely to introduce accessibility problems.
1. Every image must have "alt" text. This should describe what is in the image. Don't just repeat the figure caption here. Imagine how you would describe the image to someone who cannot see it.
1. When you must use HTML elements, choose the appropriate tags. Use `<h2>`, `<h3>`, etc. for headings and sub-headings. Use `<figure>` and `<figcaption>` for illustrations. This helps screen readers and other software interpret the page structure in a sensible way.
1. If you are adding content with sound (such as video), it *must* have captions. Consider using YouTube, which can auto-generate captions.

## Details

This website is hosted using [GitHub Pages](https://docs.github.com/en/github/working-with-github-pages).

> _Advanced:_ If you are making more complex changes and would like to test them locally before deploying, you can
do this by installing Jekyll. See the
[GitHub Pages documentation](https://docs.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll)
for more details. This is not necessary for simple changes. In most cases, it's easier to just edit the files in this repo directly and then verify
that your changes look good after the live site is updated.
