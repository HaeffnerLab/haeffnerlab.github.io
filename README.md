# Haeffner Lab group website ([https://ions.berkeley.edu](https://ions.berkeley.edu))

This repo contains the Haeffner Lab group website.

To update the website, simply commit your changes to the appropriate file.
The changes will be automatically deployed to the live website
at [https://ions.berkeley.edu](https://ions.berkeley.edu), typically within 5-10 minutes.

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

### Details

This website is hosted using [GitHub Pages](https://docs.github.com/en/github/working-with-github-pages).

> _Advanced:_ If you are making more complex changes and would like to test them locally before deploying, you can
do this by installing Jekyll. See the
[GitHub Pages documentation](https://docs.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll)
for more details. This is not necessary for simple changes. In most cases, it's easier to just edit the files in this repo directly and then verify
that your changes look good after the live site is updated.
