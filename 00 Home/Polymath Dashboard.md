---
type: dashboard
tags: [history, polymath]
---

# Polymath Dashboard

> The target is not to know many names. The target is to build models that transfer across war, politics, science, engineering, and business.

## Start here

- [[Greats Study Path]] — ordered curriculum across strategy, statecraft, science, computation, and industry
- [[History Atlas]] — chronological and thematic entry point
- [[People Atlas]] — biographies as decision case files
- [[Events Atlas]] — transformations, wars, crises, and institutional changes
- [[Strategy and Statecraft]] — power, organizations, logistics, information, legitimacy
- [[Science, Technology, and Industry]] — discovery, invention, scaling, and industrial systems
- [[Studying Greats Without Cargo Culting]] — the method
- [[Napoleon and Elon Musk - Mechanism Comparison]] — test the transcript's analogy instead of accepting it

## People to study next

```dataview
TABLE era, domains, importance, status
FROM "06 People"
WHERE type = "person"
SORT importance DESC, file.name ASC
LIMIT 20
```

## Events to study next

```dataview
TABLE start, end, themes, importance
FROM "07 Events"
WHERE type = "historical-event"
SORT importance DESC, start ASC
LIMIT 20
```

## Cross-case patterns

```dataview
TABLE domains, confidence
FROM "08 Patterns"
WHERE type = "historical-pattern"
SORT file.name ASC
```

## A high-value 30-minute block

1. Read one person note for 8 minutes.
2. Read one linked event for 8 minutes.
3. Read one linked pattern for 6 minutes.
4. Close the notes and reconstruct the causal chain from memory for 4 minutes.
5. Answer one transfer question in a different domain for 4 minutes.

## Standard of mastery

You do not know a case until you can explain what happened, why it happened, what could have changed it, which mechanism generalizes, and which details do not.
