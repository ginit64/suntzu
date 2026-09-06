---
name: suntzu
description: >
  KISS-first software engineering for implementation, bug fixes, refactoring,
  code review, and software design. Use when changing code or evaluating whether
  abstractions, dependencies, layers, configuration, shared state, or other
  complexity are necessary. Prefer the simplest correct solution to the present
  requirement.
---

# SUNTZU

Win by making the problem smaller before making the solution larger.

## Doctrine

- **Survey the terrain.** Understand the affected code, execution path, constraints, invariants, and failure modes well enough to make the change correctly.
- **Use what already works.** Prefer existing code, language and platform features, stdlib, and proven dependencies when they reduce total complexity. Do not force reuse that creates worse coupling.
- **Narrow the problem.** Solve the present requirement, not imagined future ones. Remove accidental and speculative scope, avoid hypothetical scale, and generalize only when evidence requires it. Do not reduce explicit requirements.
- **Take the simplest correct path.** Prefer explicit, local, readable, reversible changes with the fewest necessary concepts and states. Simplicity is not minimum LOC.
- **Zero unjustified coupling.** Avoid layers, shared state, configuration, dependencies, and abstractions unless they remove more complexity than they add. Prefer small duplication to coupling unrelated concepts.
- **Uphold invariants and verify.** Do not simplify away correctness, security, data integrity, explicit requirements, required compatibility, failure handling, or operational needs. Use the cheapest meaningful verification proportional to the risk of the change.

When choices are otherwise equal, prefer:

`existing over new · concrete over generic · local over global · boring over clever · reversible over irreversible`

Before adding machinery, ask:

**Why are we fighting this battle at all?**
