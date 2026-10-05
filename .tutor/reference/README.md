# AI Learning Vault Kit

A native-Linux/Obsidian adaptation of Amos Blomqvist's `learn` system, optimized for **deep understanding at high learning velocity**.

The core loop is:

**goal → diagnose → build dependency DAG → teach the highest-leverage next node → test generative understanding → repair or advance → persist → exit-evaluate → review**

The system is deliberately not optimized for either extreme:

- **shallow speed** — skimming many concepts while building brittle recognition;
- **depth theater** — spending twenty minutes unpacking details that do not materially improve the learner's mental model.

Instead it optimizes for **conceptual compression per unit time**: find the small set of generating ideas from which many details can be reconstructed, establish those ideas deeply, then move.

## What "deep" means here

For a primary target concept, the learner should be able to:

1. explain the mechanism in their own words;
2. reconstruct or derive the important result from prior knowledge;
3. say why the concept was needed in the first place;
4. identify assumptions, boundaries, and failure cases;
5. transfer it to a genuinely new case;
6. connect it to the surrounding conceptual graph.

Depth is therefore measured by what the learner can **generate**, not by how much text the tutor produced.

## Recommended vault layout

```text
AI-Learning-Vault/
├── 00 Home/
│   ├── Learning Dashboard.md
│   └── Learner Model.md
├── 01 Sessions/
├── 02 Concepts/
├── 03 Maps/
├── 04 Sources/
├── 05 Reviews/
├── 90 Templates/
├── viz/
└── .pi/
    ├── skills/
    ├── extensions/
    └── agents/
```

Run the agent from the vault root.

## Skills included

- `learning-orchestrator` — session state machine.
- `question-designer` — designs high-information diagnostic and mastery questions.
- `probe-learner` — locates the learner's prerequisite frontier.
- `plan-learning-dag` — constructs the minimal dependency graph.
- `depth-efficiency-controller` — keeps learning both extremely deep and time-efficient.
- `teach-node` — teaches one meaningful reasoning node at a time.
- `visualize-learning` — decides when/how to visualize.
- `obsidian-render` — writes clean Obsidian Markdown, MathJax and Mermaid.
- `verify-learning` — separates verified fact, derivation, intuition and uncertainty.
- `persist-learning` — stores evidence-backed learner state.
- `review-retrieval` — delayed retrieval and transfer testing.

See `LINUX_SETUP.md` and `BOOTSTRAP_AGENT_PROMPT.md`.
