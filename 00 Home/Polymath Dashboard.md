---
type: dashboard
tags: [history, polymath]
---

# Polymath Dashboard

> The target is not to know many names. The target is to build models that transfer across war, politics, science, engineering, and business.

## Do this today

- [[Today - Polymath]] — automatically shows the dated assignment for today
- [[12 Week Polymath Curriculum]] — full October 4 to December 27 sequence
- [[Napoleon and Musk - Operating System to Copy]] — the execution system to apply while studying

## Reference maps

- [[Greats Study Path]] — concept-oriented route across strategy, statecraft, science, computation, and industry
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

## Standard of mastery

You do not know a case until you can explain what happened, why it happened, what could have changed it, which mechanism generalizes, and which details do not.
