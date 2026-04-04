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

---

## Deployment: Custom Domains & GitHub Pages

This site is deployed via GitHub Pages at [chagrinvalleypainting.com](https://chagrinvalleypainting.com) (primary domain).

### Custom Domain Setup

- **Primary domain:** `chagrinvalleypainting.com`
- **Secondary domains:** `valleypaintingco.com`, `valleypaintingco.net` (should redirect to primary)
- **CNAME file:** The `public/CNAME` file contains the primary domain for GitHub Pages.
- **HTTPS:** Enforced via GitHub Pages settings (see below).

### DNS Records (configure at your domain registrar)

For each domain:

- **Apex domain** (`chagrinvalleypainting.com`, `valleypaintingco.com`, `valleypaintingco.net`):
  - Add **A records** pointing to GitHub Pages IPs:
    - `185.199.108.153`
    - `185.199.109.153`
    - `185.199.110.153`
    - `185.199.111.153`
- **www subdomain** (`www.chagrinvalleypainting.com`, etc):
  - Add a **CNAME record** pointing to `derecskey.github.io.`

### GitHub Pages Settings

1. Go to **Repository Settings > Pages**
2. Set **Custom domain** to `chagrinvalleypainting.com`
3. Check **Enforce HTTPS**
4. Save

### Redirects

- Configure `valleypaintingco.com` and `valleypaintingco.net` to redirect to `chagrinvalleypainting.com` via your domain registrar or DNS provider (if supported).
- GitHub Pages only allows one custom domain per repo; others must redirect externally.

---

