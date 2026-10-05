# Native Linux setup

Run both Obsidian and the tutor harness natively on Linux.

Recommended structure:

```text
~/Documents/AI-Learning-Vault/
├── 00 Home/
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

Run `pi` from the vault root.

## Subagents

Because Linux + tmux are available, the full subagent architecture can be used when useful:

- researcher — external verification / source mapping
- mermaid-maker — structural diagrams
- svg-maker — geometric/spatial diagrams

Subagents are useful for context isolation and verification, but they are not the pedagogy. The main learning loop must still work if a subagent fails.

## Rendering

Prefer the simplest representation that carries the concept:

1. Obsidian-native MathJax for mathematics.
2. Obsidian-native Mermaid for dependency/flow diagrams.
3. Render-and-inspect Mermaid/SVG subagents when visual correctness or layout matters.

Do not turn every idea into a PNG merely because the machinery exists.

## Model allocation

Use the strongest available model for:

- frontier diagnosis
- dependency planning
- core explanations
- misconception analysis
- high-value assessment questions

Cheaper models may handle:

- metadata normalization
- note cleanup
- simple retrieval scheduling
- non-critical formatting

Do not save model cost by weakening the part that determines what the learner actually understands.
