# Haeffner Lab group website
This repo contains the Haeffner Lab group website.

To update the website, simply commit your changes to the appropriate file.
The changes will be automatically deployed to the live website, typically within 5-10 minutes.

Here are some of the important files:

### Global website layout
- Global page layout: [_layouts/default.html](_layouts/default.html)
- Global navigation menu: [_includes/menu.html](_includes/menu.html)
- Global page footer: [_includes/foot.html](_includes/foot.html)
- CSS styles: [assets/css/style.scss](assets/css/style.scss)

### General website pages
- Home page: [index.md](index.md)
- Group members page: [members/members.md](members/members.md)
- Publications page: [publications/publications.md](publications/publications.md)
- Visitor information page: [visitors/visitors.md](visitors/visitors.md)

### Research pages
- CCT: [research/quantum-electronics/quantum-electronics.md](research/quantum-electronics/quantum-electronics.md)
- Electron: [research/eQIP/eQIP.md](research/eQIP/eQIP.md)
- Lattice: [research/quantum-emulation/quantum-emulation.md](research/quantum-emulation/quantum-emulation.md)
- Spacetime: [research/ring-trap/ring-trap.md](research/ring-trap/ring-trap.md)
- SQIP: [research/quantum-computing/quantum-computing.md](research/quantum-computing/quantum-computing.md)
- STAQ: [research/staq/staq.md](research/staq/staq.md)

### Details

This website is hosted using [GitHub Pages](https://docs.github.com/en/github/working-with-github-pages).

> _Advanced:_ If you are making more complex changes and would like to test them locally before deploying, you can
do this by installing Jekyll. See the
[GitHub Pages documentation](https://docs.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll)
for more details. This is not necessary for simple changes. In most cases, it's easier to just edit the files in this repo directly and then verify
that your changes look good after the live site is updated.
