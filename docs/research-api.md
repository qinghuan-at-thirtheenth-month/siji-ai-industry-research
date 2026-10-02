# SIJI Agent Graph API

SIJI exposes nine typed research primitives over the maintained industry world model.

The public capability catalog is available at:

```text
GET /v1/agent/capabilities
```

## Operations

| Operation | HTTP path | MCP tool |
| --- | --- | --- |
| `get_world_overview` | `POST /v1/agent/world/overview` | `siji_get_world_overview` |
| `search_entities` | `POST /v1/agent/entities/search` | `siji_search_entities` |
| `get_entities` | `POST /v1/agent/entities/get` | `siji_get_entities` |
| `list_changes` | `POST /v1/agent/changes/list` | `siji_list_changes` |
| `expand_graph` | `POST /v1/agent/graph/expand` | `siji_expand_graph` |
| `trace_paths` | `POST /v1/agent/graph/paths` | `siji_trace_paths` |
| `get_facts` | `POST /v1/agent/facts/get` | `siji_get_facts` |
| `get_evidence` | `POST /v1/agent/evidence/get` | `siji_get_evidence` |
| `compare` | `POST /v1/agent/compare` | `siji_compare` |

## Recommended use

Broad research should normally begin with `get_world_overview`, so the Agent can understand the visible world before narrowing to familiar keywords.

Known-entity research can begin directly with `search_entities` or `get_entities`.

Continue with graph traversal, facts and evidence only as needed. Use public Web sources independently for current events, commercialization timing and market pricing.

## Semantics

The API preserves typed IDs, relationship semantics, evidence/review state, time context, coverage and continuation state.

Important rules:

- partial results are partial, not absence;
- missing values are unknown, not zero;
- a graph path is not causal proof;
- structural adjacency is not a company transaction;
- evidence metadata and source-content permissions are separate;
- market pricing is outside the industry-graph conclusion.

## Machine-readable contracts

- [Capability catalog](../api/capabilities.json)
- [OpenAPI](../api/openapi.json)

A production base URL is only valid when published through an official SIJI channel.