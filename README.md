Review Assignment Due Date Open in Codespaces

Semantic HTML Refactor Guidelines
This project involves refactoring index.html into a semantic version named index.semantic.html.
Follow the rules below to ensure accessible, semantic, and standards-compliant HTML.

1. Refactor to Semantic HTML
Use semantic elements where appropriate:
header, nav, main, article, section, aside, footer.

Replace generic wrappers with semantic structures:

.title → appropriate h1–h6 (logical outline, no heading jumps).
.meta → use p, time, or relevant semantic inline elements.
.image → wrap in <figure> with <figcaption> if it conveys information.
.quote → use <blockquote> (optionally with cite).
.related → a <section> with its own heading and list.
Choose one structure for related links and be consistent:
ul > li > article
or ul > li > a.
.cards, .card → semantic grouping using section, article, or li.
Convert the sidebar into an <aside>.

Ensure the search control has a proper <label> (not placeholder-only).

2. Landmarks & Names
Exactly one <main> element per page.
Keep the skip link and point it to #main.
Add accessible names where needed:
Example: <nav aria-label="Primary"> if no visible nav heading exists.