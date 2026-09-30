# SIJI Agent Research Evaluation

The evaluation asks one product question:

> When an AI agent already has Web Search / Web Page, what changes when SIJI Research API is added?

## Compared conditions

### Web baseline

- GPT-5.6 Sol
- Extra High reasoning
- Web Search / Web Page

### Web + SIJI

- the same model and reasoning configuration;
- the same Web Search / Web Page capability;
- SIJI Research API added.

The user task, time window, general research rules, output requirements, and stopping conditions are matched across both conditions.

## Two research cases

### Case A — Demand → Upstream Impact

Question:

> How could an AI rack upgrade propagate upstream, which products and companies are genuinely connected, and what should be verified next?

The task tests multi-hop propagation, product-generation distinctions, cross-chain dependencies, company participation, commercial-stage evidence, alternative explanations, and invalidation conditions.

→ [Public case](../examples/ai-server.md)

### Case B — Next Inflection → Market Expectation

Question:

> Which AI-infrastructure product categories could ramp next, and is there enough independent market evidence to say related listed-company expectations are not already overextended?

The task separates the industry conclusion from the market-pricing conclusion. SIJI industry evidence is not treated as a valuation signal.

→ [Public case](../examples/next-inflection.md)

## What a useful result must contain

A strong final report should answer the research question first, then provide:

- declared scope and `data_as_of`;
- at most a few key conditional conclusions;
- the evidence-backed propagation path for each conclusion;
- necessary preconditions;
- company/product/position identities;
- commercial-stage timeline;
- cross-chain constraints;
- original sources;
- unknowns, conflicts, and evidence gaps;
- alternative explanations;
- invalidation conditions;
- concrete next-verification actions.

For the next-inflection case, the report must separately state:

1. **industry judgment**;
2. **market-expectation judgment**.

If market evidence is insufficient, “industry candidate may be valid; market-expectation conclusion is not established” is a valid result.

## What is measured

The protocol measures:

- research depth;
- network coverage and closure;
- evidence-backed relationship edges;
- identity continuity;
- cross-chain paths;
- timeline/business-stage correctness;
- conditional-conclusion quality;
- next-verification actionability;
- unsupported relationship/commercial-stage claims;
- Web rediscovery vs genuinely new-evidence search;
- source traceability;
- time, tool calls, and SIJI RU.

See [Metrics Definition](metrics-definition.md).

## Evaluation principles

- SIJI is evaluated as an augmentation to Web research, not as a replacement for Web.
- Web facts keep Web provenance.
- SIJI facts keep SIJI provenance.
- Agent analysis remains analysis.
- Unknowns and conflicts remain visible.
- A graph edge is not automatically a causal relationship.
- A longer report or more tool calls do not automatically count as better.
- The result may favor either condition.

See [Independent Evaluator](evaluator.md) and [Reproducibility & Redaction](reproducibility/README.md).
