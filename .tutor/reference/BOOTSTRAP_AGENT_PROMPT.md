# Bootstrap prompt for a coding agent

Set up a native-Linux Obsidian AI learning system using this `ai_learning_vault_kit` as the target design.

The goal is not merely to clone a repo. Build a reliable tutoring harness optimized for **extremely deep understanding at high learning velocity**: never skim over essential reasoning, but never waste time on detail that does not improve the learner's generative mental model.

## Environment

- Linux desktop.
- Native Obsidian.
- `tmux` is available/acceptable.
- Use my already-configured model/provider.
- Run the tutor harness from the Obsidian vault root.

## Tasks

1. Create or use an Obsidian vault named `AI-Learning-Vault` in a sensible location.
2. Create:
   `00 Home`, `01 Sessions`, `02 Concepts`, `03 Maps`, `04 Sources`, `05 Reviews`, `90 Templates`, `viz`, `.pi/skills`, `.pi/extensions`, `.pi/agents`.
3. Copy all templates and custom skills from this kit.
4. Inspect and reuse the useful runtime pieces from `https://github.com/amosblomqvist/learn`, especially:
   - `extensions/quiz.ts`
   - `extensions/ask-user-question.ts`
   - `extensions/md-log.ts`
   - researcher / Mermaid / SVG agents where compatible
   - visual-tools where useful
5. Keep this kit's custom modular pedagogy. Do not overwrite it with the repo author's personal monolithic `teach` skill.
6. Install/configure the current `pi` harness from its official documentation and verify it launches from the vault root.
7. Because this is native Linux, install/configure `tmux` subagents if the current compatible implementation works cleanly. Use them for research/verification and visual generation, but do not make the core teaching loop depend on a subagent successfully returning.
8. Make Obsidian render Markdown, MathJax, callouts, wikilinks and Mermaid cleanly.
9. Create `START_HERE.md` with exact commands for:
   - opening/locating the vault;
   - starting the tmux/pi session;
   - linking a session note with `/md-log`;
   - beginning a learning session;
   - resuming a previous topic.
10. Configure the system so every learning session follows:
    goal → diagnostic questions → minimal dependency DAG → Tier A/B node classification → deep/efficient teaching → discriminative checks → exit evaluation → persistence.
11. Ensure the tutor uses the `question-designer` skill. Pre-session and post-session questions must be high-information and adaptive, not generic textbook quizzes.
12. Ensure the tutor uses the `depth-efficiency-controller` skill:
    - extremely deep treatment for core generating ideas;
    - enough depth for enabling prerequisites;
    - skip/compress already-secure material;
    - defer peripheral rabbit holes;
    - advance at diminishing returns, not arbitrary question counts.
13. Add an end-of-session exit assessment using *new* examples/wording that tests reconstruction, transfer, boundaries, integration, and misconception rejection.
14. Persist what the questions actually demonstrated. Do not mark mastery because the learner said "I get it."
15. Test end-to-end on a nontrivial but compact concept. The test must include:
    - an adaptive diagnostic question whose follow-up changes based on the answer;
    - a Mermaid dependency DAG;
    - at least one MathJax equation;
    - one deeply taught Tier A node;
    - one transfer/error-diagnosis question;
    - an exit evaluation with novel wording;
    - an updated concept note and Learner Model.
16. Fix path/dependency/configuration problems you encounter. Do not stop at file generation.
17. Create `SETUP_REPORT.md` explaining:
    - installed components;
    - exact architecture;
    - any manually required plugin/model login;
    - tests run and results;
    - optional enhancements not required for normal use.

Keep the system simple enough to be reliable. Complexity is justified only when it improves diagnosis, teaching, verification, visualization, or durable learner state.
