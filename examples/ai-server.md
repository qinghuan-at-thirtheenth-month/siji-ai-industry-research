# Research Case — AI Rack Upgrade → Upstream Impact

## Research question

**How could an AI rack upgrade propagate upstream, and what should be verified next?**

This case starts from rack-scale AI infrastructure and asks what can — and cannot — be inferred about upstream memory and advanced packaging.

## Current conditional conclusion

The public evidence supports three separate facts:

1. NVIDIA lists **GB300 NVL72** as available and describes it as a fully liquid-cooled rack-scale system with 72 Blackwell Ultra GPUs and 36 Grace CPUs.
2. Micron disclosed **HBM4 36GB 12H** in high-volume production for NVIDIA Vera Rubin and **192GB SOCAMM2** in high-volume production for the same platform in March 2026.
3. TSMC states that its first **CoWoS-L** at 3.5X reticle size has been in volume production since 2024.

Those facts do **not** establish a direct causal chain from “GB300 is available” to “HBM4 demand increased,” “CoWoS-L orders increased,” or “a named supplier received new revenue.”

The research implication is therefore conditional:

> Rack-scale AI platform evolution makes memory bandwidth, capacity, packaging scale, interconnect, cooling, and power constraints important research variables. But each upstream product generation must be tied to the relevant platform and commercial stage with its own evidence.

## Evidence path

```text
rack-scale platform change
→ system memory / bandwidth / packaging requirements
→ product-generation evidence
→ company participation
→ commercial stage
→ next verification
```

### Downstream starting point

NVIDIA describes GB300 NVL72 as a rack-scale platform and marks it “Available Now.”

Original source:
<https://www.nvidia.com/en-us/data-center/gb300-nvl72/>

### Memory evidence

Micron disclosed HBM4 36GB 12H high-volume production for NVIDIA Vera Rubin and 192GB SOCAMM2 high-volume production for Vera Rubin.

Original source:
<https://investors.micron.com/news/press-release/2026/Micron-in-High-Volume-Production-of-HBM4-Designed-for-NVIDIA-Vera-Rubin-PCIe-Gen6-SSD-and-SOCAMM2-03-16-2026/default.aspx>

The important boundary is generation and platform identity: a Vera Rubin memory disclosure is not automatically evidence about GB300 customer procurement.

### Advanced-packaging evidence

TSMC states that CoWoS-L entered volume production in 2024 and that its first 3.5X-reticle CoWoS-L is in volume production.

Original sources:

- <https://3dfabric.tsmc.com/english/dedicatedFoundry/technology/cowos.htm>
- <https://investor.tsmc.com/static/annualReports/2024/english/index.html>

Again, production status is not the same as a quantified new capacity addition, named customer order, or revenue contribution.

## What would change the conclusion?

The next useful evidence is not another generic “AI demand is strong” article. It is evidence that closes one of the missing links:

- platform-specific memory configuration or qualification;
- named product/platform compatibility;
- supplier qualification or disclosed transaction;
- capacity expansion with unit/time scope;
- shipment/delivery evidence tied to the relevant generation;
- customer deployment volume;
- revenue or operating contribution attributable to the product/business.

## Invalidation / alternative explanations

The upstream thesis weakens if:

- the relevant platform uses a different memory/package generation;
- qualification or production timing slips;
- packaging, power, thermal, or networking constraints move the bottleneck elsewhere;
- alternative architectures reduce the expected component intensity;
- public availability does not translate into deployment volume.

## What SIJI contributes

SIJI is designed to keep the product identity, industry position, company participation, commercial stage, evidence, and source separate so an agent can continue from a known object without turning structural adjacency into a transaction claim.

SIJI-derived facts and Web-derived facts keep separate provenance.

See the [Agent Guide](../docs/agent-guide.md) and [Evidence & Sources](../docs/evidence-and-sources.md).
