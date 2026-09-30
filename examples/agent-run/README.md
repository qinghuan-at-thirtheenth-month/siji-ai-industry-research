# How an AI Agent Uses SIJI

This directory defines a reproducible public format for showing how an AI agent uses SIJI during industry research.

The evaluation compares:

```text
A: GPT-5.6 Sol + Extra High + Web Search / Web Page
B: the same configuration + the same Web capability + SIJI Research API
```

## Two research cases

### Demand → Upstream Impact

The agent starts from a downstream AI rack/platform change and researches:

- what product requirements or delivery constraints change;
- which upstream products and cross-chain dependencies matter;
- which companies have specific participation evidence;
- which links are structural vs direct business relationships;
- what conditions must hold;
- what evidence would strengthen, weaken, or overturn the conclusion.

→ [Public case](../ai-server.md)

### Next Inflection → Market Expectation

The agent researches which product categories may accelerate over the next 6–12 months, then separately checks whether available market evidence supports a claim about listed-company expectations.

The industry conclusion and market-pricing conclusion are separate outputs.

→ [Public case](../next-inflection.md)

## Research behavior

A useful run should be able to:

- move across products, positions, and companies;
- follow upstream/downstream relationships for several hops;
- identify cross-chain connections;
- preserve product/platform generation identity;
- build commercial-stage timelines;
- distinguish direct transactions from structural adjacency;
- follow newly discovered objects;
- preserve unknowns, conflicts, and evidence gaps;
- form conditional conclusions rather than fact lists;
- produce concrete next-verification and invalidation steps;
- separate source-backed facts from agent analysis.

The SIJI-enabled condition can move between SIJI and Web as needed. SIJI provides maintained identity, structure, published relationships, facts, coverage, and source anchors. Web provides freshness, original-source verification, gap filling, and independent market evidence.

## Artifact structure

- [Demand → Upstream task](cases/demand-to-upstream.md)
- [Next Inflection task](cases/next-inflection.md)
- [Prompt inputs](prompt/README.md)
- [Run metadata and trace](run/README.md)
- [Tool calls](calls/README.md)
- [Final output](output/README.md)
- [Evaluation](evaluation/README.md)
- [Public trace schema](public-trace-schema.md)

A released run should make it possible to see **what the agent knew, what it checked next, where each key fact came from, and why the final conclusion stopped where it did**.
