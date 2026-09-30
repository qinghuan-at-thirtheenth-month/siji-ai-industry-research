# Public Agent Trace Schema

Each public trace event should be machine-readable and timestamped.

Recommended fields:

```json
{
  "event_id": "stable-public-event-id",
  "event_type": "decision | tool_request | tool_result | report_checkpoint",
  "capability": "Web Search | Web Page | SIJI Research API | null",
  "provenance": "web | siji | agent_analysis | null",
  "public_summary": "short observable decision/result summary",
  "request_ref": null,
  "result_ref": null,
  "response_hash": null,
  "charged_ru": null,
  "timestamp": "RFC3339"
}
```

Rules:

- `public_summary` is an observable rationale summary, not hidden chain-of-thought.
- SIJI results retain SIJI provenance.
- Web-discovered facts retain Web provenance.
- Credentials, non-public endpoints, restricted source text, and unrelated infrastructure metadata are excluded.
- Request/result artifacts are referenced only when they can be published.
- Failures, unknowns, conflicts, and unfavorable evidence remain visible.
