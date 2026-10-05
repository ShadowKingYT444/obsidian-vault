---
name: visualize-learning
description: Create minimal learning visuals when relationships, geometry, state, or dependency are easier to understand visually.
---

# Visualize Learning

A visual must reduce reasoning load by exposing structure. Do not visualize merely to make the note look richer.

## Choose the representation

### Mermaid in Markdown — default

Use for:
- dependency DAGs
- flows
- pipelines
- state machines
- hierarchies
- sequences
- comparisons with clear relations

Prefer native Mermaid because it is editable, lightweight, and rendered directly by Obsidian.

### SVG / Excalidraw — optional

Use when exact spatial placement matters:

- geometry
- vectors
- coordinate systems
- physical layouts
- custom plots

### Equation / aligned derivation

Use MathJax instead of a diagram when the structure is fundamentally algebraic.

## Minimality rule

One picture = one idea.

Delete any label or node that does not materially help the learner infer the intended relation.

## Correctness rule

Check:
- arrow direction
- dependencies
- labels
- variable names
- dimensions/units
- visual implication

If rendering/vision tools are available, render and inspect. If not, prefer conservative Mermaid syntax and avoid claiming pixel-level verification.

## Embed

For Mermaid, place the code block directly in the session or concept note.

For an image saved under `viz/`:

```md
![[my-diagram.png|600]]
```
