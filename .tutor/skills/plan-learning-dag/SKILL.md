---
name: plan-learning-dag
description: Build the smallest dependency DAG that can take this learner from their current frontier to deep understanding of the target.
---

# Plan Learning DAG

A teaching route is a dependency graph, not a chapter outline.

The optimal graph is the **smallest graph that preserves the real reasoning required for deep mastery**.

Use `depth-efficiency-controller` while planning.

## Inputs

Use:

- target capability;
- diagnostic frontier;
- persistent learner model;
- verified domain knowledge;
- known misconceptions.

## Build the graph backward from the target

Ask:

1. What must the learner be able to generate to count as deeply understanding the target?
2. What immediate concepts make those capabilities possible?
3. Which of those are already secure?
4. Where are the shortest valid paths from secure roots to the target?

Only add nodes that carry explanatory weight.

## Classify nodes

Mark each node internally as:

- **Tier A: target generator**
- **Tier B: enabling prerequisite**
- **Tier C: peripheral/deferred**

Tier A nodes receive full depth treatment.
Tier B nodes receive enough depth to make the dependency reliable.
Tier C nodes stay out of the active route unless needed.

## Edge test

For every edge `A → B`, be able to complete:

"Without A, the learner could not derive/understand B because ____."

If that sentence is weak, the edge may be organizational rather than conceptual.

## Granularity test

Split a node if it contains multiple independent insights.

Merge nodes if they differ only by notation or bookkeeping.

## Root audit

A root must be both:

- actually available to this learner;
- strong enough to support what follows.

Do not start from a textbook's presumed prerequisite if the learner already knows something higher-level deeply.

## Optimize route length

Minimize:

- reteaching secure material;
- unnecessary historical order;
- duplicated examples;
- decorative detail;
- detours into adjacent topics.

Do **not** minimize the conceptual chain itself. Skipping an essential reasoning edge creates shallow learning.

## Present the plan

Write:

1. a short explanation of the route and why it is efficient for this learner;
2. a compact Mermaid dependency DAG;
3. the specific Tier A nodes that will receive deep mastery checks.

The DAG is editable during teaching. If evidence changes the inferred learner model, revise it.
