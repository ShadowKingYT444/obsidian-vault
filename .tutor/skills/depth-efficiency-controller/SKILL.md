---
name: depth-efficiency-controller
description: Control conceptual granularity and pacing so learning is maximally deep without wasting time. Use during planning, teaching, repair, and exit evaluation.
---

# Depth–Efficiency Controller

Optimize for **deep generative understanding per unit time**.

The two common failure modes are:

1. **shallow velocity** — many topics touched, few actually understood;
2. **depth theater** — excessive detail, side quests, repeated examples, and micro-questions that no longer improve the learner's model.

Avoid both.

## Depth is generative, not verbose

A concept is deep when the learner can regenerate important consequences from a compact mental model.

More explanation is not automatically more depth.

Prefer:
- a small number of powerful generating ideas;
- explicit dependency edges;
- mechanisms over labels;
- derivations over arbitrary rules;
- transfer over repeated rehearsal.

## Classify nodes by importance

### Tier A — target generators

Ideas central to the user's goal and from which many later facts follow.

Teach these extremely deeply.

### Tier B — enabling prerequisites

Needed to understand a Tier A node but not themselves the target.

Teach only to the depth necessary to make the dependency reliable, unless they turn out to be a misconception bottleneck.

### Tier C — peripheral detail

Historical notes, edge-case implementation trivia, alternative notation, exhaustive taxonomy.

Defer unless:
- the user asks;
- it changes the core model;
- it is required for transfer;
- it prevents a likely misconception.

This classification is one of the main time-saving mechanisms.

## Choose the correct node size

A node is too large when:
- the learner can understand the first half but not the second;
- the explanation contains multiple independent "why" jumps;
- failure cannot be localized.

A node is too small when:
- it creates bookkeeping without a new idea;
- the check question is trivial;
- several adjacent nodes always rise and fall together.

Continuously merge/split nodes to keep each node at one meaningful reasoning step.

## The depth gate

For a Tier A concept, do not call it deeply learned until there is evidence that the learner can:

- **MEANING** — explain what the object/process means;
- **MOTIVATION** — explain why it is needed;
- **MECHANISM** — trace how it works;
- **RECONSTRUCTION** — derive/rebuild the crucial relationship from secure prerequisites;
- **BOUNDARY** — identify assumptions or where the model stops applying;
- **TRANSFER** — use it in a novel case;
- **INTEGRATION** — connect it to surrounding concepts.

Do not mechanically ask seven questions. Use a small number of high-information questions that jointly cover these dimensions.

For Tier B nodes, require enough evidence that they can safely support the next Tier A inference. Do not force full Tier A treatment.

## Fast-path rule

If the learner demonstrates deep knowledge immediately, compress or skip the node.

Do not reteach because the syllabus says it comes first.

## Slow-path rule

If a dependency is genuinely broken, slow down exactly there.

Do not preserve nominal pace by building on a shaky prerequisite.

## Stop rule for a node

Advance when:

1. the learner can reconstruct the essential idea;
2. the active misconception hypotheses are ruled out;
3. at least one non-identical application succeeds;
4. more examples would mostly repeat the same evidence.

This is the point of diminishing returns.

## Rabbit-hole detector

Pause or defer a branch when:

- it does not change the target concept's mechanism;
- it is not required by the current DAG;
- it is a rare edge case;
- it introduces more prerequisites than explanatory value;
- the learner is asking out of curiosity but the branch would derail the current goal.

Record it under "parking lot / later" and continue. Curiosity is preserved without destroying session throughput.

## Compression checkpoints

Periodically ask:

- "What single idea explains the last several details?"
- "Which facts here are generators and which are consequences?"
- "Can we delete any memorized rule because it is now derivable?"

The lesson should become *simpler* in the learner's head as depth increases.

## Time is evidence-driven, not uniform

Spend time in proportion to:

**importance × uncertainty × misconception risk**

not in proportion to textbook chapter length.

A central concept with a wrong mental model deserves substantial repair.
A peripheral fact that is already secure deserves seconds.
