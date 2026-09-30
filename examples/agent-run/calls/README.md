# Tool Call Artifacts

Published runs can store tool calls as numbered request/response pairs:

```text
001-web-search.request.json
001-web-search.response.json
002-siji-research.request.json
002-siji-research.response.json
...
```

SIJI and Web artifacts retain distinct provenance.

A SIJI request may document the header name `X-API-Key`, but never its value. Restricted source text is not copied into released artifacts.
