# Pattern — Physician Signoff Commit Boundary

## Risk condition

A system treats model output as equivalent to clinical authorization.

## Boundary question

Has an authorized clinical actor explicitly accepted the action?

## Outcome

- EXECUTE only after signoff
- REFUSE otherwise

## Proof surface

- commit boundary defined at signoff
- receipt binds decision
- replay confirms outcome

## Non-disclosure

No clinical decision logic is exposed.
