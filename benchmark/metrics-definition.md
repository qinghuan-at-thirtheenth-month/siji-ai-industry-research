# Evaluation Metrics

Metrics are preregistered before each evaluation and applied consistently to both conditions.

## Cost and activity

- total tool calls;
- total elapsed time;
- Web Search / Web Page request count;
- SIJI API call count and RU;
- repeated source/search count.

## Research depth and network structure

- maximum hop depth;
- average research depth;
- evidence-backed relationship-edge count;
- distinct companies / products / positions visited;
- complete product → company → position → company → evidence paths;
- cross-chain path count;
- discovered-object follow-up rate;
- network closure and unresolved frontier.

## Identity and continuation

- continuity of entity identity across research steps;
- stable-ID continuation where SIJI IDs are available;
- identity drift / duplicate-entity resolution count;
- repeated Web searches used only to rediscover known identity/context.

## Web efficiency

Web searches are classified as:

- **rediscovery** — re-finding identity, aliases, structure, or context already known;
- **new evidence** — finding fresh information, filling a gap, or verifying an original source.

Both counts and their ratio are reported.

## Timeline and relationship quality

- timeline event count;
- correctness of stage distinctions: release / sample / validation / mass production / capacity expansion / order / shipment / delivery / revenue;
- relationship-type overreach;
- commercial-stage overreach;
- platform/product-generation mix-ups.

## Conditional-conclusion quality

For each major conclusion:

- is the conclusion explicit rather than hidden in a fact list?
- is the evidence path traceable?
- are necessary preconditions stated?
- is the expected time window stated when justified?
- are alternative explanations present?
- are invalidation conditions present?
- does the conclusion stop where evidence stops?

## Next-verification quality

- number of concrete verification actions;
- whether each action names the object/metric/source class to inspect;
- whether the report explains what a positive or negative result would change;
- whether the action is executable rather than “continue to monitor.”

## Industry vs market separation

For the next-inflection case:

- industry conclusion is scored separately from market-expectation conclusion;
- product evidence is not treated as a valuation signal;
- company/security identity is resolved before market analysis;
- comparable market data use a declared date/window/basis;
- missing market evidence produces an explicit “not established” result rather than a forced ranking.

## Evidence discipline

- facts with original-source traceability;
- key relationships with source traceability;
- unsupported claim count;
- explicit preservation of unknown / conflict / evidence gaps;
- separation of sourced fact, SIJI contribution, Web contribution, and agent analysis.
