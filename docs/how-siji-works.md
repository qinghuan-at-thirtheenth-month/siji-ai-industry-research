# How SIJI Works

SIJI is designed as an **industry world model for research**, not an answer generator.

## Start from the world when the question is broad

For an open-ended question, the useful order is:

```text
world overview
→ candidate universe
→ graph / change / entity drill-down
→ facts and evidence
→ public-Web verification
→ market evidence separately
```

`get_world_overview` exposes the current visible company/product/business/position identities and typed relationship skeleton. It lets an Agent see the research space before it decides which keywords deserve attention.

For a narrow known-entity question, an Agent may start directly from entity search/get.

## Evidence organization

```text
Product / business
→ Industry position
→ Company participation
→ Commercial fact
→ Evidence reference
→ Original source
```

## Research derivation

```text
industry change
→ affected product layer
→ alternative / adjacent / upstream / downstream paths
→ concrete companies and products
→ facts and evidence
→ conditional conclusion
→ next verification / invalidation signal
```

The second chain is analytical. A graph path is not automatically causal proof.

## Roles

**SIJI** provides stable identity, world structure, typed relationships, commercial facts, evidence state, coverage and source anchors.

**Public Web** provides independent freshness, original-source verification, information outside SIJI coverage, and market evidence.

**The Agent** decides which branches matter, compares alternatives, preserves uncertainty, and chooses the next verification.

## Hard boundaries

- structural adjacency ≠ transaction;
- product existence ≠ qualification;
- qualification ≠ mass production;
- mass production ≠ order;
- order ≠ shipment/delivery;
- delivery ≠ revenue;
- nearby product maturity ≠ target product maturity;
- unknown/partial ≠ non-existence;
- industry evidence ≠ market-pricing evidence.

See [Agent Guide](agent-guide.md) and the [flagship case](../examples/next-inflection.md).