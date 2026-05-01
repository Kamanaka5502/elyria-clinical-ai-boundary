# Pattern — Clinical Replay Receipt

## Risk condition

A clinical decision cannot be reproduced under identical conditions.

## Boundary question

Does the same state and governing conditions produce the same outcome?

## Outcome

- EXECUTE if replay matches
- REFUSE or HALT if mismatch

## Proof surface

- receipt contains state signature and outcome
- replay confirms determinism

## Non-disclosure

No patient data or implementation details are exposed.
