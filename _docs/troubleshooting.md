---
layout: default
title: Troubleshooting
parent: Processes
nav_order: 3
---

# Troubleshooting

title: Troubleshooting & Gotchas

## tags: [tips, troubleshooting]

- **ODBC driver mismatch**: 32‑bit vs 64‑bit DSN. Ensure your querying tool matches the driver bitness.

- **Read‑only ODBC**: Most open approaches are read‑only. Writing typically requires the Sage SDK.

- **Weird date formats**: Normalize to ISO `YYYY‑MM‑DD` before converting to QIF/OFX.

- **Bank CSV quirks**: Separate `Debit`/`Credit` columns? Convert to a single signed **Amount**.

- **Vendor name chaos**: Save mapping rules; maintain a `Vendors Mapping` note for consistency.
