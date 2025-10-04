---
layout: default
title: Odbc Setup Windows
parent: Setup & Integrations
nav_order: 60
---
# Odbc Setup Windows

---
title: ODBC Setup (Windows)
tags: [odbc, windows, sage50, canada]
---

# ODBC Setup (Windows) for Sage 50 Canada

1. Install Sage 50 (Canadian Edition) on the machine with the company dataset.
2. Open **ODBC Data Sources (64-bit)**. Create a **System DSN** using *Sage 50* ODBC Driver.
3. Point the DSN at your Sage 50 company file folder (*.SAI + .SAJ* directory).
4. Test connection with the *Query* button or via a basic ODBC client.
5. Use **read-only** queries for exports/reporting. Write access generally requires the Sage SDK/Partner program.

> Tip: Keep driver/version notes with the DSN name, e.g., `Sage50CA_v2025_RO`.
