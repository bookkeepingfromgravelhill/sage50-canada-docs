# Practical **checklists, setup guides, and workflows** for Sage 50 (Canadian Edition)

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

```


## Contributing

- Write pages in Markdown in `/docs/` with clear headings.

- Each page includes a small YAML front‑matter block to place it in the left‑hand navigation.

- Keep file names **kebab‑case** (e.g., `month-end-checklist.md`).

## Licenses

- **Docs**: CC BY 4.0 — see `LICENSES/DOCS-CC-BY-4.0.txt`

- **Templates**: CC0 1.0 — see `LICENSES/TEMPLATES-CC0-1.0.txt`
