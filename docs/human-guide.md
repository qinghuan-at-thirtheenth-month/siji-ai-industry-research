# SIJI Human Guide

This guide is for researchers using SIJI directly or asking an AI assistant to use it.

## The short version

Use SIJI as an **industry-world model**, not as an answer generator.

For broad questions, start by seeing the world before choosing keywords:

1. `get_world_overview` — understand the visible industry space.
2. Form a broad candidate set.
3. `list_changes` — see recent canonical changes.
4. `search_entities` / `get_entities` — resolve exact objects.
5. `expand_graph` / `trace_paths` — inspect neighborhoods and possible paths.
6. `get_facts` — check qualified facts and commercial stages.
7. `get_evidence` — reopen source references.
8. `compare` — align explicit candidates.
9. Use public Web sources independently for freshness, commercialization timing, and market expectations.

For a narrow question about a known company/product, starting from entity search is fine; you do not need a world overview every time.

## Nine public research primitives

| Primitive | Use it for |
| --- | --- |
| `get_world_overview` | See the current visible industry world before deciding where to search |
| `search_entities` | Resolve company/product/business/position names to canonical IDs |
| `get_entities` | Reopen exact typed references |
| `list_changes` | Discover recent canonical changes or track known objects |
| `expand_graph` | Explore neighborhoods and adjacent positions/relationships |
| `trace_paths` | Find bounded graph connections and alternate routes |
| `get_facts` | Reopen explicit facts or inspect qualified facts for known entities |
| `get_evidence` | Reopen citations/source references behind facts and relationships |
| `compare` | Align explicit candidates without pretending missing values are zero |

See [Research API](research-api.md) for the current HTTP/MCP mapping.

## The most important interpretation rules

Do not collapse different states into one:

```text
exists
≠ qualified
≠ mass produced
≠ ordered
≠ shipped
≠ delivered
≠ revenue
```

Do not convert graph structure into transactions:

```text
same industry position
≠ supplier/customer
≠ purchase order
≠ causal dependency
```

Always preserve `verified`, `review_required`, conflicts, time scope, and coverage notes.

## Broad research workflow

Suppose the question is:

> What could be the next AI-infrastructure inflection?

A good workflow is:

```text
world overview
→ candidate universe across all relevant chains
→ Web screening for timing and external reality
→ freeze a shortlist
→ graph / facts / evidence drill-down
→ Web verification of the important branches
→ independent market-expectation check
```

Do not rank candidates by graph density or change counts alone. High density means “more visible structure,” not “better investment.”

## SIJI and Web are complementary

**Use SIJI for:**

- stable identity;
- maintained product/position structure;
- typed relationships;
- known commercial facts;
- evidence states and citations;
- unknowns and coverage;
- research navigation.

**Use Web for:**

- latest developments outside the snapshot;
- reading public original sources;
- independent verification;
- information outside current SIJI coverage;
- securities prices, valuation, expectations and crowding.

A Web fact stays Web provenance until it is separately processed into SIJI. Agent analysis remains analysis.

## What a trustworthy answer looks like

A good answer should make clear:

- what SIJI directly supports;
- what came from public Web verification;
- what is inference;
- what is still unknown;
- what would falsify the current view;
- whether the market-pricing question is actually supported.

See the [flagship case](../examples/next-inflection.md).
