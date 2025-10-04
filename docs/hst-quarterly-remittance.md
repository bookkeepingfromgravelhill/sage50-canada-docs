---
layout: default
title: HST Quarterly Remittance
parent: Checklists
nav_order: 6
---

# HST Quarterly Remittance

title: "HST Quarterly Remittance Workflow"
tags: [sage50, bookkeeping, canada, hst, workflow]
type: workflow

## status: final

This workflow explains how to remit HST to the CRA each quarter using **Payables Invoices**. It covers both **amount owing** and **refund** cases.

## Accounts Used

- **2310 – HST charged on Sales** (liability, tax collected)

- **2315 – HST paid on Purchases** (asset, input tax credits)

- **Receiver General – HST** (vendor in Payables)

## Step 1. Run Reports

- Pull balances for **2310** and **2315** at quarter end.

- Calculate net:

```text
  Net HST = 2310 – 2315

```text
text

- Positive result = you **owe CRA**.

- Negative result = CRA **owes you (refund)**.

## Step 2. Enter Payables Invoice

### If You Owe CRA

- Go to **Payables → Enter Purchase Invoice**.

- Vendor: `Receiver General – HST`

- Reference: `Q[quarter/year] HST Filing`

- Date: [Quarter end date]

- Lines:

```text
text
  Line 1: 2310 HST charged on Sales     (positive, full balance)
  Line 2: 2315 HST paid on Purchases    (negative, full balance)

```text
text

- Invoice Total = Net owing.

### If CRA Owes You (Refund)

- Go to **Payables → Enter Purchase Credit Note**.

- Vendor: `Receiver General – HST`

- Reference: `Q[quarter/year] HST Refund`

- Lines:

```text
text
  Line 1: 2310 HST charged on Sales     (positive, full balance)
  Line 2: 2315 HST paid on Purchases    (negative, full balance)

```text
text

- Invoice Total = Net refund (negative balance).

## Step 3. Record Settlement

### Owing CRA

- Go to **Payables → Payments**.

- Select `Receiver General – HST`.

- Apply payment to invoice (Net owing).

- Bank decreases, Payables clears.

### Receiving Refund

- Go to **Payables → Payments**.

- Enter **negative payment** (deposit).

- Bank increases, Payables clears.

## Notes

- Always enter **2310 as positive** and **2315 as negative**.

- The net result must equal the CRA remittance/refund.

- This method avoids using Receivables and keeps CRA properly in Payables.
