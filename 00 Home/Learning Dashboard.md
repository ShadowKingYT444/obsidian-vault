# Learning Dashboard

> [!tip] Start small
> Pick one active topic. The tutor will diagnose the next useful step.

## Active frontier

```dataview
TABLE status, last_tested, next_review
FROM "02 Concepts"
WHERE type = "concept" AND (status = "frontier" OR status = "fragile")
SORT last_tested ASC
```

## Due for review

```dataview
TABLE status, last_tested
FROM "02 Concepts"
WHERE type = "concept" AND next_review AND date(next_review) <= date(today)
SORT next_review ASC
```

## Recent sessions

```dataview
TABLE topic, status
FROM "01 Sessions"
WHERE type = "learning-session"
SORT date DESC
LIMIT 8
```
