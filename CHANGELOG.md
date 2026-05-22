# Changelog

All notable changes to **Moe-Kyaw-Aung-portfolio-V5** are documented here.

Format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [5.0.0] — 2026-05-22 🚀 Initial Release

### Added
- Complete single-file portfolio architecture (HTML + CSS + JS, zero dependencies)
- **Hero Section** — Interactive Canvas particle system (90 particles, mouse-following lines)
- **Hero Section** — Floating glasspunk info card with animated float effect
- **About Section** — Real Gravatar profile photo with glow border + floating badge
- **Skills Section** — 12 animated progress bars triggered by IntersectionObserver
- **Stats Section** — Animated counter: 5+ years, 49+ certs, 22 repos, 12 socials
- **Projects Section** — 6 real GitHub repositories with tech chips and links
- **Certificates Section** — 49 real Programming Hub certificates with:
  - Category filter (All, Mobile, Web, Security, Cloud & AI, Other)
  - Full-screen lightbox with keyboard navigation (← → Esc)
  - Lazy-loading images with graceful fallback
- **GitHub Section** — 2 GitHub accounts (Dev-moe-kyawaung + Moekyawaung) with pinned repos
- **Organizations Section** — 6 org cards (Microsoft, Google, Programming Hub, etc.)
- **Social Links Section** — 16 verified platforms from Gravatar
- **Testimonials Slider** — 4 slides, 5s auto-play, dot indicators, manual controls
- **Pricing Table** — 3 tiers: Starter ($800), Professional ($2,500), Enterprise (Custom)
- **FAQ Accordion** — 6 questions with smooth max-height CSS transition
- **Newsletter Form** — Email validation + success confirmation
- **Contact Form** — Full field validation + Google Maps embed (Tachileik, Myanmar)
- **Footer** — 4-column layout with social icons and links
- Dark/Light mode toggle with localStorage persistence
- Responsive left sidebar navigation with hamburger menu (mobile)
- Scroll-triggered fade animations (.fi / .fl / .fr classes with staggered delays)
- Parallax depth effect on decorative orbs
- Back-to-top button (appears after 400px scroll)
- Sticky "Hire Me" CTA button
- Active nav link sync via IntersectionObserver
- Animated preloader with dual-ring orbit and glowing core
- WCAG 2.1 AA accessibility compliance
- Full SEO meta tags (OpenGraph, Twitter Card, robots, canonical)
- GitHub Actions CI/CD workflow for auto-deploy to GitHub Pages

### Design System
- Glasspunk design language with `backdrop-filter: blur()` layered panels
- CSS custom properties for both Light and Dark themes
- Color palette: Primary `#9b8ec4` / Secondary `#7c6daa` / Accent `#c084fc`
- Typography: Orbitron (headings) + Nunito (body) via Google Fonts

### Tech Stack
- HTML5 semantic elements
- CSS3 custom properties, animations, grid, flexbox
- Vanilla JavaScript ES6+ (Canvas API, IntersectionObserver, requestAnimationFrame)
- Font Awesome 6.5.0 icons
- Zero build tools, zero frameworks, zero npm packages

---

## [Unreleased] — Upcoming

### Planned for V5.1.0
- EmailJS integration for real contact form submissions
- Formspree/Netlify Forms newsletter backend

### Planned for V5.2.0
- Blog section with lightweight Markdown renderer
- RSS feed support

### Planned for V5.3.0
- PWA: Web App Manifest + Service Worker
- Offline support with cache strategy

### Planned for V6.0.0
- Full React/Next.js rebuild
- Headless CMS (Contentful or Sanity) for certificates/projects
- Server-side rendering for SEO
- TypeScript
