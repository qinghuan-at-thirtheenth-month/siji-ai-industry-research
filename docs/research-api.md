# SIJI Research API

SIJI exposes one research contract:

```text
POST /v1/research
```

Supported modes:

- `company`
- `product`
- `industry`
- `compare`
- `changes`

The response is a structured research packet built from maintained, published intelligence.

A packet can include:

- stable subject identity;
- research scope;
- products and positions;
- companies;
- relationships;
- claims and milestones;
- evidence and sources;
- unknowns and conflicts;
- coverage;
- changes;
- usage / RU;
- response hash.

JSON and Markdown are two representations of the same logical research packet.

## Machine-readable contract

See [OpenAPI](../api/openapi.json).

## Availability

A public production base URL is not listed in this repository. Use only an endpoint published through an official SIJI channel.

MCP distribution is not published here. Any future MCP adapter should expose the same research semantics rather than a separate fact system.
