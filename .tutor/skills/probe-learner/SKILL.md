---
name: probe-learner
description: Diagnose the learner's prerequisite frontier with a small number of highly discriminative questions before teaching.
---

# Probe Learner

The probe is model identification.

Infer the learner's current conceptual graph well enough to place the lesson exactly at the frontier, while spending as few questions as necessary.

Use `question-designer` to construct the questions.

## 1. Sketch the prerequisite graph

Before asking anything, identify the smallest set of prerequisite strands required by the target.

For each strand, consider possible failure types:

- vocabulary only;
- missing intuition;
- missing mechanism;
- missing formalism;
- inability to connect formalism to meaning;
- misconception;
- knowledge is present but not retrievable;
- local knowledge with no transfer.

## 2. Ask broad, high-information questions first

Prefer a question that simultaneously exposes several dependencies.

Example pattern:

"Here is a concrete situation. Predict what happens, and explain the mechanism."

A good response may prove several prerequisites at once.
A bad response tells you which branch to probe next.

Do not begin with a checklist of twenty atomized questions.

## 3. Binary-search uncertainty

For every relevant strand, locate a floor and a ceiling.

- Strong answer → jump substantially harder or more abstract.
- Weak answer → move down one dependency.
- Correct but unexplained → test reconstruction or transfer.
- Confident wrong answer → identify the exact misconception.
- "I don't know" → treat as useful evidence, not failure.

Stop probing a strand once the teaching-relevant frontier is located.

## 4. Distinguish types of knowing

Do not collapse all knowledge into right/wrong.

Ask enough to distinguish:

- recognizes terminology;
- can state a definition;
- understands mechanism;
- can derive/reconstruct;
- can transfer;
- has integrated the idea with neighboring concepts.

The lesson should begin at the first missing level that matters for the target.

## 5. Misconception mapping

When an answer is wrong, ask:

"What internal rule would make this answer seem reasonable?"

Then test that candidate rule with one discriminative follow-up.

Persist the misconception if it is systematic.

## 6. Efficiency rule

Every extra probe question must reduce uncertainty that would change the lesson plan.

If the answer to a question would not affect what you teach or how you teach it, do not ask it.

## Output

Write a compact diagnostic state:

### Secure foundations
What can safely be built on.

### Frontier
The exact next missing conceptual edges.

### Misconceptions
Wrong models with evidence.

### Uncertainty
What was not worth probing yet.

### Recommended starting node
The highest-leverage point at the learner's frontier.
