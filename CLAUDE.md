# neno web GmbH Website

## 🎯 Project Vision & Strategy

A minimalist, high-end one-pager for **neno web GmbH**. The site positions the company as a **Senior Expert Collective** (not a traditional agency). It emphasizes Swiss precision, technical excellence (Next.js, React, Vue, Angular, Astro), and industry-leading Accessibility (A11y).

* **Core Message:** "No Juniors. Just Experts."
* **USP:** 5-time Best of Swiss Web Award winners. Experts in A11y and Frontend Architecture.
* **Design Language:** Swiss Minimalist (Grid-based, typography-focused, plenty of whitespace).
* **Target Audience:** Large enterprises (SBB, insurance, etc.) and high-end digital agencies looking for senior reinforcement.

## 🛠 Tech Stack

* **Framework:** [Astro](https://astro.build/) (Static Site Generation for maximum performance).
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (Utility-first, minimalist).
* **Components:** Minimal React (only for islands of interactivity, if needed).
* **Deployment:** Vercel or Netlify.
* **Accessibility:** 100/100 Lighthouse score, WCAG 2.1/2.2 AA/AAA compliance.

## 📋 Project Roadmap & Tasks

### Phase 1: Foundation & Setup

* [ ] Initialize Astro project with Tailwind CSS.
* [ ] Setup folder structure (`/components`, `/layouts`, `/content`).
* [ ] Configure bilingual support (English/German) via Astro i18n or simple sub-routes.
* [ ] Implement global SEO metadata & Social Share cards.


### Phase 2: Design System & Layout

* [ ] Define Typography (Inter/Neue Montreal) and Color Palette (White/Black/Neno-Red).
* [ ] Create the **Swiss Grid** layout (Fixed navigation, responsive margins).
* [ ] Implement the minimalist Header (SVG Logo integration).
* [ ] Build the massive typography Hero Section.

### Phase 3: Content Sections (English & German)

* [ ] **Section 1: Hero.** "Crafting High-End Digital Products."
* [ ] **Section 2: Social Proof.** Logos of SBB, PwC, CSS, MediData + Awards.
* [ ] **Section 3: The Trio.** Profiles for Nenad, Josip, and Bojan.
* [ ] **Section 4: Expertise.** Next.js, A11y, Design Systems.
* [ ] **Section 5: Featured Work.** Current highlights (SBB, Janzz).


Find the translated content in `./src/i18n/de.json` from german and `./scr/i18.en.json` for english

**Example implementation:**

````
---
const { lang = 'en' } = Astro.props;
const t = lang === 'de' ? deStrings : enStrings;
---
<h1>{t.hero.headline}</h1>
````

### Phase 4: Quality & Polish

* [ ] **Accessibility Audit:** Semantic HTML, ARIA labels, keyboard navigation.
* [ ] **Performance:** Image optimization (Astro `<Image />`), font subsetting.
* [ ] **Interactions:** Subtle scroll-reveal animations (Framer Motion or simple CSS).
* [ ] **Dark Mode:** Optional high-contrast mode for developers.

### Phase 5: Deployment

* [ ] Final Lighthouse check (Targeting 4x 100).
* [ ] Configure `neno.ch` domain and SSL.
* [ ] Setup form handling for "Let's work together."

## 🛠 Command Reference

* `npm run dev` — Start local dev server.
* `npm run build` — Build for production.
* `npm run preview` — Preview the production build.
* `npm run astro ...` — Run Astro CLI commands.

## 📝 Style & Guidelines

1. **Code Quality:** Senior-level code. Clean, modular, and well-commented.
2. **A11y First:** Every element must be accessible. No exceptions.
3. **Copywriting:** Professional, confident, and minimalist. Avoid "buzzword bingo."
4. **Performance:** Zero unnecessary JavaScript. Use Astro's "Zero JS by default" philosophy.
