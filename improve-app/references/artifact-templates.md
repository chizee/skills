# Artifact Templates — improve-app

Skeletons this metaskill creates in the user's `docs/` folder. Extend-only artifacts are governed by the section headings named in each phase — add or update your own sections, preserve everyone else's. The four skeletons below (TECH-DEBT, TESTING, RELIABILITY, DESIGN) are the ones improve-app most often creates from scratch when no prior journey has touched them; the other artifacts it extends (ARCHITECTURE.md, PRODUCT.md, METRICS.md) already exist by the time this journey reaches them; extend them under the exact section headings named in each phase's Artifact field.

## Tracker: docs/IMPROVE-APP-PLAN.md

```markdown
# Improve an App Plan

## Context
Intake answers, date started, project specifics.

## Phase Status
| Phase | Skill | Status | Artifact | Date |
|---|---|---|---|---|
| 1 Quality baseline | clean-code | pending | TECH-DEBT.md | |
| 2 Refactor safely | refactoring-patterns | pending | TECH-DEBT.md | |
| 3 Safety net (GATE) | working-with-legacy-code | pending | TESTING.md, TECH-DEBT.md | |
| 4 Deepen the design | software-design-philosophy | pending | ARCHITECTURE.md | |
| 5 Survive production | release-it | pending | RELIABILITY.md | |
| 6 Fix the data layer | ddia-systems | pending | ARCHITECTURE.md, RELIABILITY.md | |
| 7 Polish microinteractions | microinteractions | pending | DESIGN.md | |
| 8 Remove friction | ux-heuristics | pending | DESIGN.md | |
| 9 Make it fast | high-perf-browser | pending | METRICS.md | |
| 10 Lock in habits | pragmatic-programmer | pending | TECH-DEBT.md, ARCHITECTURE.md | |
| 11 Brutal review | steve-jobs-design-review | pending | PRODUCT.md, DESIGN.md | |
Statuses: pending · in-progress · awaiting-evidence · done · deferred: <reason> · skipped: <reason>

## Key Decisions
| Date | Phase | Decision | Rationale |
|---|---|---|---|

## Next Actions
- [ ] action (owner, due)
```

## docs/TECH-DEBT.md

```markdown
# Technical Debt

## Debt Ledger
| Item | Location | Type | Risk | Effort | Priority | Status |
|---|---|---|---|---|---|---|

## Smell Inventory
| Smell | Location | Refactoring | Status |
|---|---|---|---|

## Sprout / Wrap Register
Code added beside legacy (to fold back in later).

## Debt Budget & Broken-Windows Policy
Time per iteration; what gets fixed now vs boarded up with a ticket.

## Adopted Conventions
```

## docs/TESTING.md

```markdown
# Testing

## Test Strategy
Pyramid, tooling, what "green" gates.

## Safety Net Map
| Module | Pinned behaviors | Test files | Gaps |
|---|---|---|---|

## Characterization Backlog
- [ ] module (risk, priority)

## CI Gates
```

## docs/RELIABILITY.md

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

## docs/DESIGN.md

```markdown
# Design System

## Design Direction
Signature moment, personality, references.

## Typography
Typefaces, scale, measure, line height, loading strategy.

## Tokens
Spacing scale · color palette (shades, tinted grays) · shadows.

## Components
| Component | Decision | Status |
|---|---|---|

## UX Audit Findings
| Issue | Heuristic | Severity (0-4) | Fix | Status |
|---|---|---|---|---|

## Microinteraction Inventory
| Interaction | Trigger/Rules/Feedback/Loops | Fix | Status |
|---|---|---|---|
```
