---
layout: default
title: Bank Imports Qif Ofx
parent: Setup & Integrations
nav_order: 2
grand_parent: Documents
---

# Bank Imports Qif Ofx

title: Bank Imports (QIF/OFX)

## tags: [bank, qif, ofx, csv]

When your bank export is messy CSV, convert to **QIF** or **OFX** first.

## Quick path

- **QIF**: use `csv2qif-py` (Python) or `csv2qif-ts` (Node).

- **OFX**: use `ofxtools` (Python) or `ofxstatement` (CLI with plugins).

### Minimal working headers (CSV → QIF)

```text
Date,Payee,Amount,Memo
2025-01-05,"CANADA POST",-12.34,"stamps"

```text
text
> Map your bank’s debit/credit columns to a single signed **Amount**.

### Minimal working headers (CSV → OFX via ofxstatement)
Use a plugin for your bank, or a generic CSV plugin config (see `templates/ofxstatement.ini`).

## Sage import

1. Back up the company file.

2. Bank Reconciliation → Import → choose **QIF**/**OFX**.

3. Verify the date range, then map unmatched payees to accounts/vendors. Save mappings for future imports.
