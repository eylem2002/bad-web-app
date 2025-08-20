# Bad Web App — Balanced Workload Edition

This version spreads the mess evenly across **Header/Nav**, **About**, **Gallery**, **Contact**, and **Footer** so 3 students can split work fairly.

## Team of 3 — Equal Work Split

Create **three branches** and divide responsibilities so each student has similar effort. Example:

- Student A — **Structure & Semantics**

  - Convert table/inline-styled header & footer to semantic HTML (`<header> <nav> <footer>`).
  - Replace `<font>`, underline, inline styles with classes.
  - Add the correct `<meta name="viewport">`.
  - Fix heading hierarchy.
  - Remove deprecated tags and ensure one `<h1>`.

- Student B — **CSS & Box Model**

  - Resolve conflicting `box-sizing` and remove `!important`.
  - Remove inline styles; move to CSS.
  - Standardize spacing/typography/colors; improve contrast.
  - Replace fixed widths with responsive units (`%`, `rem`, `minmax()`, `vw/vh`).
  - Add subtle, consistent transitions (no harsh effects).

- Student C — **Layout, Forms & Responsive**
  - Replace gallery floats + fixed px with responsive **CSS Grid** (`auto-fit/auto-fill`).
  - Rework Contact form into a clean **two-column** on desktop, single column on mobile.
  - Properly associate `<label for="">`/`id` on inputs.
  - Add HTML5 attributes where needed (`required`, `min`, `max`, `pattern`) — **NOTE:** the starter has **no checks**; you must add them.
  - Add accessible focus states and tidy button styles.

> All students should also test across widths and ensure no horizontal scroll on mobile (make sure it's responsive)

## Git Workflow (each student)

```bash
git clone <repo-url>
cd bad-web-app-balanced
git checkout -b improve-<your-name>
# Work in small commits
git add .
git commit -m "feat: [short clear message]"
git push -u origin improve-<your-name>
# open a PR to main, request reviews, iterate, then merge
```

## Deliverables

- Clean, semantic HTML (no tables for layout, no deprecated tags).
- Organized CSS (no inline styles, no `!important`, coherent scale).
- Responsive layout (header/about/gallery/contact/footer).
- **Form with proper labels and HTML5 validation** (you implement it).
- PRs reviewed by peers before merging.
