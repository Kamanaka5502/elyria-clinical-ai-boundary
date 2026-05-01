# Clinical 15D Boundary Model

This repository uses a public-safe 15D clinical boundary frame.

It is not a medical model. It does not diagnose, prescribe, triage, or recommend care.

The 15D frame exists to show that clinical AI consequence cannot be evaluated as a flat approval workflow. A recommendation may move toward clinical consequence only when every required dimension remains admissible at the boundary.

## Public 15D dimensions

1. Patient-state freshness
2. Evidence recency
3. Clinical context fit
4. Authority and role validity
5. Physician signoff boundary
6. Policy and institutional constraint
7. Consent and permitted-use scope
8. Risk burden
9. Capacity to support consequence
10. Traceability of source evidence
11. Receipt continuity
12. Replay determinism
13. Refusal conditions
14. Escalation conditions
15. Post-decision persistence validity

## Boundary equation

Clinical consequence may bind only when the public-safe boundary relation holds:

A(x) >= 0
Phi(x) >= 0
U(x) = 1
R(x) = valid

Where:

- A(x) represents admissibility
- Phi(x) represents remaining capacity after burden
- U(x) represents authority validity
- R(x) represents replayable receipt continuity

## Consequence rule

A recommendation is not authorization.

A generated clinical output becomes consequence-relevant only after boundary admission. If any required dimension fails, the lawful outcome is REFUSE, ESCALATE, REDIRECT, or HALT.

## Market distinction

Most clinical AI systems optimize for outputs.

This surface governs whether an output is admissible to move toward consequence.

That is the difference between model performance and clinical boundary control.

## Private layer not exposed

This public model does not expose:

- medical logic
- patient data
- PHI
- diagnostic scoring
- treatment recommendation logic
- production evaluator internals
- thresholds
- runtime implementation
