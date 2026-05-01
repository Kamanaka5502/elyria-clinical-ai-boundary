# Clinical Boundary Model

This repository defines a public-safe boundary model for clinical AI consequence control.

It does not provide medical advice, diagnosis, triage, prescribing logic, or treatment recommendation logic.

## Boundary principle

A clinical AI output is not clinical authorization.

A recommendation may only move toward consequence after the boundary confirms that the required evidence, authority, role, policy, and replay conditions hold.

## Boundary stack

1. Input formation
2. Evidence freshness check
3. Role and authority check
4. Clinical context qualification
5. Physician signoff boundary
6. Receipt emission
7. Replay verification
8. Persistence validation

## Core distinction

Most clinical AI systems focus on output quality.

Elyria Systems focuses on whether an output is admissible to move toward consequence.

## Public outcomes

- EXECUTE — boundary conditions hold and the action may continue toward authorized clinical path
- REFUSE — required conditions fail
- ESCALATE — human review is required before continuation
- REDIRECT — missing or stale evidence must be repaired before review
- HALT — continuation is unsafe or structurally unsupported

## Commit boundary

The clinical commit boundary is not model generation.

For this public surface, the commit boundary is physician signoff or equivalent authorized clinical acceptance.

## Private layer not exposed

This document does not expose implementation, scoring, thresholds, patient data, PHI, clinical models, production adapters, or decision-support logic.
