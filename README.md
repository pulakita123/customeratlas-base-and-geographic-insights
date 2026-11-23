# CustomerAtlas: Customer Base & Geographic Insights | Excel

An Excel-based customer analytics project focused on understanding customer growth, tenure and the distribution of a customer base across countries and companies.

I approached this as a business reporting problem: turn a customer-level dataset into a set of clear measures and interactive views that help a business understand who its customers are, how the base has changed over time, and where the customer base is concentrated.

![Customer Analytics Dashboard](https://github.com/user-attachments/assets/0b0dfde6-de92-43ac-9abd-30572eaf55e9)

> **Project note:** The repository contains original and cleaned CSV files and an Excel workbook. The dashboard preview and existing project notes support the qualitative takeaways below. Exact numeric findings have not been reproduced in this documentation because the large source files could not be independently inspected during this review. No figures have been invented.

## Project overview

| Area | Description |
|---|---|
| Business domain | Customer analytics |
| Tool | Microsoft Excel |
| Analysis focus | Customer growth, tenure, geography and company distribution |
| Techniques | Data cleaning, derived fields, PivotTables, slicers, conditional formatting and dashboard reporting |
| Main output | Interactive customer analytics dashboard |

## 1. The business problem

A business may know how many customers it has, but a headline count alone does not explain whether its customer base is growing, how long customers have stayed, or whether the base depends heavily on a small number of countries or companies.

I framed the business question as:

**How can customer data be organised into a simple, interactive view that helps decision-makers understand customer growth, tenure and concentration?**

The analysis is intended to support customer-base monitoring and further investigation. It does not establish why customers joined, why they stayed, or whether they are profitable; those questions would require additional data.

## 2. Business questions

- How many customers are represented in the dataset?
- How has the number of customers changed by subscription year?
- What does the customer-tenure distribution look like?
- Which countries account for the largest portions of the customer base?
- Which companies account for the largest portions of the customer base?
- Does the customer base appear geographically or organisationally concentrated?

## 3. Data and project files

| File | Purpose |
|---|---|
| [Customer Analytics original.csv](Customer%20Analytics%20original.csv) | Original dataset supplied with the project |
| [Customer Analytics Cleaned.csv](Customer%20Analytics%20Cleaned.csv) | Cleaned dataset used for analysis |
| [Customer Analytics.xlsx](Customer%20Analytics.xlsx) | Excel analysis and dashboard workbook |

The project notes describe customer attributes such as country, company, subscription year and tenure. Please refer to the workbook and CSV headers for the authoritative field names and definitions.

## 4. Analysis workflow

1. **Review the source data:** understand the available customer attributes and identify fields needed for the business questions.
2. **Prepare the data:** check duplicate and invalid records, standardise country and company labels, and review missing values.
3. **Create analysis fields:** derive subscription year and tenure groupings where the source fields allow them.
4. **Validate the cleaned data:** compare row counts and key totals before and after cleaning, and check that derived fields are sensible.
5. **Summarise the customer base:** use PivotTables to aggregate customers by year, country, company and tenure.
6. **Build the dashboard:** bring the key measures and breakdowns into one view, with slicers for interactive filtering.
7. **Interpret the results:** use the patterns to identify areas that may warrant deeper customer or market analysis.

More detail is available in [Methodology & Data Quality](docs/METHODOLOGY.md) and the [Project Report](docs/PROJECT_REPORT.md).

## 5. Dashboard and KPIs

The existing project describes the following dashboard elements:

- Total customer count
- New customers by year
- Average customer tenure
- Customer distribution by country
- Customer distribution by company
- Interactive filters for year, country and company

Definitions and interpretation notes are in [KPI Definitions](docs/KPI_DEFINITIONS.md).

## 6. Key takeaways recorded in the project

The existing analysis notes report three broad patterns:

- The customer base shows geographic and company-level concentration.
- A meaningful portion of customers falls into longer-tenure groups, suggesting a degree of customer-base stability.
- Customer acquisition patterns differ across subscription years.

These are qualitative takeaways from the original project description. Exact counts, percentages, top-ranked countries or companies, and year-by-year changes should be confirmed directly from the workbook before being used as quantified business claims. See [Key Findings & Interpretation](docs/KEY_FINDINGS.md).

## 7. What the findings could mean for a business

- **Concentration:** a business may want to understand its exposure to a limited set of countries or large customer organisations.
- **Tenure:** longer-tenure segments may be useful for retention analysis, but tenure alone does not prove satisfaction or loyalty.
- **Acquisition trends:** changes by subscription year can guide questions about marketing, sales activity or market expansion, but the reasons require additional evidence.

These are possible interpretations, not causal conclusions established by this dataset.

## 8. My role and skills demonstrated

I used Excel to prepare customer data, create analysis fields, summarise customer patterns and communicate the results through an interactive dashboard.

**Skills demonstrated:** Excel data cleaning, data validation, PivotTables, derived fields, customer segmentation, KPI definition, trend analysis, geographic and company-level analysis, dashboard design and business insight communication.

## 9. How to review the project

1. Start with the dashboard preview above.
2. Review the original and cleaned CSV files to understand the data preparation step.
3. Open the Excel workbook to inspect the analysis and dashboard.
4. Read the methodology and findings notes to understand the questions, calculations and interpretation.

## 10. Limitations and next steps

The analysis is descriptive. It does not include customer revenue, acquisition cost, churn events, customer satisfaction, contract value or transaction history. Therefore, it cannot establish customer lifetime value, profitability, churn rate or the causes of acquisition and retention patterns.

The next step is to validate the exact field definitions and all displayed numbers against the workbook, then extend the analysis with revenue and churn data if those sources become available.

---
*This project demonstrates how I turn customer data into structured reporting and business questions. The documented patterns should be treated as descriptive, not causal.*
