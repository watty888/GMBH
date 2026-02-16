---
type: playbook
status: active
---

# Prompt QC Playbook

This is the repeatable delivery process.

## 0) Intake (Discovery)
Inputs:
- Business goal for the agent
- Tooling platform (e.g. [[40_Playbooks/Platform Notes - Retell.md]])
- Available data sources + constraints
- Compliance constraints

Outputs:
- [[40_Playbooks/Voice Agent Prompt Spec.md]] draft
- Test plan skeleton

## 1) Define “Done”
You need explicit metrics:
- Task success rate (by scenario)
- Hallucination / incorrect-info rate
- Escalation quality (when it should hand off)
- Latency constraints for voice calls
- Safety/compliance constraints

## 2) Build a Prompt Spec (not just a prompt)
- System role & tone boundaries
- Tool contracts
- Grounding rules
- Failure handling + escalation
- “When unsure” policy

## 3) Build the Test Harness
- Golden path scenarios
- Edge cases (noisy input, interruptions, multiple intents)
- Adversarial tests (jailbreak-ish inputs, prompt injection via user)
- Regression suite (must pass every release)

## 4) Iterate
Loop:
Prompt change → test run → analyze failures → refine spec → repeat

## 5) Ship
- Version the prompt
- Store test suite
- Release notes
- Runbook for incidents

Links:
- [[40_Playbooks/Eval Harness - Overview.md]]
- [[50_Experiments/Template - Experiment.md]]
