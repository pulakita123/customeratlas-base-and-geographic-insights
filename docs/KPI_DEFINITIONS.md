# KPI Definitions & Interpretation

This project is intended to describe the customer base. The following definitions should be used consistently in the workbook and any future reporting.

| KPI | Suggested definition | Interpretation note |
|---|---|---|
| Total customers | Count of distinct customer identifiers in the selected dataset | Use a distinct count if the source can contain multiple rows per customer |
| New customers by year | Distinct customers grouped by subscription year | Confirm the date field and treatment of missing dates |
| Average customer tenure | Average elapsed time between subscription date and reporting reference date | State the reference date and unit (months or years) |
| Customers by country | Distinct customer count grouped by standardised country | Define treatment of blank or unknown country values |
| Customers by company | Distinct customer count grouped by standardised company | Confirm whether one customer can be associated with multiple companies |
| Tenure distribution | Distinct customer count grouped into documented tenure bands | State band boundaries and reference date |

## Suggested calculation logic

- **Customer share by category:** customers in category ÷ total customers in current filter context × 100.
- **Year-over-year change:** (current-year new customers − previous-year new customers) ÷ previous-year new customers × 100, where the prior-year value is non-zero.
- **Average tenure:** sum of customer tenure values ÷ number of valid customer tenure values.

These are calculation definitions, not verified workbook formulas. They should be reconciled against the actual PivotTables and formulas before being reported as final metrics.

## Reporting rules to agree
- What uniquely identifies a customer?
- Does the report include inactive or historical customer records?
- What is the tenure reference date?
- Are blank country/company values included as an Unknown category?
- Are year comparisons based on full calendar years or partial years?
- How should customers with multiple company or country associations be counted?

## Avoid over-interpreting
Customer count is not revenue. Tenure is not proof of loyalty. A large country or company share is a concentration signal, not automatically a risk. Acquisition patterns alone do not explain why customers joined.
