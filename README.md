Practical **checklists, setup guides, and workflows** for Sage 50 (Canadian Edition).
This repository also publishes a GitHub Pages documentation site using the **Just the Docs** theme.

## Contents

- **Checklists**: Month‑end, year‑end, HST remittance, sign‑offs
- **Setup & Integrations**: ODBC, QIF/OFX, GST/HST, bank/data export recipes
- **Processes**: Reconciliations, payroll basics, troubleshooting
- **Templates**: CSV/INI files and sign‑off forms (`/templates/`), plus one PDF in `/assets/files/`

## Local structure


```text
/
├─ _config.yml            # Jekyll settings (Just the Docs)
├─ index.md               # Site landing page
├─ docs/                  # All documentation pages (Markdown)
├─ templates/             # Templates and example files
├─ assets/files/          # Downloadable PDFs and attachments
├─ LICENSES/              # License files
└─ .github/workflows/     # Linting workflows (markdownlint, link check)

```text
## How to publish with GitHub Pages

1. Push to the `main` branch.
2. In **Repository → Settings → Pages**:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` / **root** (`/`)
3. GitHub will build the site (Jekyll + remote theme `just-the-docs/just-the-docs`).

### Linking from the main site (ledger.fromgravelhill.ca)

To have a `/doc/` path on the main site point to these docs, add a redirect page in your main site repo
[`bookkeepingfromgravelhill/bookkeepingfromgravelhill.github.io`](https://github.com/bookkeepingfromgravelhill/bookkeepingfromgravelhill.github.io):

Create `doc/index.html` with:


```html
<!doctype html>
<meta charset="utf-8">
<meta http-equiv="refresh" content="0; url=https://bookkeepingfromgravelhill.github.io/sage50-canada-docs/">
<link rel="canonical" href="https://bookkeepingfromgravelhill.github.io/sage50-canada-docs/">
<title>Redirecting…</title>
<a href="https://bookkeepingfromgravelhill.github.io/sage50-canada-docs/">Redirecting to docs…</a>

```text
(If you later add a `CNAME`/custom domain for the docs, update the URL in the redirect accordingly.)

## Contributing

- Write pages in Markdown in `/docs/` with clear headings.
- Each page includes a small YAML front‑matter block to place it in the left‑hand navigation.
- Keep file names **kebab‑case** (e.g., `month-end-checklist.md`).

## Licenses

- **Docs**: CC BY 4.0 — see `LICENSES/DOCS-CC-BY-4.0.txt`
- **Templates**: CC0 1.0 — see `LICENSES/TEMPLATES-CC0-1.0.txt`
