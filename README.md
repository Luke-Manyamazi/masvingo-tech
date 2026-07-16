# Masvingo Tech Community

Landing page for Masvingo Tech Community — a community-driven tech ecosystem connecting developers, students, entrepreneurs, and innovators across Masvingo Province, Zimbabwe.

Live concept site: single-page, no build step, no backend. Built with static HTML, Tailwind CSS (via CDN), and vanilla JS for scroll animations and interactivity.

## Running locally

No install or build required — it's a single static HTML file.

- Open `index.html` directly in a browser, or
- Serve it locally for a more production-like experience (some browsers restrict fonts/local file access under `file://`):

  ```bash
  npx serve .
  # or
  python -m http.server 8000
  ```

## Project structure

```
index.html          All markup, styles, and script (single file)
favicon.svg          Fallback vector favicon
assets/
  logo.png           Full brand lockup (icon + wordmark), transparent background
  logo-icon.png       Cropped emblem only, used in nav/footer/favicon
```

## Before deploying

- **WhatsApp invite link**: set in `CONFIG.whatsappLink` near the bottom of `index.html`. All `[data-whatsapp]` links pull from this single source of truth.
- **OG image**: `assets/og-image.jpg` is referenced in the `<meta property="og:image">` tags but not yet included — add a real 1200×630 social preview image before launch.
- **Canonical URL**: currently set to `https://masvingotech.org/` in the `<link rel="canonical">` and Open Graph tags — update if the domain changes.

## Tech notes

- Styling is Tailwind CSS loaded from the CDN plus a small `<style>` block for custom effects (glass cards, gradient blobs, scroll-reveal, roadmap line draw, scroll-progress bar, cursor parallax on the hero).
- All interactivity (mobile menu, active nav highlighting, section reveals, scroll-to-top button) is plain JS at the bottom of `index.html` — no framework, no bundler.
