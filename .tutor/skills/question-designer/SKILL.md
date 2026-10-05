---
name: question-designer
description: Design high-information questions that reveal what the learner actually understands before, during, and after learning. Use whenever evaluating knowledge, probing misconceptions, checking a teaching node, or running an exit/review assessment.
---

# Question Designer

A good question is an **instrument**. Its job is not to look difficult; its job is to distinguish between plausible internal models of the learner.

Never generate a generic quiz by sampling textbook questions.

## 1. Start with hypotheses about the learner

Before asking a question, identify the 2–5 most plausible states you are trying to distinguish.

Example for attention matrix shapes:

- H1 — knows matrix multiplication mechanically but not what rows mean;
- H2 — understands rows as token representations but not why `K^T` is needed;
- H3 — knows shape algebra but thinks transpose changes semantic content;
- H4 — understands both shape and pairwise-dot-product meaning.

Now design a question whose possible answers separate these hypotheses.

If you cannot state what different answers would tell you, the question is low-value.

## 2. Maximize information gain

Prefer questions with high discrimination:

- one answer reveals several dependencies at once;
- different mistakes point to different misconceptions;
- correct reasoning is difficult to fake by recognition;
- the question can be answered quickly.

Avoid ten nearly identical easy questions when one carefully chosen question can locate the frontier.

## 3. Use the right question archetype

### Prediction

Ask what should happen *before* showing the result.

Best for:
- causal/mechanistic understanding
- physical intuition
- algorithms
- mathematical transformations

### Reconstruction

Remove a key step and ask the learner to rebuild it.

Best for:
- derivations
- proofs
- architecture reasoning
- procedural knowledge

### Contrast

Present two nearly plausible alternatives and ask what property distinguishes them.

Best for:
- concepts commonly confused
- terminology with similar surface forms
- model/algorithm comparisons

### Error diagnosis

Give a plausible incorrect explanation and ask exactly where it breaks.

Best for:
- deep conceptual understanding
- known misconceptions
- post-learning verification

### Counterexample / boundary

Ask for a case where a claim stops applying.

Best for:
- assumptions
- theorem conditions
- overgeneralization

### Transfer

Change surface details while preserving deep structure.

Best for:
- detecting memorization
- post-session mastery
- abstraction

### Teach-back

Ask the learner to explain the idea to a technically competent person who knows the prerequisites but not this concept.

Best for:
- integration
- detecting hidden gaps in causal chains

### Compression

Ask: "What is the smallest set of ideas you would need to reconstruct the rest?"

Best for:
- identifying generating ideas
- end-of-session synthesis

## 4. Match the response format to the diagnostic goal

### Multiple choice

Use only when the options correspond to distinct misconceptions or models.

Construct distractors from real plausible errors. Never use filler distractors.

### Short free response

Default for explanations, predictions, and causal reasoning.

Keep the requested answer bounded: usually 1–5 sentences or a few equations.

### Worked problem

Use when execution matters.

Choose the smallest problem that still exposes the conceptual dependency.

### Diagram / annotation

Use when spatial, architectural, or graph structure is what matters.

## 5. Adaptive follow-up

Do not grade only right/wrong.

Classify the answer:

- **secure reasoning** — correct conclusion with a coherent causal/derivational path;
- **fragile reasoning** — correct answer but shallow, incomplete, lucky, or cue-dependent;
- **local gap** — mostly correct model with one missing edge;
- **systematic misconception** — internally coherent but wrong model;
- **unknown** — insufficient evidence.

Then ask the *minimum* follow-up that distinguishes remaining hypotheses.

Never ask another question merely because a fixed quiz count has not been reached.

## 6. Pre-learning diagnostic questions

The opening probe should answer:

- What prerequisites are secure?
- Where does each relevant strand break?
- Is the learner missing vocabulary, mechanism, formalism, or integration?
- What misconceptions are already active?
- How deep is the learner's target?

Start broad, then branch sharply.

A good opening question often spans several prerequisites at once. Based on the answer, drill only where uncertainty remains.

## 7. In-learning questions

After a teaching node, test the dependency edge just created.

Do **not** simply ask the learner to repeat the sentence you just said.

Prefer:
- prediction from the new idea;
- rebuild one missing step;
- distinguish the new concept from its nearest neighbor;
- apply it in a tiny new case.

## 8. Exit evaluation

The end-of-session assessment must use **novel prompts**, not recycled teaching examples.

For the primary target concept, sample across:

1. mechanism / meaning;
2. reconstruction or derivation;
3. boundary / assumption;
4. transfer;
5. integration with neighboring concepts;
6. misconception rejection.

Do not necessarily ask six separate questions. One well-designed problem may test several dimensions.

The learner should not pass merely by remembering the wording of the lesson.

## 9. Delayed review questions

Change both the wording and surface context.

Test whether the learner can regenerate the idea after context has decayed.

A delayed question should be harder to answer from episodic memory of the session and easier to answer from the actual conceptual model.

## 10. Question quality audit

Before asking, check:

- What latent distinction does this question measure?
- What would each likely wrong answer imply?
- Can the learner answer correctly by pattern matching?
- Is it harder than necessary to obtain the desired information?
- Does it test the concept or irrelevant arithmetic/wording?
- Is the answer unambiguous under the intended interpretation?

If the question fails this audit, redesign it.
