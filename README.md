# SIJI — AI Industry & Supply-Chain Research

**Trace downstream change to upstream implications.**

SIJI connects products, supply-chain roles, company participation, commercial milestones, evidence, and original sources so researchers and AI agents can follow a real industry question: **what may change next, which businesses are genuinely connected, what has actually been disclosed, and what evidence would confirm or overturn the view.**

[中文说明](README.zh-CN.md)

## Start with a research question

- **How could an AI rack upgrade propagate upstream, and what should I verify next?**
- **Which AI-infrastructure product categories could ramp next — and what evidence would test that view?**
- Which companies have disclosed participation rather than only a thematic label?
- Is a company a disclosed supplier/customer, or only structurally adjacent?
- Has a product reached sampling, validation, mass production, shipment, delivery, or revenue?
- Can I trace a research statement back to the original source?

Start with the [Questions index](questions/README.md).

## What a SIJI research path looks like

SIJI organizes evidence around:

```text
Product
→ Complete supply chain
→ Industry position
→ Company participation
→ Commercial fact
→ Evidence
→ Original source
```

A research conclusion then asks a different question:

```text
Downstream change or demand
→ product requirement / delivery constraint
→ upstream products and cross-chain dependencies
→ companies with specific participation evidence
→ conditional conclusion
→ next verification / invalidation signal
```

The two chains should not be confused. A graph edge is not automatically a causal claim.

## Featured research cases

### 1. AI rack upgrade → upstream impact

**Question:** How could an AI rack upgrade change upstream memory and advanced-packaging research?

**Current conclusion:** rack-scale availability by itself is not enough to claim incremental HBM4 demand, packaging orders, customer purchases, or deployment. The useful research path is to separate the rack-level change from the next-generation memory/package evidence and then test the missing links.

→ [Read the AI rack-upgrade case](examples/ai-server.md)

### 2. Next inflection → market expectation check

**Question:** Which AI-infrastructure product categories could ramp next, and have related listed-company expectations already become overextended?

**Current conclusion:** industry ramp evidence and market pricing are separate questions. Product, shipment, or capacity evidence does not by itself prove a security is under- or over-priced. The case therefore separates the industry candidate, the company/business mapping, and the independent market-evidence check.

→ [Read the next-inflection case](examples/next-inflection.md)

## Why the result is verifiable

A useful SIJI result keeps:

1. stable identity;
2. declared research scope;
3. relation/fact type;
4. evidence and source provenance;
5. commercial stage and time context;
6. unknowns, conflicts, and coverage gaps;
7. the distinction between source-backed fact and agent analysis;
8. the next observation that would strengthen, weaken, or overturn the conclusion.

See [Evidence & Sources](docs/evidence-and-sources.md) and [Coverage & Unknowns](docs/coverage-and-unknowns.md).

## Explore

- [Questions](questions/README.md)
- [How SIJI works](docs/how-siji-works.md)
- [AI rack-upgrade case](examples/ai-server.md)
- [Next-inflection case](examples/next-inflection.md)
- [Research API](docs/research-api.md)
- [OpenAPI contract](api/openapi.json)
- [Agent discovery guide](AGENT_DISCOVERY.md)
- [Agent research format](examples/agent-run/README.md)
- [Research evaluation protocol](benchmark/README.md)

## Availability

| Capability | Availability |
| --- | --- |
| Bilingual documentation | Available |
| Public research examples | Available |
| Evidence / coverage / unknown semantics | Available |
| Research API contract | Available |
| Public production API endpoint | Not listed in this repository |
| MCP distribution | Not published |
| Agent research evaluation method | Available |
| Reproducible evaluation results | Published with the corresponding public artifacts |

## Research API

SIJI uses one external research contract:

```text
POST /v1/research
```

Modes: `company`, `product`, `industry`, `compare`, `changes`.

It returns structured packets from maintained, published intelligence. It does **not** launch a new web crawl for every request.

See [Research API](docs/research-api.md).

## What SIJI is not

SIJI is not:

- a buy/sell or target-price system;
- real-time market data;
- an unlimited crawler;
- a promise of complete coverage for every company or industry;
- proof that structurally adjacent companies trade with each other;
- proof of mass production, orders, delivery, or revenue without evidence for those facts.

SIJI provides research structure, evidence, and explicit uncertainty. Investment decisions remain with the researcher.

## Data and sources

Public examples keep links to original publishers and separate source-backed facts from analysis. Credentials, restricted source text, and non-public system data are not included.

See [Data Usage](docs/data-usage.md).

### Additional narrow examples

The repository also keeps small examples that demonstrate identity and evidence semantics without claiming broad industry coverage:

- [Company → product example](examples/company-research.md)
- [Distributed-training software example](examples/training-software.md)
