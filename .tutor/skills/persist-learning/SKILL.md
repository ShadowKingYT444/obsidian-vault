---
name: persist-learning
description: Persist evidence-backed learner state, including what was tested, how it was tested, misconceptions, and remaining uncertainty.
---

# Persist Learning

The vault is an inspectable learner model, not a transcript dump.

Persist **evidence**, not vibes.

## Update after meaningful checkpoints

Maintain:

1. active session note;
2. `00 Home/Learner Model.md`;
3. relevant `02 Concepts/` notes;
4. review metadata.

## Mastery states

Use:

- `unknown`
- `frontier`
- `fragile`
- `secure`

## Evidence dimensions

For important concepts, record evidence such as:

- meaning/mechanism;
- motivation;
- reconstruction/derivation;
- boundary awareness;
- transfer;
- integration;
- misconception rejection.

Do not require all dimensions for every prerequisite. The primary target should have broad evidence; enabling prerequisites need evidence proportional to their role.

## Evidence quality

Distinguish:

- `recognition`
- `recall`
- `reasoning`
- `reconstruction`
- `transfer`
- `error-diagnosis`

Later evidence types generally dominate earlier ones.

A correct recognition answer should not outweigh a failed transfer problem.

## Concept-note metadata

Example:

```yaml
status: fragile
last_tested: 2026-09-02
next_review: 2026-09-05
dependencies:
  - "[[Vector spaces]]"
supports:
  - "[[Linear maps]]"
evidence:
  - type: reconstruction
    result: pass
  - type: transfer
    result: partial
```

Do not pretend a numeric confidence score is calibrated unless the system actually calibrates it. Evidence tags are preferable to false precision.

## Misconceptions

Store the wrong generative rule.

Bad:
"Missed a transpose question."

Good:
"Treats transpose as modifying element values rather than exchanging axes, so predicts semantic transformation rather than index reorientation."

Record:
- evidence for the misconception;
- whether it was repaired;
- the question type that exposed it.

## Session end

Persist:

- target capability;
- generating ideas;
- strongest evidence of mastery;
- failed/fragile dimensions;
- active misconceptions;
- current frontier;
- deferred rabbit holes;
- next high-leverage node;
- suggested delayed-review targets.
