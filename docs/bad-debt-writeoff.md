---
layout: default
title: Bad Debt Write-off
parent: Processes
nav_order: 80
---
# Bad Debt Write-off

---
title: "Bad Debt Write-Off Workflow"
tags: [sage50, bookkeeping, canada, bad-debt, workflow]
type: workflow
status: final
---

# Bad Debt Write-Off (Sage 50 Canadian)

This workflow explains how to handle customer invoices that will never be paid, including the GST/HST reversal.

---

## Accounts Used
- **Accounts Receivable** (customer subledger)
- **Bad Debts Expense** (new or existing expense account)
- **2310 HST charged on Sales** (to reverse tax)
- Customer record (mark as inactive after write-off)

---

## Step 1. Confirm Bad Debt
- Ensure the invoice is overdue > 1 year with no likelihood of payment.
- Verify customer reminders and communication are documented.
- CRA requires reasonable evidence of uncollectibility to claim back HST.

---

## Step 2. Enter Credit Note
- Go to **Receivables → Sales Invoicing → Credit Note**.
- Customer: Select the debtor.
- Reference: `Bad Debt Write-off – [Invoice #]`
- Date: [date of decision].
- Lines:
  ```
  Line 1: Bad Debts Expense    (for the invoice subtotal)
  Line 2: 2310 HST charged     (for the HST originally charged, as negative)
  ```
- Total = full invoice balance.

---

## Step 3. Apply Credit Note
- Apply the credit note against the unpaid invoice.
- Customer A/R balance becomes **zero**.
- A/R Aging report is cleaned.

---

## Step 4. Reporting Effects
- **Income Statement:** Bad Debts Expense increases (reduces net income).
- **Balance Sheet:** Accounts Receivable decreases.
- **GST/HST:** Original HST remitted is reversed, so it is recovered on the next return.

---

## Step 5. Prevent Future Issues
- Mark customer as **inactive** in Receivables.
- Keep documentation in case of CRA audit.

---
