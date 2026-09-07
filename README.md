# Nworah, Jecintha — Portfolio

A single-page personal portfolio site for Chinyere Jecintha Nworah — Computer Science student, full-stack developer, and AI/ML enthusiast. Built as a dark, editorial-style site with scroll-driven animation, a custom project grid, and direct links to live work.

---

## Overview

This site is a single `index.html` file — no build step, no framework, no dependencies to install. It's meant to be dropped straight into a GitHub Pages repo and served as-is.

It covers:
- A hero section introducing who I am, with a rotating role tagline (Full-Stack Dev / AI-ML Enthusiast / Problem Solver / Builder)
- A **Selected Work** grid linking out to live projects
- An **About** section with education, experience, certification, and a skills breakdown
- An **Elsewhere online** section linking to GitHub, LinkedIn, and X
- A closing contact section with a direct email CTA

## Tech stack

- **HTML5 / CSS3** — semantic structure, CSS custom properties for theming, responsive grid layouts
- **Vanilla JavaScript** — no framework; handles scroll progress, role-word cycling, and reveal logic
- **[GSAP](https://gsap.com/) + ScrollTrigger** — hero load-in sequence, scroll-triggered reveals, and parallax drift on section labels and social icons (loaded via CDN)
- **Google Fonts** — [Unbounded](https://fonts.google.com/specimen/Unbounded) (display), [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) (body), [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (mono/labels)

No package manager, bundler, or build process is used — everything is loaded via CDN `<link>`/`<script>` tags directly in `index.html`.

## Features

- **Scroll progress bar** — thin gradient bar across the top tracking scroll position
- **Animated hero load-in** — staggered entrance for name, role, bio, and tech-stack pills
- **Rotating role tagline** — cycles through role titles every few seconds
- **Scroll-triggered reveals** — sections and project cards fade/slide in as they enter the viewport
- **Ghost-text section labels** — large outlined background text behind each section heading, with subtle parallax drift on scroll
- **Project grid** — each project card includes an icon, description, tech tags, and a live-demo link (where applicable)
- **Accessibility considerations:**
  - Respects `prefers-reduced-motion` — disables the role cycler, parallax drift, and smooth scrolling for users who've requested reduced motion
  - `:focus-visible` states on all interactive elements (nav links, project links, buttons, social CTAs) for keyboard navigation
  - Standard system cursor throughout (no custom cursor overlay)
- **Fully responsive** — dedicated breakpoints for tablet (≤860px) and mobile (≤480px), including grid reflow, hidden decorative elements, and full-width CTAs on small screens

## Project structure

```
.
└── index.html   # Everything — markup, styles, and scripts in one file
```

## Running locally

No build step required. Either:

- Open `index.html` directly in a browser, or
- Serve it locally for a closer-to-production experience:
  ```bash
  python3 -m http.server 8000
  ```
  then visit `http://localhost:8000`

## Deployment

This site is deployed via **GitHub Pages**:

1. Push `index.html` to the `main` branch of this repo
2. In repo Settings → Pages, set Source to "Deploy from a branch," branch `main`, folder `/ (root)`
3. The site publishes automatically to `https://jecinthacodes.github.io/REPO-NAME/`

## Featured projects linked from this site

| Project | Description |
|---|---|
| [MarketBook](https://jecinthacodes.github.io/marketbook/) | Offline-capable daily profit tracker for African market traders |
| [EduFlow — CSC 1/4 Portal](https://jecinthacodes.github.io/student-portal/) | Coordination hub for a 398-student CS class |
| [The Home Restaurant & Lounge](https://jecinthacodes.github.io/thehomerestaurant-lounge/) | Frontend site for a Calabar restaurant & lounge |
| [Winners.xyz](https://jecinthacodes.github.io/winners.xyz/) | Animated landing page for Winners FC |
| DevPair | In-progress developer work-partner matchmaking app |

## About me

Computer Science student (B.Sc., University of Cross River State) passionate about building software that solves practical problems. I work across frontend, backend, databases, and AI/ML — and learn best by building, experimenting, and debugging.

- **Skills:** HTML, CSS, JavaScript, Python, C#, SQL, MongoDB, Git/GitHub, Responsive Web Design, AI-assisted development, Machine Learning
- **Certification:** Introduction to Programming 1 — Saylor University

## Contact

- **Email:** [jecinthabusiness@gmail.com](mailto:jecinthabusiness@gmail.com)
- **GitHub:** [@jecinthacodes](https://github.com/jecinthacodes)
- **LinkedIn:** [Chinyere Nworah](https://www.linkedin.com/in/chinyere-nworah-45a51b434)
- **X:** [@jecinthaX](https://x.com/jecinthaX)

---

© 2026 Chinyere Jecintha Nworah
