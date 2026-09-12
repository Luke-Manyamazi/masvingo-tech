# Masvingo Tech Community

> A community-focused technology landing page connecting developers, students, entrepreneurs, and innovators across Masvingo Province, Zimbabwe.

Masvingo Tech Community is a lightweight static website concept designed to showcase a local technology ecosystem and provide an accessible starting point for community participation.

## Highlights

- Responsive landing-page experience
- Community-focused information architecture
- Mobile navigation and section-based browsing
- Scroll-reveal and visual interaction effects
- Centralized WhatsApp community-link configuration
- Social sharing and canonical metadata prepared for deployment

## Technology

- HTML5
- Tailwind CSS via CDN
- Vanilla JavaScript
- Responsive CSS
- Browser-based animations and interactions

## Project Structure

```text
index.html
favicon.svg
assets/
├── logo.png
├── logo-icon.png
└── og-image.jpg
```

The site is intentionally dependency-light: the page, styling, and interactivity are kept in a small static project without a framework, backend, or build pipeline.

## Running Locally

No package installation is required.

```bash
npx serve .
```

Or use Python's built-in server:

```bash
python -m http.server 8000
```

## Deployment Notes

Before production launch, verify the community invitation link, Open Graph preview image, and canonical domain configuration. The project can be hosted on any static web host.

## Engineering Focus

This project demonstrates responsive static-site development, semantic HTML, utility-first CSS, browser-side JavaScript, lightweight interaction design, and deployment-ready metadata without introducing unnecessary framework complexity.
