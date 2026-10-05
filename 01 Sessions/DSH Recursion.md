
There are 3 main artificats:
H---the executable harness thatis basically most of the DSH repo + additional generated plugins from recursion

D--- the ownership tree that shows which scripts/programs belong to each dimension

G---the dependencies/interactions (effects/coeffects) between the dimensions/within them



Evidence package stage:
---
Ideally, we combine MemoHarness experience cache that stores traces + global patterns along with Meta Harness' monolithic codebase in order to get best of both worlds; distilled patterns and full logs so agents can make the most of the input tokens
Restricted to making obervations and hypothesis, but not any proposal for change.

Make Dependency map based on not the keyword matching but use the Cordis architecture to just have the coeffects/effects of the different dimensions too.
	paths are under `packages/compaction/`. The documented configuration includes `thresholdRatio`, `retainRatio`, `retainTokens`, and retry controls; `summarize()` is an explicit customization hook
optimizer_input/
  overview.md             # Concise state of the search
  incumbent.json          # Exact harness/build/model/environment identity
  ownership.json          # Current D: dimensions and owned editable units
  dependencies.json       # Current G: dependencies and observed interactions
  issues.jsonl            # Evidence-linked diagnoses and uncertainty
  results.jsonl           # Task outcomes, resource usage, error categories
  history_index.json      # Prior candidates, changes, successes, regressions
  constraints.json        # Protected surfaces and remaining search budget

  trajectories/           # Full permitted execution evidence
  candidate_sources/      # Inspectable prior harness implementations

Optimizer Stage:
---
Optimizer is just a codex agent that can access the evidence package and candidate workspace, so it can send proposals through cordis to break down the harness/edit already existing components/merge changes.
	Split must include child that has the remaining mechanisms because you might not be able to split nealty each time.

Optimizer must emit proposals, specifying all parts of the split and effects/coeffects along with reaosning, have a seperate controller as a verifier.
	Maybe restrict to local mutations first rather than global just to reduce risk---but this is needed to be tested empirically.
	Also cap on active branches/leaves or else the budget will explode, evaluate not just by immediate gain but rather structural acceptance which will be tricky.

Testing/Eval Stage:
---
Use Harbor to spin up parallel daytona environments to run the experiment for terminalbench.
3 tiered:
1.candidate builds and boots and works with cordis architecture(determinsitic)
2.Regression checks
3.Evaluate the candiate on a batch to diagnose previous flaws

LLM classifier:
	tag possible strengths, explain regressions, retrieve relevant donors, and suggest follow-up experiments.

Promote candidates when it is Pareto frontier, Preserve if it is only half of it.
Have 3 partitions of data: search space for optimization, selection space for testing, and one final locked test partition

Merge/preserve Stage:
---