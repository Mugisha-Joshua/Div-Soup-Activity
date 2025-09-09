# Semantic HTML Refactor Guidelines

This project involves refactoring `index.html` into a semantic version named `index.semantic.html`.
The goal is to improve **accessibility, readability, and standards compliance** using semantic HTML5 elements.

---

## 1. Refactor to Semantic HTML

Use **semantic elements** where appropriate:

* `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<aside>`, `<footer>`

### Element Replacements

* `.title` → use appropriate **`<h1>`–`<h6>`** (follow logical document outline, no heading level jumps).
* `.meta` → replace with **`<p>`**, `<time>`, or other inline semantic elements.
* `.image` → wrap inside **`<figure>`** and include `<figcaption>` if the image conveys information.
* `.quote` → use **`<blockquote>`** (with optional `cite` attribute).
* `.related` → convert to a **`<section>`** with its own heading and a list of related links or items.

  * Choose one consistent structure:

    * `ul > li > article`, **or**
    * `ul > li > a`.
* `.cards` / `.card` → refactor into semantic groupings:

  * `<section>`, `<article>`, or `<li>` depending on context.
* Sidebar → use `<aside>`.

### Forms & Inputs

* Ensure search controls have a **visible `<label>`** (not placeholder-only).

---

## 2. Landmarks & Accessible Names

### Landmarks

* Exactly **one `<main>`** element per page.
* Keep the **skip link** and point it to `#main`.

### Accessible Naming

* Add `aria-label` when no visible heading exists.
  Example:

  ```html
  <nav aria-label="Primary">
  ```

---
