# mybolg

A Hexo blog using the default Landscape theme.

Published at: https://hanchen2232.github.io/

## Local Development

This environment did not have Node.js installed globally, so a local Node.js runtime was placed in `.tools/` and ignored by git.

```bash
export PATH="$PWD/.tools/bin:$PATH"
npm install
npm run server
```

Then open the local URL printed by Hexo, usually `http://localhost:4000`.

## Build

```bash
export PATH="$PWD/.tools/bin:$PATH"
npm run clean
npm run build
```

The generated static site is written to `public/`.

## GitHub Pages Notes

This repository is configured for the GitHub Pages user site:

```yaml
url: https://hanchen2232.github.io
root: /
```

GitHub Actions builds the Hexo site and deploys the generated `public/` directory to GitHub Pages.
