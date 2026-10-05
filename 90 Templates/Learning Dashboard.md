# Learning Dashboard

## Active frontier

```dataview
TABLE status, last_tested, next_review, length(evidence) AS "Evidence items"
FROM "02 Concepts"
WHERE type = "concept" AND (status = "frontier" OR status = "fragile")
SORT last_tested ASC
```

## Due for review

```dataview
TABLE status, last_tested, length(evidence) AS "Evidence items"
FROM "02 Concepts"
WHERE type = "concept" AND next_review AND date(next_review) <= date(today)
SORT next_review ASC
```

## Secure concepts

```dataview
TABLE last_tested, length(evidence) AS "Evidence items"
FROM "02 Concepts"
WHERE type = "concept" AND status = "secure"
SORT last_tested DESC
```

## Known misconceptions

```dataview
LIST
FROM "02 Concepts"
WHERE type = "concept" AND misconceptions
SORT last_tested DESC
```

## Recent sessions

```dataview
TABLE topic, status
FROM "01 Sessions"
WHERE type = "learning-session"
SORT date DESC
LIMIT 8
```
