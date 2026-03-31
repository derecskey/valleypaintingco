# Agents

## Coding Agent

The GitHub Copilot Coding Agent implements GitHub Issues in this repository. Each issue includes a description and acceptance criteria that define the scope of the change.

### Build & Dev Commands

```bash
npm run dev      # local dev server
npm run build    # production build → dist/
npm run preview  # preview the production build locally
```

### Key Constraints

- Do not introduce server-side rendering or API routes. This is a fully static site.
- Do not add unnecessary JavaScript; prefer Astro's zero-JS default.
- All pages and components must maintain WCAG 2.1 AA accessibility.
- Do not add analytics or third-party scripts that violate the privacy-friendly requirement.
- New pages must use `BaseLayout.astro` and follow existing folder/naming conventions.
