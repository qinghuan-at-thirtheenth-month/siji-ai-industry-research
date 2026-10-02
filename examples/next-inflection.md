# Flagship Case — Finding the Next AI Industry Inflection from the Whole Map

## Research question

> **Over the next 6–12 months, which AI-industry product layer is most likely to hit a meaningful inflection, become a hotspot or risk point, and may not yet be fully reflected in market expectations?**

This case uses SIJI as an industry world model, then independently verifies important branches on the public Web.

Evidence cutoff: **2026-10-02T01:54:55Z**

SIJI world data in the case: **2026-10-01**

## 1. Start with the industry world, not a few guessed keywords

Before narrowing candidates, the Agent consumed the visible SIJI world overview:

| Visible world | Count |
| --- | ---: |
| Industry categories | 24 |
| Industry positions | 85 |
| Connected companies | 947 |
| Products / business subjects | 1,499 |
| Company → subject edges | 1,534 |
| Subject → position edges | 1,533 |
| Company ↔ company edges | 61 |
| Position ↔ position structural edges | 36 |
| Total typed edges | **3,164** |

The map was screened across ten families: semiconductor inputs/equipment; EDA/compute; memory/advanced packaging/rack; board power/connectors; scale-up/network/optics; storage/data movement; facility power; cooling; cloud/training/inference/data lifecycle; demand/edge perception.

The map defined **what deserved to be considered** before Web verification narrowed the field. Graph density was not treated as an investment score.

## 2. Final industrial candidates

### #1 — Rack-level 800VDC power architecture

The near-term layer is not simply “data-center power.” It separates into:

- power rack / sidecar;
- PDU / Busway / DC distribution;
- fast DC protection and grounding;
- transient buffering / short-duration energy storage.

Public verification supports a live architecture transition: NVIDIA describes an H2-2026 MGX-compatible 800VDC power rack and a 2027 row-power-center path; Schneider separately describes rack-level power racks/sidecars as an immediate enabler.

The world model also keeps rack power, switchgear, PDU/Busway, transformer/substation and UPS/storage as distinct positions instead of merging them into one “power” theme.

### #2 — Context-memory / KV-cache storage

This was the most important product-layer upgrade from the whole-map view.

SIJI places **Huawei OceanStor M900 Context Memory Storage** in both storage and `Prefill / Decode / KV Cache` contexts. Graph paths connect the branch to Enterprise NVMe SSD, object storage and inference/KV-cache orchestration.

Public Web verification confirms that Huawei launched M900 as a dedicated context-memory storage product for large-scale AI inference, including tiering across memory/DRAM/SSD and shared KV-cache use.

The resulting hypothesis is more specific than “AI inference needs more enterprise SSD”:

> **Context memory may be becoming a distinct infrastructure product layer between compute, memory, storage and inference software.**

Important unknown: multi-vendor or hyperscaler adoption beyond the first dedicated product systems is still limited.

### #3 — Hybrid bonding / D2W metrology

The map and change feed expose dedicated hybrid-bonding and die-to-wafer metrology equipment inside advanced packaging.

Public evidence supports commercialization: Reuters reported Besi Q2 2026 orders of EUR292.9m and continued expansion of hybrid-bonding customers.

This makes hybrid bonding a strong industrial candidate, but also reduces the claim that it is still hidden from investors.

### #4 — High-capacity CDU / liquid-cooling distribution

SIJI facts separate CDU from cold plates, TIM and facility water/rejection.

Vertiv publicly announced its CoolChip CDU 2300 as NVIDIA DSX Ready, with a 2.3 MW cooling-capacity specification.

Industrial relevance is strong; market visibility is also already high.

### #5 — CPO / silicon-photonics optical engines

SIJI separates optical modules, silicon photonics, optical engines/CPO/NPO and laser sources.

Public evidence supports a transition toward CPO industrialization, but mature pluggable/laser production cannot be used as proof that CPO itself has reached the same mass-production stage.

### #6 — 224G AEC / high-speed copper

High-speed copper remains a real short-reach path and shared dependency. Its value depends on the copper-to-optics crossover in reach, power, thermal budget and system cost rather than a universal “copper wins” or “optics wins” conclusion.

