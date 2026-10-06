# DataPilot: governed data conversations on Snowflake

Built for the Build with Snowflake CoCo challenge.

## What it does
Ask a business question. CoCo (Cortex Code) writes the pipeline and SQL, governance checks run, Cortex Analyst serves the answer, and CoWork turns it into an action. Less glue code, more shipping.

## The flow
1. Prep: raw tables become a curated dynamic table.
2. Govern: roles, masking policies and lineage are checked on every query.
3. Serve: answer plus visible SQL, then a CoWork task.

## Demo scenarios
- Revenue drop analysis (analytics)
- Churn-risk model (ML)
- Masked customer emails (governance)

## Run it
Open `index.html` in any browser. It uses sample data and needs no setup.

## Snowflake setup (production path)
1. Create RAW, CURATED, ML schemas and roles ANALYST, ENGINEER, STEWARD.
2. Use CoCo to generate ingestion and dynamic tables.
3. Add a semantic model for Cortex Analyst.
4. Apply masking policies on PII columns.
5. Train and register the model with Snowflake ML.
6. Connect CoWork for tasks and approvals.

## Files
index.html, requirements.md, readme.md, tasks.md

## Notes
Demo figures are illustrative. Check current Snowflake docs for which capabilities are GA or preview in your account.
