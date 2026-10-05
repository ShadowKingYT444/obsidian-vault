---
type: review-dashboard
tags: [history, review]
---

# History Retrieval Queue

Use this page for recall without rereading.

## Random person prompts

```dataview
TABLE era, domains, events
FROM "06 People"
WHERE type = "person"
SORT file.name ASC
```

For a selected person, answer from memory:

1. What problem were they actually solving?
2. What constraint mattered most?
3. Name one high-quality decision and one damaging decision.
4. Which success depended on context that would not transfer?
5. Which event best tests the story you tell about them?

## Event reconstruction

```dataview
TABLE start, end, themes
FROM "07 Events"
WHERE type = "historical-event"
SORT start ASC
```

For a selected event, reconstruct: structural pressure -> trigger -> key decisions -> turning point -> first-order result -> second-order result.

## Pattern falsification

Choose one note from `08 Patterns`. Find a counterexample. If you cannot find one, your pattern may be vague rather than true.
