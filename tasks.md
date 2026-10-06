# Tasks: DataPilot

## Phase 1: Foundation
- [ ] Create Snowflake trial account, warehouse, auto-suspend 60s
- [ ] Create schemas RAW, CURATED, ML and roles
- [ ] Load sample orders, accounts, contacts data

## Phase 2: Prep with CoCo
- [ ] Prompt CoCo for ingestion and dynamic table ORDERS_DT
- [ ] Review generated SQL and commit to repo
- [ ] Add data quality checks

## Phase 3: Govern
- [ ] Masking policy EMAIL_MASK on contacts
- [ ] Row access and role grants
- [ ] Verify audit log via ACCESS_HISTORY

## Phase 4: Serve
- [ ] Write semantic model for Cortex Analyst
- [ ] Train churn model with Snowflake ML and register it
- [ ] Write predictions to ML.OUT.AT_RISK

## Phase 5: Act
- [ ] Connect CoWork for tasks and approvals
- [ ] Wire the three demo actions

## Phase 6: Ship
- [ ] Polish index.html with live query results
- [ ] Record 2-minute demo
- [ ] Final README and submission check
