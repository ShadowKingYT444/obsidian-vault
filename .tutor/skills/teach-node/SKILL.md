---
name: teach-node
description: Teach one meaningful dependency node deeply and efficiently using motivation, reconstruction, connection, and discriminative testing.
---

# Teach One Node

The unit of teaching is one **meaningful reasoning step**.

Use `depth-efficiency-controller` to determine how much depth this node deserves and `question-designer` to test it.

## 1. State the local problem

Before introducing the new object/rule, make the limitation of the current model visible.

The learner should know:

- what we are trying to accomplish;
- why existing tools are insufficient;
- what property a solution would need.

This creates the motivation edge.

## 2. Let the learner predict when productive

If the next move is plausibly discoverable from secure prerequisites, ask a short prediction/reconstruction question.

Do not turn every sentence into Socratic interrogation.

Socratic interaction is useful only when the learner has enough structure to reason forward.

## 3. Establish the generating idea

Give the smallest idea that explains the largest number of consequences.

Separate clearly:

- intuitive model;
- formal statement;
- assumptions/domain;
- notation.

Avoid dumping every consequence immediately.

## 4. Reconstruct, do not decree

For important relationships, make the path derivable:

- What constraint are we satisfying?
- What candidate operation/object would satisfy it?
- Why this one?
- What would break if we chose differently?

The learner should feel that the result is *forced or motivated*, not arbitrary.

## 5. Connect to the graph

Explicitly state:

- which prior node supports this;
- what new capability this node unlocks;
- which later target node it will support.

This turns a fact into a dependency edge.

## 6. Add one high-value example

Choose an example that exposes the mechanism.

Do not give five routine examples when the first already establishes the pattern.

If a second example is needed, change the structure enough to test generalization.

## 7. Visualize only structural content

Use `visualize-learning` when geometry, dependency, flow, state, or architecture carries explanatory information.

Do not add diagrams as decoration.

## 8. Check generative understanding

Do not ask:
"What is X?" immediately after defining X, unless recall itself is the uncertain dimension.

Use a high-information question such as:

- predict a consequence;
- rebuild a missing derivation step;
- explain why a tempting alternative fails;
- transfer the idea to a changed case;
- identify a boundary.

## 9. Diagnose failure at the edge

If the learner misses:

1. infer the broken dependency;
2. ask one discriminative follow-up if needed;
3. repair only that edge;
4. retest with a new surface form.

Do not restart the whole explanation.

## 10. Advance at diminishing returns

For Tier A nodes, advance when the learner demonstrates:
- mechanism;
- reconstruction;
- at least one novel transfer;
- no active core misconception;
- enough boundary awareness to avoid obvious overgeneralization.

For Tier B nodes, advance as soon as the prerequisite is reliable enough to support the next inference.

Depth must be concentrated where it creates reusable explanatory power.
