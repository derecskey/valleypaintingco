# Copilot Instructions

## Project Overview

Static brochure website for Valley Painting Company, a residential and commercial painting business serving Northeast Ohio. Deployed to GitHub Pages at `chagrinvalleypainting.com` / `valleypaintingco.com`. Fast, lightweight, accessible, privacy-conscious, and easy to maintain.

## Tech Stack

- **Framework:** Astro (`output: 'static'` — fully pre-rendered, no server runtime)
- **Deployment:** GitHub Pages via GitHub Actions (push to `main` triggers deploy)
- **Content:** Markdown/YAML files in `src/content/`
- **Styling:** Plain CSS or a minimal utility approach — avoid heavy frameworks unless warranted

## Guiding Principles

- **Static-first:** All pages are pre-rendered HTML. No SSR, no API routes.
- **Lightweight:** Ship minimal JavaScript. Prefer Astro's zero-JS default.
- **Accessible:** WCAG 2.1 AA compliance throughout — semantic HTML, proper alt text, keyboard navigability, sufficient color contrast.
- **Privacy-conscious:** No ad tracking or retargeting. Any analytics must be privacy-friendly (Plausible, Umami, or GoatCounter).
- **Easy to maintain:** Simple structure, clear conventions, minimal dependencies.

## Project Structure

```
src/
  layouts/    # Base layout components (e.g. BaseLayout.astro)
  components/ # Reusable UI components (PascalCase filenames)
  pages/      # One file per route (.astro or .md)
  content/    # Markdown/YAML content files
  assets/     # Images and other assets processed by Astro
public/       # Static files copied as-is (CNAME, robots.txt, etc.)
```

## Key Pages

Current planned pages include, but are not limited to: Home · Services (Interior, Exterior, Additional, Index) · About · Service Areas · Testimonials · Contact/Estimate · Privacy Policy · Accessibility Statement · 404. Refer to `src/pages/` for the authoritative route list as the project evolves.

## Conventions

- Pages use `BaseLayout.astro` for consistent header, nav, and footer.
- Content-heavy text lives in `src/content/`, not hardcoded in components.
- One component per file; PascalCase filenames for components.
- Prefer semantic HTML elements over generic `<div>` wrappers.
