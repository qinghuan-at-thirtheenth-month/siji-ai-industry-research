# Reproducibility Checklist

Before publishing evaluation artifacts:

- [ ] No API key, cookie, token, credential, or secret header value is present.
- [ ] No non-public endpoint is exposed.
- [ ] No restricted source full text is copied.
- [ ] No hidden chain-of-thought or model scratchpad is included.
- [ ] Capability labels use public names such as Web Search, Web Page, and SIJI Research API.
- [ ] Every key fact/relation retains provenance: SIJI, Web source, or agent analysis.
- [ ] Web-discovered facts are not relabeled as SIJI facts.
- [ ] Task/model/tool conditions and relevant timestamps are preserved.
- [ ] Failures, unknowns, conflicts, and unfavorable outcomes are preserved.
- [ ] Metrics use the preregistered definitions.
- [ ] Historical evaluation artifacts are not silently rewritten after later data updates.