### #7 — Physical-AI lidar

Robotics-lidar shipment growth validates a physical-AI demand branch, but it is not a shared bottleneck across the whole AI compute infrastructure.

## 3. What the world model changed

### It exposed a storage-to-inference bridge

M900 was not treated as a generic storage product. Its placement across storage and KV-cache/inference positions changed the research question from:

> “Will AI inference consume more SSD?”

to:

> “Is a dedicated context-memory infrastructure layer forming?”

That creates a different set of next verifications: additional vendors, hyperscaler deployments, common interfaces, installed capacity, TCO and attributable revenue.

### It kept product layers separate

800VDC rack power, PDU/Busway, switchgear, transformer/substation and UPS/storage are related but not interchangeable.

Likewise, mature EML/pluggable-optics facts do not automatically establish CPO mass production.

### It constrained what could be claimed

A participation or path can support an industry-placement statement without proving:

- a customer order;
- shipment volume;
- mass production;
- recognized revenue.

Missing or partial results were not treated as proof of non-existence.

## 4. Market conclusion

**market_assessment = insufficient_evidence**

This is deliberate.

The research found strong industry transitions, but market visibility is already substantial in power, cooling, hybrid bonding, optics and enterprise storage. Context memory is newer, yet public-equity exposure and multi-vendor earnings evidence remain weak.

Therefore:

> **A valid industry inflection does not automatically establish an under-priced security.**

## 5. Key public sources

- NVIDIA — [Why Scaling AI Compute Performance Requires a New Power Architecture](https://blogs.nvidia.com/blog/800-vdc-power-architecture-ai-factory/) — 2026-08-11.
- Schneider Electric — [5 Principles for 800 VDC in AI Data Centers](https://www.se.com/us/en/download/document/SPD_WP213_EN/) — 2026-03-02.
- ABB — [Direct-current portfolio for AI data centers](https://new.abb.com/news/detail/139013/abbs-new-direct-current-portfolio-aims-to-rewire-ai-data-center-energy-infrastructure) — 2026-09-23.
- Huawei — [OceanStor M900 Context Memory Storage](https://www.huawei.com/en/news/2026/9/hc-context-memory-storage) — 2026-09-17.
- TrendForce — [AI Server Demand Sustains Memory Contract Price Increases in 4Q26](https://www.trendforce.com/presscenter/news/20260930-13258.html) — 2026-09-30.
- Alibaba — [RTP-LLM](https://github.com/alibaba/rtp-llm) — production inference/KV-cache architecture.
- Besi — [Q2-26 and H1-26 results](https://www.besi.com/investor-relations/press-releases/details/be-semiconductor-industries-nv-announces-q2-26-and-h1-26-results/) — 2026-07-23; Q2 orders €292.9m with strong AI/hybrid-bonding demand.
- Vertiv — [CoolChip CDU 2300 qualified as NVIDIA DSX Ready](https://www.vertiv.com/en-us/about/news-and-events/corporate-news/2026/vertiv-coolant-distribution-unit-qualified-as-nvidia-dsx-ready-for-ai-factory-infrastructure/) — 2026-09-21.
- Lumentum — [Enabling the Next Phase of AI Optical Infrastructure](https://www.lumentum.com/en/blog/enabling-next-phase-ai-optical-infrastructure) — 2026-04-30.
- Hesai — [Q2/H1 2026 results](https://investor.hesaitech.com/static-files/41782b09-9c75-47ee-88ac-188e15b051a8) — 2026-08-18.

## 6. What to verify next

- **800VDC:** 2027 orders, supplier revenue, design wins, protection/distribution economics.
- **Context memory:** second/third vendors, independent deployments, standard interfaces, capacity, TCO and revenue attribution.
- **Hybrid bonding:** HBM4/HBM4E equipment shipments, throughput and yield.
- **CDU:** orders / installed MW and whether the bottleneck moves toward facility water/rejection.
- **CPO / 224G:** volume yield, serviceability, reach/power/cost crossover.

The point of the case is not that SIJI “knows the winning answer.” The point is that the world model changes **which product layers become visible, how they are connected, and what evidence the Agent knows it must verify next**.
