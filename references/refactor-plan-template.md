# Incremental Refactoring Plan

## Goal

Describe the architectural problem to solve and the behaviors that must remain unchanged.

## Invariants
- [ ] Public APIs/contracts remain compatible, or an explicit migration is defined
- [ ] Domain rules and validation semantics remain unchanged
- [ ] Persistent data/file formats remain readable
- [ ] State ownership and update ordering remain correct
- [ ] Critical user workflows remain usable
- [ ] Error handling and failure recovery remain acceptable

## Batches

### Batch 0 — Baseline and protection
- Scope:
- Existing behavior/tests to capture:
- Commands to run:
- Exit criteria:
- Rollback:

### Batch 1 — First low-risk change
- Scope:
- Files/modules:
- Expected boundary improvement:
- Required caller migrations:
- Tests/checks:
- Exit criteria:
- Rollback:

### Batch 2 — Consolidate or move one responsibility
- Scope:
- Files/modules:
- Expected boundary improvement:
- Required caller migrations:
- Tests/checks:
- Exit criteria:
- Rollback:

### Batch 3 — Larger structural changes
- Scope:
- Protected/high-risk areas:
- Required tests:
- Tests/checks:
- Exit criteria:
- Rollback:

## Architecture guardrails to add
- [ ] Forbidden dependency checks
- [ ] Circular dependency checks
- [ ] Canonical import/API checks
- [ ] Ownership or behavior invariants

## Completion report
- Changed/moved/deleted paths:
- Validation commands and outcomes:
- Unrun checks and reasons:
- Remaining risks:
- Follow-up candidates:
