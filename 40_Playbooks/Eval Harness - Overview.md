---
type: playbook
status: active
---

# Eval Harness — Overview

You need a way to evaluate prompts like software.

## Core idea
A prompt is a **behavioral program**. Test it with:
- fixed scenarios (golden tests)
- randomized variations (fuzzing)
- adversarial inputs (safety + injection)

## Artifacts
- Scenario library (YAML/JSON or Markdown)
- Expected outcomes (assertions)
- Scoring rubric
- Regression dashboard (even a spreadsheet works at first)

## Metrics (pick a few)
- Task completion rate
- Incorrect info rate
- Unnecessary escalation rate
- Time-to-resolution
- Policy violation count

Templates:
- [[40_Playbooks/Template - Scenario.md]]
- [[40_Playbooks/Template - Scoring Rubric.md]]
