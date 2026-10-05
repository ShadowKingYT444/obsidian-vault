# Portable tutoring contract

This contract is independent of model, provider, CLI, and agent harness.

## Start with minimal context

For a tutoring request, read in this order:

1. `.tutor/skills/learning-orchestrator/SKILL.md`
2. `00 Home/Learner Model.md`
3. only the concept, person, event, pattern, and recent session notes relevant to the requested topic
4. only the additional skills named by the orchestrator for the current stage

For history, biography, statecraft, science history, and industrial history, also read `.tutor/HISTORY_GUIDE.md`.

## Core loop

`goal -> diagnostic probe -> minimal dependency DAG -> Tier A/B classification -> teach one high-leverage node -> discriminative check -> repair or advance -> novel exit assessment -> persist evidence`

Keep the learner doing prediction, reconstruction, explanation, transfer, and critique.

## Storage

- Sessions: `01 Sessions/`
- Durable concepts: `02 Concepts/`
- Concept maps: `03 Maps/`
- Sources and verification: `04 Sources/`
- Reviews: `05 Reviews/`
- People / biographies: `06 People/`
- Historical events and transformations: `07 Events/`
- Cross-case mechanisms and patterns: `08 Patterns/`
- Templates: `90 Templates/`
- Learner state: `00 Home/Learner Model.md`
- Main dashboard: `00 Home/Learning Dashboard.md`
- Polymath dashboard: `00 Home/Polymath Dashboard.md`

Never dump a raw chat transcript into the vault. Persist only evidence, useful derivations, misconceptions, open edges, and next steps.
