# Methodology & Data Quality

## 1. Data understanding
The repository includes an original CSV, a cleaned CSV and an Excel workbook. The project description identifies customer distribution, subscription year and tenure as analysis themes.

Before extending the analysis, I would inspect the exact headers, data types, row grain and date formats in the workbook and both CSV files. The source files are the authority for field names; this document intentionally does not invent column names.

## 2. Data preparation checks
The original project notes describe the following preparation activities:

- Check for duplicate customer records.
- Identify invalid or incomplete records.
- Standardise country and company labels.
- Create a subscription-year field from the relevant date field, where available.
- Create tenure values or tenure buckets using a consistent reference date.
- Validate counts after cleaning.

For a reproducible workflow, the project should record the number of rows before and after each cleaning step, the duplicate-handling rule, missing-value treatment and any excluded records.

## 3. Derived fields
Two derived concepts are described in the project:

**Subscription year:** the calendar year associated with the customer's subscription date. The exact date field and treatment of missing or invalid dates must be confirmed from the workbook.

**Customer tenure:** the elapsed time between the subscription date and a chosen reporting reference date. The reference date must be stated because tenure changes over time. If tenure buckets are used, their boundaries should be documented.

## 4. Analysis
PivotTables are used to summarise customer counts by subscription year, country, company and tenure grouping. Slicers provide interactive filtering by year, country and company.

For each summary, I would verify that:
- the aggregation counts customers rather than unrelated rows;
- each customer is counted at the intended grain;
- blank or unknown categories are handled consistently;
- filtered totals reconcile to the underlying customer records.

## 5. Dashboard design
The dashboard is intended to provide:
- high-level KPI cards;
- customer additions by subscription year;
- tenure distribution;
- country and company breakdowns;
- slicers for year, country and company.

The goal is to make the overall picture readable first, while allowing a reviewer to investigate a selected segment.

## 6. Validation checklist
- Compare original and cleaned row counts.
- Check duplicate customer identifiers, if an identifier exists.
- Review missing values in fields used by the dashboard.
- Check standardised country and company labels.
- Reconcile KPI cards to PivotTable totals.
- Test slicers individually and in combination.
- Confirm that tenure calculations use the intended reference date.

## Evidence limitation
The large CSV files could not be independently inspected during this documentation update. The exact headers, row count, cleaning decisions, formulas, PivotTable configuration and numerical outputs therefore remain to be verified against the Excel workbook. This document describes the analysis approach rather than claiming an independent audit of those details.
