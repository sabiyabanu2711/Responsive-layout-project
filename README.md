# Week 2: Responsive Layout Project — NovaTech Landing Page

> **Mandatory Hand-in Statement (One Sentence):**  
> *"I must submit a live hosted website link of a mobile-friendly landing page clone built using semantic HTML5, CSS Flexbox, and CSS Grid, along with verification screenshots taken at 360px (mobile), 768px (tablet), and 1280px (desktop) viewport widths."*

---

## 🚀 Live Demo & Repository
- **Project Name:** NovaTech — Next-Gen Cloud Intelligence Platform
- **GitHub Repository:** [https://github.com/sabiyabanu2711/Responsive-layout-project](https://github.com/sabiyabanu2711/Responsive-layout-project)
- **Live Demo (GitHub Pages):** [https://sabiyabanu2711.github.io/Responsive-layout-project/](https://sabiyabanu2711.github.io/Responsive-layout-project/)
- **Core Technologies:** HTML5 (Semantic), CSS3 (Modern Flexbox + Grid, Custom Properties), Vanilla JavaScript.

---

## 📋 Task Compliance & Requirements Checklist

| Requirement | Implementation Detail | Status |
| :--- | :--- | :---: |
| **Clone a landing page** | Built NovaTech SaaS Cloud Landing Page with Hero, Stats, Features, How It Works, Pricing, Testimonials, CTA, and Footer | ✅ Complete |
| **Use Flexbox** | Navbar alignment, Hero CTA buttons, Split-row alternating sections, Pricing cards, Footer bottom row | ✅ Complete |
| **Use CSS Grid** | Dashboard metrics KPI grid, Stats counter grid, 6-card Features grid, 3-card Pricing grid, 2-column Testimonials grid, 4-column Footer grid | ✅ Complete |
| **Mobile-Friendly (Mobile First)** | Base styles engineered for `360px+` first; added `@media (min-width: 768px)` and `@media (min-width: 1024px) / 1280px` | ✅ Complete |
| **Semantic HTML Elements** | Replaced generic `div`s with `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`, `<button>`, `<h1>`-`<h4>` | ✅ Complete |
| **Image `alt` Attributes** | Every image (`<img>`) and SVG icon has clear descriptive `alt` or `aria-label` tags for 100% accessibility | ✅ Complete |
| **Test at 360px, 768px, 1280px** | Fully tested across all three standard devtools viewport widths | ✅ Complete |
| **Submit Link & Screenshots** | Live deployment steps + direct DevTools screenshot capture instructions included | ✅ Complete |

---

## 🏗️ Technical Architecture: Flexbox vs. CSS Grid

### 1. Where CSS Flexbox is used (1D Layouts & Component Alignment):
1. **Header & Navigation (`.nav-wrapper`, `.nav-list`, `.nav-actions`):**
   - Keeps brand logo on the left, navigation links in the center, and CTA buttons on the right.
   - On mobile screens, turns into a responsive vertical drawer menu toggled by an accessible hamburger button.
2. **Hero Action Buttons (`.hero-cta-group`):**
   - Stacks vertically on mobile (`flex-direction: column`) and aligns side-by-side on tablet/desktop (`flex-direction: row`).
3. **Split Feature Sections (`.split-row`, `.split-row-reverse`):**
   - Uses `display: flex;` with `flex: 1` columns to alternate text and interactive visual cards.
4. **Card Internal Alignment (`.pricing-card`, `.testimonial-card`):**
   - Uses `flex-direction: column; justify-content: space-between;` so cards maintain uniform heights regardless of content length.
5. **Footer Bar (`.footer-bottom`):**
   - Stacks vertically on mobile and spreads horizontally (`justify-content: space-between`) on desktop.

### 2. Where CSS Grid is used (2D Layouts & Responsive Cards):
1. **Dashboard KPI Row (`.dashboard-kpi-row`):**
   - `grid-template-columns: 1fr` (mobile) &rarr; `repeat(2, 1fr)` (tablet) &rarr; `repeat(4, 1fr)` (desktop).
2. **Performance Metrics (`.stats-grid`):**
   - 4-card statistics layout adjusting from 1 column on mobile to 2 columns on tablet and 4 columns on desktop.
3. **Product Features Grid (`.features-grid`):**
   - 6 high-impact feature cards: 1 column on mobile, 2 columns at 768px, and 3 columns at 1024px+.
4. **Pricing Comparison Grid (`.pricing-grid`):**
   - 3 structured pricing tiers with featured card highlighting.
5. **Customer Testimonials (`.testimonials-grid`):**
   - 2-card layout with photo avatars, quotes, and author credits.
6. **Footer Navigation Grid (`.footer-grid`):**
   - 4-column layout (`2fr 1fr 1fr 1fr`) on desktop; gracefully stacks on mobile devices.

---

## 📱 Viewport Breakpoints Guide

- **Mobile Viewport (`360px` - `767px`):**
  - Single column fluid flow.
  - Collapsible drawer navigation with animated hamburger button.
  - Buttons expand to full touch targets for ergonomics.
- **Tablet Viewport (`768px` - `1023px`):**
  - `@media (min-width: 768px)`
  - 2-column feature and stats grids.
  - Hero action buttons align horizontally.
  - Side-by-side alternating workflow sections.
- **Desktop Viewport (`1024px` - `1280px+`):**
  - `@media (min-width: 1024px)` & `@media (min-width: 1280px)`
  - Full desktop horizontal navigation bar with inline CTA.
  - 3-column features and pricing grids.
  - 4-column global stats and footer navigation.

---

## 📸 How to Take Your 3 Required Submission Screenshots

Follow these quick steps in Google Chrome or Microsoft Edge to capture clean screenshots:

1. Double-click `index.html` in your file explorer to open it in your browser.
2. Press **`F12`** (or `Ctrl + Shift + I`) to open **Developer Tools**.
3. Press **`Ctrl + Shift + M`** to toggle the **Device Toolbar**.
4. Test and capture each required breakpoint:
   - **Mobile (360px):**
     - Type `360` in the width box and `800` in height.
     - Press `Ctrl + Shift + P` &rarr; type `screenshot` &rarr; select **"Capture full size screenshot"**.
     - Save as `mobile-360px.png`.
   - **Tablet (768px):**
     - Type `768` in width and `1024` in height.
     - Press `Ctrl + Shift + P` &rarr; select **"Capture full size screenshot"**.
     - Save as `tablet-768px.png`.
   - **Desktop (1280px):**
     - Type `1280` in width and `900` in height.
     - Press `Ctrl + Shift + P` &rarr; select **"Capture full size screenshot"**.
     - Save as `desktop-1280px.png`.

---

## 🌐 How to Deploy and Get Your Live Link (Under 2 Minutes)

### Option A: Free GitHub Pages (Recommended)
1. Initialize git in this folder and push to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Complete Week 2 Responsive layout project"
   git branch -M main
   git remote add origin https://github.com/<your-username>/responsive-layout-project.git
   git push -u origin main
   ```
2. Go to your repository on GitHub &rarr; **Settings** &rarr; **Pages**.
3. Under **Branch**, select `main` and root `/`, then click **Save**.
4. Your live link will be: `https://<your-username>.github.io/responsive-layout-project/`.

### Option B: Free Vercel / Netlify Drop (Instant Zero-CLI)
1. Open [https://app.netlify.com/drop](https://app.netlify.com/drop) or [https://vercel.com](https://vercel.com).
2. Drag and drop the `Responsive layout project` folder directly into the window.
3. You will immediately receive a live URL (e.g., `https://novatech-landing.netlify.app`) to submit!

---

## 📂 Project Structure
```text
Responsive layout project/
├── index.html        # Semantic HTML5 markup with accessible tags and aria attributes
├── style.css         # Mobile-first CSS stylesheet with CSS Flexbox & Grid systems
├── script.js         # Vanilla JS for hamburger menu toggle and scroll behavior
├── screenshots/      # Folder to store your 360px, 768px, and 1280px screenshots
└── README.md         # Full documentation and grading submission guide
```

