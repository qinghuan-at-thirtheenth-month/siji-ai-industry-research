# Run Metadata & Trace

Published agent runs should include:

- `manifest.json` — run metadata and preregistered input hashes;
- `trace.jsonl` — timestamped public research trace.

A manifest records:

- case ID;
- model/version and reasoning configuration;
- run time;
- input hashes;
- tool scope;
- budget / stopping conditions;
- SIJI schema/version where applicable;
- data-as-of / snapshot IDs returned by SIJI;
- whether human route intervention occurred.

The trace records user task, public planning summaries, tool decisions, tool requests/results, synthesis checkpoints, and stop decisions.

Credentials, restricted source text, non-public endpoints, and hidden reasoning are excluded.
