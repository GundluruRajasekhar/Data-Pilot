# Requirements: DataPilot on Snowflake CoCo

## Purpose
A governed, conversational data assistant that takes a business question from raw data to a trusted answer and a follow-up action, built with Snowflake CoCo (Cortex Code) and CoWork.

## Users
- Business analyst: asks questions in plain English.
- Data engineer: reviews CoCo-generated pipelines and SQL.
- Data steward: sets roles, masking policies and audits access.

## Functional requirements
1. FR1 Prep: CoCo generates ingestion and a dynamic table from RAW to CURATED.
2. FR2 Serve: natural-language questions answered via Cortex Analyst over a semantic model.
3. FR3 ML: CoCo builds and registers a Snowflake ML model (for example churn risk) and writes predictions to a governed table.
4. FR4 Govern: every answer shows role, masking and lineage checks.
5. FR5 Act: results trigger a CoWork task or approval request.
6. FR6 Transparency: generated SQL is always visible before and after execution.

## Non-functional requirements
- Security: role-based access, masking on PII, audit log of queries.
- Performance: answers within 10 seconds on sample data.
- Cost: warehouse auto-suspend at 60 seconds; resource monitor on.
- Explainability: each answer links to SQL and source tables.
- Portability: demo UI is a single static HTML file.

## Success criteria
- Three demo scenarios (analytics, ML, governance) run end to end.
- Zero PII shown to non-privileged roles.
- Prototype to production path documented in tasks.md.

## Out of scope
Real customer data, multi-cloud deployment, custom model training beyond Snowflake ML.
