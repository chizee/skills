# architecture-optimization artifact templates

Skeletons this metaskill creates in the user's docs/ folder. Extend-only artifacts (TESTING.md, ARCHITECTURE.md, TECH-DEBT.md) are governed by the section headings named in each phase — read the file before writing, add or update your sections, and preserve everyone else's. The skeletons below are the files this journey most often creates from scratch; copy them verbatim only when the file is missing.

## Tracker: docs/ARCHITECTURE-OPTIMIZATION-PLAN.md

Created on the first run (Intake). Never shared with another journey.

```markdown
# Architecture Optimization Plan

## Context
Intake answers, date started, hot paths in scope, tool of record for measurements.

## Phase Status
| Phase | Skill | Status | Artifact | Date |
|---|---|---|---|---|
| 1 | working-with-legacy-code | pending | TESTING.md, PERFORMANCE.md | |
| 2 | clean-architecture | pending | ARCHITECTURE.md | |
| 3 | software-design-philosophy | pending | TECH-DEBT.md | |
| 4 | refactoring-patterns | pending | TECH-DEBT.md | |
| 5 | system-design | pending | PERFORMANCE.md, ARCHITECTURE.md | |
| 6 | ddia-systems | pending | ARCHITECTURE.md, PERFORMANCE.md | |
| 7 | release-it | pending | RELIABILITY.md | |
| 8 | pragmatic-programmer | pending | PERFORMANCE.md, TECH-DEBT.md, TESTING.md | |
Statuses: pending · in-progress · awaiting-evidence · done · deferred: <reason> · skipped: <reason>

## Key Decisions
| Date | Phase | Decision | Rationale |
|---|---|---|---|

## Next Actions
- [ ] action (owner, due)
```

## docs/PERFORMANCE.md

Measured performance state — baselines, budgets, findings, and the before/after ledger. Creates: architecture-optimization.

```markdown
# Performance

## Baselines & Budgets
| Metric (p50/p95, throughput, cost) | Baseline (date) | Budget | Gate |
|---|---|---|---|

## Load Reality
Measured QPS average/peak, data volumes, growth rate.

## Profile Findings
| Hotspot | Evidence (profiler/APM) | Suspected cause | Fix | Status |
|---|---|---|---|---|

## Optimization Ledger
| Change | Before | After | Verdict (keep/revert) | Date |
|---|---|---|---|---|
```

## docs/RELIABILITY.md

Production hardening status — created here only when no prior journey has (otherwise extend).

```markdown
# Reliability

## Integration-Point Audit
| Dependency | Timeout | Circuit breaker | Bulkhead | Retry policy | Status |
|---|---|---|---|---|---|

## Query & Resource Findings
Unbounded result sets, missing LIMITs/pagination, blocked threads.

## Health Checks & Metrics
Deep health checks · RED metrics · symptom-based alerts.

## Deploy vs Release
Feature flags, expand-contract migrations, rollback plan.
```
