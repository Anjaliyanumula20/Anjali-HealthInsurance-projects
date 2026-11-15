# Health Insurance – Policy Renewal Management Dashboard

An Excel practice project that monitors upcoming expiries, pending payments, completed renewals and overdue policies, the way a **Renewal team** in health insurance operations would.

> **Note:** All customer names, policy numbers and figures are **made-up sample data**. The 30-day due-soon window and 30-day grace period are assumed values and can be changed on the `Assumptions` sheet.

**File:** `Health_Insurance_Renewal_Management_Dashboard.xlsx`

## What it does

- Records policy expiry date, details verification, customer contact, premium status and renewal date
- Calculates **days to expiry** and **renewal status**: **Renewed, Upcoming, Due Soon, Overdue, Lapsed**
- Suggests the **next action required**: verify details, contact customer, follow up premium payment, process renewal, or escalate for reinstatement
- Dashboard shows renewal rate, premium collected vs premium at risk, lapse rate, pending follow-ups, expiries by month and renewal performance by plan

## Business logic

| Status | Rule |
|---|---|
| Renewed | Renewal date is filled |
| Upcoming | Expiry is more than 30 days away |
| Due Soon | Expiry within the next 30 days |
| Overdue | Expired, within the 30-day grace period |
| Lapsed | Expired beyond the grace period |

## Workbook structure

| Sheet | Purpose |
|---|---|
| `Dashboard` | KPI cards, summary tables and charts |
| `Renewals` | 40 sample policies (blue text = input, black text = formula) |
| `Assumptions` | As-on date, due-soon window, grace period and dropdown lists |

## Excel skills used

- **Formulas:** `IF`, `COUNTIF`, `COUNTIFS`, `SUMIFS`, `IFERROR`, `EDATE`, `TEXT`
- **Date logic:** days to expiry, grace period and monthly expiry grouping
- **Data validation:** dropdown lists for plan, details verified, customer contacted and premium status
- **Conditional formatting:** colour-coded renewal statuses
- **MIS reporting:** formula-driven summary tables (Pivot-style) and charts
- **Filters and frozen panes** for easy review

## How to use

1. Open the file in Excel.
2. On the `Assumptions` sheet, set the **as-on date**, due-soon window and grace period.
3. Edit or add rows on the `Renewals` sheet using the blue input columns. Leave **Renewal Date** blank until the policy is renewed (copy the formula columns down for new rows).
4. Open the `Dashboard` sheet to see updated KPIs and charts.

## Key learnings

- How renewal tracking works: expiry monitoring, customer follow-up, payment status, lapse risk
- How to prioritise open cases by status and next action
- Building clean, formula-driven MIS reports in Excel

## Author

**Anjali Yanumula** | M.A. Economics | Mumbai
[LinkedIn](https://www.linkedin.com/in/anjali-yanumula-1b4393325) | [GitHub](https://github.com/Anjaliyanumula20)
