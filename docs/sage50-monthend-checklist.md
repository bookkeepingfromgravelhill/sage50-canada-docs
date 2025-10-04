---
layout: default
title: Month-End Checklist (Alternate)
parent: Checklists
nav_order: 60
---
# Month-End Checklist (Alternate)
##
title: "Sage 50 Canadian — Month-End (Unified Checklist + Filing Reference)"
date: 2025-10-02
tags: [accounting, sage50, month-end, checklist, filing]

## status: final

> Use this at each month-end to post activity, reconcile accounts, save standard reports, file documents (digital + physical), and lock the period.

## 1) Pre-Close

- [ ] Post all **sales** invoices & receipts (Customers & Sales).
- [ ] Post all **purchase** invoices & payments (Vendors & Purchases).
- [ ] Post **payroll** (or record manual payroll JEs if using external payroll).
- [ ] Post **accruals/deferrals** (insurance, leases, subscriptions, WIP).
- [ ] Quick review for **duplicates/mispostings**; clear suspense/clearing accounts.
- [ ] Backup: `PRE-MONTHEND-{{YYYY-MM}}.cab`.

## 2) Reconciliations

- [ ] **Bank** accounts reconciled to statement date (Reports → Banking → Account Reconciliation).
- [ ] **Credit card(s)** reconciled (Reports → Credit Cards → Account Reconciliation).
- [ ] **Petty cash** counted / reconciled (if applicable).
- [ ] **A/R subledger = A/R control** (Aged Receivables vs GL).
- [ ] **A/P subledger = A/P control** (Aged Payables vs GL).
- [ ] **Undeposited funds / clearing** accounts are **zero** at close.

## 3) Reviews

- [ ] **A/R Aging**: follow up past-due; note expected collections.
- [ ] **A/P Aging**: schedule payments; take discounts where available.
- [ ] **Inventory valuation** agrees to GL (if inventory tracked).
- [ ] **GST/HST/PST**: prepare file if period ends; confirm GL tie-out.
- [ ] **Projects/Jobs (WIP)** reviewed and posted (if used).

## 4) Standard Reports to Save (PDF or Excel)
Save into: `/Finance/MonthEnd/{{YYYY-MM}}/Month-End Reports/`

**Bank & Credit Card**

- [ ] Bank Reconciliation Report — *Reports → Banking → Account Reconciliation*
- [ ] Credit Card Reconciliation Report — *Reports → Credit Cards → Account Reconciliation*

**Aged Reports**

- [ ] Aged Receivables (as of month-end) — *Reports → Customers & Sales → Aged Receivables*
- [ ] Aged Payables (as of month-end) — *Reports → Vendors & Purchases → Aged Payables*

**Financials**

- [ ] Income Statement (month & YTD) — *Reports → Financials → Income Statement*
- [ ] Balance Sheet (as of month-end) — *Reports → Financials → Balance Sheet*

**Ledgers**

- [ ] General Ledger Detail (month) — *Reports → General Ledger → General Ledger Detail*
- [ ] Vendor Ledger (optional) — *Reports → Vendors & Purchases → Vendor Ledger*
- [ ] Customer Ledger (optional) — *Reports → Customers & Sales → Customer Ledger*

**Taxes**

- [ ] Sales Tax Report — *Reports → Taxes → Sales Tax Report*

**Payroll (if no Sage Payroll add-on)**

- [ ] Payroll Expense GL Detail (filter payroll accounts) — *Reports → General Ledger → General Ledger Detail*

**Naming convention**

- Save as: `{{YYYY-MM}} - {{ReportName}}.pdf` (e.g., `2025-09 - Aged Receivables.pdf`).

## 5) Filing & Archiving

### A) Physical (Monthly Binder + Source Documents)

- **Binders (tabbed):** Bank, Credit Card, Receivables, Payables, Financials, Ledgers, Taxes, Payroll.
- **Source folders:** Bank, Credit Card, Sales, Purchases, Receipts, CRA.
- **Stamps:**
  - *Posted* → only after entry verified in Sage.
  - *Paid* → only after payment clears.
- **Highlighting:** Color 1 = Invoice #; Color 2 = Final Total.
- **Owner initials** month-end binder checklist for accountability.

### B) Digital (Consistent Tree + Backups)

- **Folder structure:** `…/Finance/{{YYYY}}/{{YYYY-MM}}/{Bank Statements|Credit Card Statements|Sales Invoices|Purchase Invoices|Receipts|CRA|Month-End Reports}`
- **File names:** `{{YYYY-MM-DD}} - {{Vendor}} - {{Type}} - {{Amount}}.pdf`
- **Backups:**
  - Save Sage backups to `…/Finance/Backups/` as `{{YYYY-MM-DD}} - {{Company}} - Backup.cab`
  - Store **in two locations** (local + cloud/external).

### C) Best Practices

- Use the **same names/structure** every month.
- **Scan fragile/fading receipts** immediately.
- **Purge duplicates**; retain only what’s required (CRA: **7 years**).
- Lock months in Sage after reconciliations (see §7).

## 6) Completion Checks

- [ ] All reports saved (digital) and filed (binder).
- [ ] All receipts/invoices filed physically & digitally.
- [ ] AR/AP reconciliations match GL controls.
- [ ] Sales tax return prepared (if period end) and GL ties.

## 7) Close & Lock

- [ ] Backup: `POST-MONTHEND-{{YYYY-MM}}.cab`.
- [ ] **Lock prior dates** to prevent changes (Settings → Company → System).
- [ ] Roll recurring entries/memos needed for next month.
