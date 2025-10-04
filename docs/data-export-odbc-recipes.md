---
layout: default
title: Data Export Odbc Recipes
parent: Setup & Integrations
nav_order: 40
---
# Data Export Odbc Recipes

title: Data Export via ODBC — Recipes

## tags: [odbc, export, sql]

> Use an ODBC client (e.g., Python `pyodbc`, DBeaver, or even Excel) to run **read-only** queries.

## Examples (pseudo-table names; inspect your DSN for actual table names)


- **GL transactions (by date range)**
```sql
SELECT TxnDate, Source, Account, Debit, Credit, Memo
FROM GLTransactions
WHERE TxnDate BETWEEN '2025-01-01' AND '2025-01-31'
ORDER BY TxnDate, Source;
```
text

- **Customer list**
```sql
SELECT CustomerID, Name, Email, Phone, Terms
FROM Customers
ORDER BY Name;
```
text

- **Supplier list**
```sql
SELECT VendorID, Name, Email, Phone, Terms
FROM Vendors
ORDER BY Name;
```
text
