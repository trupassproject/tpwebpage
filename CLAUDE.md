# TruPASS site (trupass.eu) — editing guide

Static site, no build step. Design, wording and layout are final: change them only when explicitly asked.

| Task | Edit only |
|---|---|
| Add news | `news.html` — paste a new `<article class="post">` right under the HOW TO comment (template is inside it). Newest first. Photos go next to `news.html`; set `width`/`height` to the real pixel size. |
| Partners | `index.html`, section `id="partners"`; logos live in `assets/partners/` |
| Page copy | `index.html`, locate the section by its `id` with Grep and edit that block only |
| Styling | `css/style.css` (colours are variables in `:root`) |

Rules: never invent dates, links or partners; do not link LinkedIn from news items (the LinkedIn page is linked in the footer only); tags are `event`, `publication` or `announcement`. Do not read `index.html` for a news task. Preview: `python -m http.server 8741` in this folder.
