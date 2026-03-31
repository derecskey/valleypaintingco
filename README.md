# valleypaintingco
Astro-based, static-first brochure website for Valley Painting Company (valleypaintingco.com): fast, lightweight, accessible, privacy-conscious, and easy to maintain. Showcases services, gallery, service areas, and estimate/contact flow for a Northeast Ohio painting business.

## Project Folder Structure & Conventions

- `src/layouts/` — Base layout components (e.g. BaseLayout.astro)
- `src/components/` — Reusable UI components (PascalCase filenames)
- `src/pages/` — One file per route (.astro or .md)
- `src/content/` — Markdown/YAML content files
- `public/` — Static assets (images, fonts, CNAME, etc.)

**Note:** Empty folders are tracked with a `.keep` file so git can commit them.

## Local Development

```bash
npm install        # Install dependencies
npm run dev        # Start dev server at http://localhost:4321
```

## Build

```bash
npm run build      # Build static site to dist/
npm run preview    # Preview the production build locally
```

