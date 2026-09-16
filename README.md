# Shopify Theme Handbook

The internal knowledge base for scaffolding, developing, and publishing Shopify themes to the Theme Store — currently written for the Solis project, reusable for any future theme.

**Live site:** [https://saabbir.github.io/shopify-theme-handbook/](https://saabbir.github.io/shopify-theme-handbook/)

This repo is the **documentation site only**. It does not contain a Shopify theme's code.

For day-of-submission work (scorecard, QA checklist, packaging gate, rejection autopsy), use the companion toolkit: [Theme Store Checklist](https://saabbir.github.io/shopify-theme-store-checklist/) ([repo](https://github.com/Saabbir/shopify-theme-store-checklist)).

## Stack

Built with [Astro](https://astro.build) + [Starlight](https://starlight.astro.build) — a static docs site. Content lives as Markdown in `src/content/docs/`.

## Running locally

```bash
npm install
npm run dev
```

Then open `http://localhost:4321/shopify-theme-handbook/`.

```bash
npm run build    # outputs to dist/
npm run preview  # preview the production build locally
```

## Deploying

GitHub Pages is configured via [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml). Pushes to `main` build with Astro and publish to `https://saabbir.github.io/shopify-theme-handbook/`.

## Structure

```
src/content/docs/    → all handbook content (Markdown)
public/templates/    → downloadable files (Cursor rules, CLAUDE.md, PR template, CI workflow)
src/styles/          → brand/theme overrides for the Starlight UI
astro.config.mjs     → site config + sidebar navigation structure
```
