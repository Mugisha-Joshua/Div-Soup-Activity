[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/-J_txwUd)
[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=20290025)
# Semantic HTML Refactor Guidelines

This project involves refactoring `index.html` into a semantic version named **`index.semantic.html`**.  
Follow the rules below to ensure accessible, semantic, and standards-compliant HTML.

---

## 1. Refactor to Semantic HTML

- Use semantic elements where appropriate:  
  `header`, `nav`, `main`, `article`, `section`, `aside`, `footer`.

- Replace generic wrappers with semantic structures:
  - `.title` → appropriate `h1–h6` (logical outline, no heading jumps).
  - `.meta` → use `p`, `time`, or relevant semantic inline elements.
  - `.image` → wrap in `<figure>` with `<figcaption>` if it conveys information.
  - `.quote` → use `<blockquote>` (optionally with `cite`).
  - `.related` → a `<section>` with its own heading and list.
    - Choose **one** structure for related links and be consistent:  
      - `ul > li > article`  
      - *or* `ul > li > a`.
  - `.cards`, `.card` → semantic grouping using `section`, `article`, or `li`.

- Convert the sidebar into an `<aside>`.

- Ensure the **search control** has a proper `<label>` (not placeholder-only).

---

## 2. Landmarks & Names

- Exactly **one `<main>`** element per page.
- Keep the **skip link** and point it to `#main`.
- Add accessible names where needed:
  - Example: `<nav aria-label="Primary">` if no visible nav heading exists.
