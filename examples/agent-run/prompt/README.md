# Task & Prompt Inputs

Both evaluation conditions share:

- the same user research task;
- the same general research rules;
- the same model and reasoning configuration;
- the same Web Search / Web Page capability;
- the same research date/time window;
- the same output requirements and stopping conditions.

The SIJI-enabled condition additionally receives:

- [SIJI Agent Rules](siji-agent-rules.md);
- the SIJI Research API tool definition.

The Web baseline does not receive SIJI-specific instructions.

## Case 1 — Demand → Upstream Impact

The user asks the agent to start from an AI rack/platform change and research upstream memory and advanced-packaging implications, including company participation, commercial stages, conditions, alternative explanations, and next verification.

The task must not prewrite the answer or the exact research route.

## Case 2 — Next Inflection → Market Expectation

The user asks the agent to compare a small set of AI-infrastructure product categories, identify evidence for a possible 6–12 month ramp, map the relevant businesses, and independently test whether comparable market evidence supports a statement about expectations.

The task must not assume that a valid candidate exists.

Evaluation tasks are preregistered before execution and remain the same across A/B conditions.
