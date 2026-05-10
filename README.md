# fredkchoi.github.io

Personal portfolio for Fred Choi. Built with [Astro](https://astro.build/) and deployed to GitHub Pages.

Live site: https://fredkchoi.github.io

## Develop

```bash
npm install
npm run dev      # http://localhost:4321
npm run build    # outputs to dist/
npm run preview  # preview the production build locally
```

## Deploy

Pushes to `main` are deployed automatically via GitHub Actions
(`.github/workflows/deploy.yml`). Make sure the repository's Pages source is
set to "GitHub Actions" under **Settings → Pages**.

## Structure

```
src/
  layouts/BaseLayout.astro   # html shell, fonts, meta, nav + footer
  components/Nav.astro
  components/Footer.astro
  pages/
    index.astro              # Home
    about.astro              # About & Experience
    projects.astro           # Projects
    contact.astro            # Contact
  styles/global.css          # design tokens + utilities
```

Design system is Chrome-inspired minimalist (Inter, hairline borders, single
blue accent `#1a73e8`). All tokens live in `src/styles/global.css` under
`:root`.
