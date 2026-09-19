# Data Quality Notes

## Core Principles

The raw layer was preserved. Cleaning decisions were made only when supported by evidence.

## Main Issues

- 97 exact duplicate ticket rows
- 91 defensible missing-client imputations
- 30 ambiguous missing-client records retained as NULL
- 97 orphan agent IDs
- 146 agent/team mismatch records involving 85 agents
- 170 missing category IDs recovered through exact label mapping
- 243 missing first-response timestamps retained as NULL
- 1,052 records with missing resolution values retained where status made the values not applicable
- 557 materially inconsistent stored resolution durations
- 22 invalid CSAT scores
- 45 duplicate feedback rows
- 30 orphan feedback records
- 292 nonstandard status values normalized
- Multiple priority variants normalized
- SLA policy gaps retained as unevaluable instead of force-matched

## Validation Rule

A record was not changed merely because it looked unusual. The available evidence was reviewed first, and ambiguous cases were retained or flagged.
