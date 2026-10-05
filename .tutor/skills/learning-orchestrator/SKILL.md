---
name: learning-orchestrator
description: Orchestrate adaptive learning for extremely deep understanding at high learning velocity. Use whenever the user asks to learn, understand, review, or be taught a topic.
---

# Learning Orchestrator

Treat learning as a stateful inference-and-control loop.

The objective is:

**maximize durable generative understanding per unit time**

not "cover material quickly" and not "spend a long time being thorough."

## State machine

1. **Specify target**
2. **Read existing learner state**
3. **Probe**
4. **Build minimal dependency DAG**
5. **Classify node importance**
6. **Teach the highest-leverage unresolved node**
7. **Check with high-information questions**
8. If weak: diagnose and repair the exact broken edge.
9. If secure enough for its role: advance.
10. **Exit-evaluate the target with novel questions**
11. **Persist evidence**
12. **Schedule/recommend retrieval**

## Session start

Create or choose a note in `01 Sessions/`.

Read:

- `00 Home/Learner Model.md`
- relevant `02 Concepts/` notes
- recent sessions touching the same prerequisites

Stored mastery is evidence, not truth. Re-check anything stale or important.

Translate the learner's request into an observable target:

- derive X;
- explain X from first principles;
- solve class Y;
- implement X and explain why it works;
- compare X and Y mechanistically;
- critique an argument;
- reconstruct a system from its constraints.

## Skills

Use:

- `question-designer`
- `probe-learner`
- `plan-learning-dag`
- `depth-efficiency-controller`
- `teach-node`
- `visualize-learning`
- `obsidian-render`
- `verify-learning`
- `persist-learning`
- `review-retrieval`

## Allocation of cognitive work

The system handles:

- sequencing;
- source triage;
- verification;
- notation consistency;
- note maintenance;
- progress inference;
- deciding what to test next.

The learner handles the cognition that actually produces learning:

- prediction;
- explanation;
- derivation;
- reconstruction;
- comparison;
- counterexample generation;
- transfer;
- critique.

Do not waste the learner's effort on logistics. Do not remove the productive struggle inside the subject.

## Pacing

Teach **one meaningful reasoning step at a time**, not one sentence at a time.

Use `depth-efficiency-controller` to continuously adjust node granularity.

If the learner already has a node deeply, skip it.
If one dependency is broken, slow down exactly there.
If a tangent is not structurally necessary, park it.

## Assessment discipline

Use `question-designer` for every meaningful assessment.

Questions should be chosen for information gain, not generated from a generic quiz template.

Before learning, questions infer the frontier.
During learning, they test the newest dependency edge.
After learning, they test novel transfer and reconstruction without reusing the lesson's wording.

## Mastery states

Use:

- `unknown`
- `frontier`
- `fragile`
- `secure`

For the primary session target, "secure" means there is evidence of generative understanding across multiple dimensions, especially reconstruction and transfer.

Never infer secure understanding from:
- fluent conversation;
- one correct multiple-choice response;
- immediate repetition of the tutor's wording;
- the learner saying "yeah that makes sense."

## Session completion

Do not end merely because the explanation is finished.

Run an **exit evaluation** that tries to falsify the belief that the target was learned.

If the learner passes, persist the strongest evidence and remaining boundaries.
If the learner fails, repair only the failed dimensions, then retest with a new prompt.
