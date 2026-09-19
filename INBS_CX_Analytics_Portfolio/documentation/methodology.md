# Methodology

## Workflow

1. Preserve raw CSV data.
2. Load raw data into PostgreSQL.
3. Profile row counts, nulls, duplicates, and distinct values.
4. Investigate data-quality issues.
5. Create clean-layer transformations.
6. Match tickets to time-effective SLA policies.
7. Create analytical fields and DAX measures.
8. Build a one-page Power BI dashboard.
9. Interpret findings with business context and analytical limitations.

## Data-Layer Design

- `raw`: source data preserved as received
- `clean`: deduplication, normalization, and defensible corrections
- `analytics`: analytical fields, SLA matching, and BI-ready structures

## Analytical Principles

- Do not overwrite raw data.
- Do not guess ambiguous mappings.
- Do not treat all NULLs as errors.
- Do not classify unevaluable records as failures.
- Preserve original fields when creating derived analytical fields.
- Distinguish association from causation.
- Use the business question to determine the appropriate visual.
