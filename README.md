# Codebase Architecture Governance Skill

A reusable Agent Skill for understanding and improving module boundaries, dependency direction, state ownership, code duplication, unnecessary indirection, and safe refactoring plans.

## What it does

- Maps the current architecture before proposing changes.
- Helps decide when to keep, split, merge, move, migrate, or delete modules.
- Defines clear responsibilities and dependencies for frontend, backend, AI/workflow, and algorithm-heavy projects.
- Emphasizes evidence, behavior preservation, high-risk areas, and reversible batches.
- Produces a file/module audit and a practical validation plan.

## Install

Install the skill globally with [skills CLI](https://www.npmjs.com/package/skills):

```bash
npx skills add MercatorProj/codebase-architecture-governance@codebase-architecture-governance -g
```

For tooling that supports project-local skills, copy or install this folder into a path such as `.agents/skills/codebase-architecture-governance/`.

## Recommended first prompt

> Use the `codebase-architecture-governance` skill in assessment mode. Inspect this repository and produce a current-state module map, responsibility/ownership map, dependency rules, candidate file actions with evidence and risk, and a phased refactoring plan. Do not modify source files yet. Clearly separate confirmed facts from hypotheses and recommendations.

## Recommended implementation prompt

> Using the approved plan, implement only the first low-risk batch. Preserve existing behavior, keep the diff small, run the repository's relevant tests/checks, and report exact paths changed plus any unresolved risks.

## Design principles

The skill does not prescribe a fixed architecture or require fewer files at any cost. It prioritizes cohesive responsibilities, single ownership, explicit interfaces, correct dependency direction, and testable incremental changes.
