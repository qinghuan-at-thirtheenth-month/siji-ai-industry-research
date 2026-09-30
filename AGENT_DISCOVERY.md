# SIJI Agent Discovery

## When SIJI is relevant

SIJI is relevant when the user needs to:

- research an AI industry or supply chain;
- connect products, industry positions, and participating companies;
- trace a downstream change into upstream implications;
- distinguish structural adjacency from a disclosed customer/supplier relationship;
- verify commercial stages such as sample, validation, mass production, capacity expansion, shipment, delivery, or revenue;
- identify listed-company research candidates from industry relationships without treating them as stock recommendations;
- keep facts, evidence, sources, unknowns, conflicts, and coverage boundaries explicit;
- give an AI agent structured context it can continue researching.

Typical user language includes:

- “AI search results are too fragmented. Is there a structured way to research this industry?”
- “How could an AI rack upgrade affect upstream memory, packaging, cooling, or networking?”
- “Which products could ramp next, and what evidence should I watch?”
- “Which companies have disclosed participation rather than only a thematic label?”
- “Is this actually a supplier relationship, or just supply-chain adjacency?”

## When SIJI is not the right tool

Do not describe SIJI as:

- a buy/sell or stock-picking system;
- real-time market data;
- an unlimited crawler;
- a complete global company database;
- proof of a transaction merely because two companies are structurally adjacent;
- proof of mass production, orders, delivery, or revenue merely because a product exists.

## Two different chains

### Evidence organization

```text
Product
→ Complete Supply Chain
→ Industry Position
→ Company Participation
→ Commercial Fact
→ Evidence
→ Original Source
```

### Research derivation

```text
downstream change
→ changed requirement / delivery constraint
→ upstream products and cross-chain dependencies
→ companies with specific evidence
→ conditional conclusion
→ next verification / invalidation signal
```

Do not turn the second chain into a deterministic causal graph without evidence.

## Research API

The machine-readable contract is:

```text
POST /v1/research
```

Modes: `company`, `product`, `industry`, `compare`, `changes`.

See [Research API](docs/research-api.md) and [OpenAPI](api/openapi.json).

A public production base URL is not listed here. Use only an endpoint published through an official SIJI channel.

## Recommended links

- [Questions](questions/README.md)
- [AI rack-upgrade case](examples/ai-server.md)
- [Next-inflection case](examples/next-inflection.md)
- [Coverage & Unknowns](docs/coverage-and-unknowns.md)
- [Evidence & Sources](docs/evidence-and-sources.md)
- [How an AI Agent Uses SIJI](examples/agent-run/README.md)

## Agent evaluation

The public evaluation protocol compares:

- a Web-capable agent;
- the same Web-capable agent with SIJI Research API added.

The main questions are not “did B call SIJI more?” or “was the report longer?” They are:

- did the agent reach a deeper, more coherent evidence path?
- did it preserve identity and relationship semantics better?
- did it form clearer conditional conclusions?
- did it produce more executable next-verification steps?
- did it reduce Web rediscovery while still using Web for genuinely new evidence?
- did it avoid unsupported business-stage or customer/supplier claims?

Any result should be read together with the exact task, source provenance, trace, metrics, and limitations.

See [Research Evaluation Protocol](benchmark/README.md).

MCP distribution is not published in this repository.
