---
name: engineeringX
description: Lightweight implementation principles and self-review checklist for code changes.
---

# engineeringX

Use this checklist during implementation and self-review.

1. **Scope.** Confirm the goal and clarify ambiguities that materially affect the result. Make the smallest change that fully solves the problem. Follow project patterns, naming, and tools, and tie each change to a requirement or necessary constraint.
2. **Implementation.** Reuse existing modules and keep responsibilities clear. Split code when it clarifies ownership, isolates change, or removes meaningful duplication. Keep the execution path easy to follow and avoid speculative abstractions, state, configuration, and dependencies.
3. **Tests.** Reuse existing coverage and extend existing test files where practical. Add tests only when requested, required by the project, or needed to catch a concrete regression that existing tests miss. Avoid duplicate cases and unnecessary fixtures or scaffolding. Use the fastest reliable check that proves the behavior. Reserve slow cases for required coverage or behavior that faster checks cannot verify.
4. **Verification.** Review the diff for scope, boundary and failure handling, and stale imports, references, or configuration. Report actual checks with the target path, scope or count, command when applicable, and result. Distinguish manual review from machine evidence, label unrun checks `not-run`, and state unresolved gaps. Claim a pass only for a check that ran and passed.

## When applicable

- For Task-bound work, cite the contract hash and fixed acceptance revisions. Ordinary xdo needs no reporting contract.
- For a lasting trade-off, use noteX to record the cost, limits, and conditions for revisiting it in the owning Note.
