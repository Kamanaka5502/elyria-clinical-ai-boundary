# Elyria Systems — Clinical AI Boundary

Public clinical AI boundary proof surface for recommendation admissibility, physician signoff, stale evidence refusal, receipt binding, and replayable clinical governance.

This repository is not a medical AI tool.

It does not diagnose, treat, prescribe, triage, or recommend care.

It defines a public-safe boundary model for deciding whether a clinical AI output may proceed toward human clinical review, authorization, or consequence.

## Core claim

A model recommendation is not clinical authorization.

A clinical consequence may bind only after the required boundary conditions hold:

- evidence is current enough for the intended use
- authority is valid
- clinical role is explicit
- physician signoff boundary is respected
- refusal occurs when admissibility fails
- receipt binds the decision surface
- replay can reproduce the boundary result

## Public proof surfaces

- CLINICAL_BOUNDARY_MODEL.md
- PATTERN_STALE_CLINICAL_EVIDENCE.md
- PATTERN_PHYSICIAN_SIGNOFF_COMMIT.md
- PATTERN_RECOMMENDATION_NOT_AUTHORIZATION.md
- PATTERN_CLINICAL_REPLAY_RECEIPT.md
- ONE_CLINICAL_PROOF.md
- NON_IMPLEMENTATION_NOTICE.md
- LICENSE
- NOTICE
- clinical_boundary_register.json

## Public-safety boundary

This repository does not contain:

- patient data
- PHI
- diagnosis logic
- treatment recommendation logic
- medical scoring models
- clinical decision support implementation
- production integration code
- private evaluator algorithms

## Foundation lineage

Elyria Systems is the visible product surface.

VA / Veritas Aegis remains the foundation and enforcement lineage beneath the product surface.