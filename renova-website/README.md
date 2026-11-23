# Renova Global Solutions: website prototype

Single-file static site (`index.html`): HTML, CSS and vanilla JS. No build step, no dependencies beyond Google Fonts.

## Run locally
Open `index.html` in a browser, or run `npx serve .`

## Deploy
Import the repository in Vercel (framework preset: Other, no build command). Output directory: `.` (root).

## Before launch
- **Quotation form:** set `CFG.endpoint` at the top of the `<script>` to a form backend URL (Formspree, a Vercel function, etc.). Until then the form falls back to opening the visitor's email app (`mailto:`).
- **Indexing:** `vercel.json` sends `X-Robots-Tag: noindex` while this is a prototype. Remove that header at launch.
- **Content to supply:** client imagery, Regina Ndunge's biography, partner details beyond Ginnah's Bakery, strategic priorities.
- **Contact details** (`CFG.wa`, `CFG.email`) and **services** (`S` array) are editable in the script.
