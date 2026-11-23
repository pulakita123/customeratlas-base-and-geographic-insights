# Assumptions, Limitations & Next Steps

## Project status
This is an Excel-based descriptive customer analytics project. The repository contains an original CSV, a cleaned CSV, an Excel workbook and a dashboard preview.

## Assumptions to validate
- The intended unit of analysis is one customer, or the workbook has a defined method for counting distinct customers.
- Subscription year is derived from a valid subscription date.
- Tenure is calculated using a documented reference date.
- Country and company labels can be standardised without losing meaningful distinctions.
- The year, country and company slicers filter the intended dashboard elements.

## Data and evidence limitations
- The large CSV contents could not be independently inspected during this documentation update.
- The internal formulas, PivotTables, data model and dashboard interactions in the Excel workbook have not been independently audited.
- Exact column names, row counts, duplicate-removal rules and missing-value treatment need confirmation.
- Numerical dashboard values and rankings have not been recalculated here.
- The analysis does not include revenue, costs, churn events, satisfaction, contract value or transaction-level behaviour.

## What this project cannot establish
- Customer lifetime value or profitability
- Actual churn or retention rate
- Customer satisfaction or loyalty
- Reasons for acquisition trends
- Causal drivers of customer growth
- Future customer behaviour

## Recommended next steps
1. Validate source and cleaned CSV row counts and exact column names.
2. Confirm the unique customer key and duplicate-handling logic.
3. Document the tenure formula, reference date and tenure-band boundaries.
4. Reconcile each dashboard KPI with its source PivotTable or formula.
5. Add exact numeric findings and ranked segments only after validation.
6. Test slicers and confirm that all dashboard visuals respond correctly.
7. Extend the analysis with revenue, renewal, churn or engagement data if available.
8. Capture a clear dashboard screenshot and, if appropriate, a short walkthrough for the repository.

## Reproducibility note
The Excel workbook is the primary analysis artefact. A reviewer should be able to open it and inspect the PivotTables, formulas, filters and dashboard. The README links to the original and cleaned datasets so the preparation and analysis inputs are visible.
