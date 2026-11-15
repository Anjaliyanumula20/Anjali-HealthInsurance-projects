# Health Insurance – New Business Application Tracker & Dashboard

An Excel practice project that tracks new health insurance applications from receipt to policy issuance, the way a **New Business (NB) operations** team would.

> **Note:** All customer names and figures are **made-up sample data**. The SLA target (5 days) is an assumed value and can be changed on the `Assumptions` sheet.

**File:** `Health_Insurance_NB_Application_Tracker.xlsx`

## What it does

- Records applications with plan, sum insured, channel, KYC status, proposal form status, medical documents and premium payment
- Automatically checks documents (`Complete` / `Pending`)
- Assigns an application stage: **Docs Pending, Payment Pending, Ready to Issue, Policy Issued, Rejected**
- Calculates **TAT (days)** from application date to policy issuance and flags **SLA breaches**
- Dashboard shows total applications, policies issued, pending cases, average TAT, SLA compliance %, rejection rate, and summaries by stage, plan, channel and KYC status

## Business logic

| Stage | Rule |
|---|---|
| Rejected | KYC status is Rejected |
| Docs Pending | KYC not verified, proposal incomplete, or medical documents pending |
| Payment Pending | Documents complete but premium not paid |
| Ready to Issue | Documents complete and premium paid, policy not yet issued |
| Policy Issued | Policy issue date is filled |

## Workbook structure

| Sheet | Purpose |
|---|---|
| `Dashboard` | KPI cards, summary tables and charts |
| `Applications` | 40 sample applications (blue text = input, black text = formula) |
| `Assumptions` | As-on date, SLA target and dropdown lists |

## Excel skills used

- **Formulas:** `IF`, `AND`, `COUNTIF`, `COUNTIFS`, `SUMIFS`, `AVERAGEIFS`, `IFERROR`, `TEXT`
- **Data validation:** dropdown lists for plan, channel, KYC status, proposal, medical docs and premium paid
- **Conditional formatting:** colour-coded stages and SLA breaches
- **MIS reporting:** formula-driven summary tables (Pivot-style) and charts
- **Filters and frozen panes** for easy review

## How to use

1. Open the file in Excel.
2. On the `Assumptions` sheet, set the **as-on date** and **SLA target**.
3. Edit or add rows on the `Applications` sheet using the blue input columns (copy the formula columns down for new rows).
4. Open the `Dashboard` sheet to see updated KPIs and charts.

## Key learnings

- How NB processing flows: application, KYC and document verification, payment, policy issuance
- How TAT and SLA are measured and reported in operations
- Building clean, formula-driven MIS reports in Excel

## Author

**Anjali Yanumula** | M.A. Economics | Mumbai
[LinkedIn](https://www.linkedin.com/in/anjali-yanumula-1b4393325) | [GitHub](https://github.com/Anjaliyanumula20)
