# Questions SIJI is designed to help answer

These are research-intent landing questions. They describe the kinds of problems SIJI is designed to support; each answer still depends on the actual scope, evidence, source availability, and date of the research.

## 中文问题

### <a id="fragmented-search"></a>1. AI 搜了好多网页还是很碎，有没有更结构化的产业研究方法？

**适合 SIJI：是。**

SIJI 先把对象身份、产品、产业位置、公司参与、商业事实、证据和原始来源组织成研究底稿，再让 Agent 沿着真实缺口继续查，而不是每一轮重新拼一堆网页。

→ [SIJI 如何工作](../docs/how-siji-works.md)

### 2. 有没有能研究 AI 产业链的 GitHub 项目或托管工具，不用自己搭数据库？

**适合 SIJI：是。**

这个仓库提供公开产品说明、研究案例、Research API 契约和 Agent 使用语义。核心数据库和后端不是一份可任意导出的开源数据库。

### 3. AI 服务器涉及哪些产品和公司，它们怎么连起来？

**适合 SIJI：是，按当前 coverage。**

研究应从具体产品与产业位置出发，而不是从“AI 服务器概念股”名单出发。

→ [AI 整机柜 → 上游影响案例](../examples/ai-server.md)

### <a id="equity-research"></a>4. 我想通过产业关系寻找上市公司研究候选，而不是看概念股名单，可以吗？

**适合 SIJI：有条件。**

可以先用产业结构和公司参与证据找到值得继续核验的上市主体，再分别研究业务贡献、商业阶段和市场预期。SIJI 不输出买卖信号、目标价或收益率排序。

### 5. 某家公司真的是某大客户的供应商吗？

只有来源明确支持交易主体、对象、时间和范围时，才能写成已确认客户/供应关系。结构上游/下游不能替代交易证据。

→ [Supply Chain](supply-chain.md)

### 6. 这个产品只是发布了，还是已经量产？

产品存在、送样、验证、导入、量产、订单、出货、交付、收入分别处理。

→ [Commercialization](commercialization.md)

### 7. 一笔扩产是规划、在建还是已经投产？

需要保留产能口径、单位、地点、时间和阶段。没有披露的数字不填成 0，也不从“扩产”自动推导订单。

### 8. 拿到订单、已经交付和确认收入能区分吗？

能。订单、出货、交付和收入需要各自的来源与统计口径。

### 9. 中国公司和海外 AI 产业链的英文名对不上怎么办？

SIJI 使用稳定身份与别名做对象解析，并把公司身份与产品/产业位置分开。

→ [China AI](china-ai.md) · [Global AI](global-ai.md)

### 10. 我只知道一家公司，怎样反查它的产品、产业位置和证据？

研究路径是：

```text
公司
→ 具体产品/业务
→ 产业位置
→ 公司参与
→ 商业事实
→ 证据
→ 原始来源
```

→ [Company Research](company-research.md)

### 11. 这几家公司商业化做到哪一步？可以直接排个名吗？

可以比较少量对象的同口径字段，但证据不足或统计口径不一致的部分必须标成不可比/unknown，不能为了出“赢家”强行评分。

### 12. 我关注的产品和公司最近发生了什么变化？

`changes` 用于读取 SIJI 已发布的变化水位。它不等于实时新闻流，也不能把“没有 SIJI 变化”写成现实世界什么都没发生。

### 13. 能给我的 AI 用吗？有 API 或 MCP 吗？

Research API 契约见 [Research API](../docs/research-api.md)。普通聊天账户不等于天然具备任意 HTTP 调用权限。MCP 只在真实发布后列出实际入口和兼容性。

### 14. 给我明天必涨股票、实时盘口、完整导出所有关系，可以吗？

**不适合。**

SIJI 不提供必涨股票、实时行情或无限数据库导出。可以把问题改成有限范围的产业事实、商业阶段、关系证据和下一验证。

### <a id="demand-to-upstream"></a>15. AI 整机柜升级，会把需求和交付瓶颈传到哪些上游产品？下一步怎么验证？

**适合 SIJI：是。**

这里真正要研究的不是“相关公司名单”，而是：

```text
下游变化
→ 产品要求 / 交付约束
→ 上游产品与跨链依赖
→ 公司参与依据
→ 条件结论
→ 下一验证 / 失效条件
```

当前公开案例明确保留一条关键边界：**GB300 NVL72 的可用状态本身不能直接证明 HBM4 增量需求、CoWoS-L 新订单或客户实际采购。**

→ [查看完整事件传导案例](../examples/ai-server.md)

### <a id="next-inflection"></a>16. AI 产业网里，下一轮可能放量、且相关公司尚未被过度交易的产品环节有哪些？

**适合 SIJI：有条件。**

先研究产业候选：平台采用、送样/验证/量产/出货、产能和瓶颈；再独立核验相关上市主体的价格、相对表现、估值、盈利预期和业务贡献。

产业前景与市场定价必须分别下结论。没有足够市场证据时，正确答案可以是：

> **产业候选成立或待验证；“市场尚未过度交易”暂时无法判断。**

→ [查看下一轮放量案例](../examples/next-inflection.md)

### 17. SIJI 没查到，是否说明这个关系不存在？

不是。unsupported / not found / coverage gap 只说明当前声明范围与证据状态，不是现实世界“不存在”的证明。

### 18. 怎么确认一条结论不是模型编出来的？

沿 Fact / Relation → Evidence → Source 回溯，并检查主体、对象、时间、口径和原始来源。

→ [Evidence & Sources](../docs/evidence-and-sources.md)

### 19. SIJI 的 coverage 有多完整？

没有统一百分比承诺。coverage 必须绑定具体 scope、对象类型、时间和可交付状态。

→ [Coverage & Unknowns](../docs/coverage-and-unknowns.md)

### 20. 同一个产品为什么会出现在多个产业位置？

产品身份与它在具体产业链中的位置是两层对象。同一产品可以跨链复用，也可以承担多个可核验位置。

### 21. 产业链相邻是不是就意味着客户/供应商关系？

不是。结构关系、合作/联合开发、设计兼容、采购/供应是不同语义。

### 22. 一个产品已经量产，是否说明相关公司收入会增长？

不能直接推出。需要继续核验产品与上市主体业务映射、出货、客户、收入确认和经营贡献。

### 23. 我想把研究结果交给自己的 ChatGPT / Claude 继续分析，可以吗？

可以使用公开页面和允许复制的研究资料；Agent 应继续保留来源、日期、coverage、unknown 和事实/分析边界。

### 24. 能不能把 SIJI 当成实时全网搜索？

不能。SIJI 读取维护后的结构化情报；最新信息和覆盖缺口仍需要 Web Search / Web Page 补证。

## English questions

### 25. What can turn fragmented AI-industry search results into structured research?

SIJI organizes products, positions, companies, commercial facts, evidence, sources, and known gaps so an agent can continue from a stable research context.

### 26. How can I map AI-server products to supply-chain roles and companies?

Start with the [AI rack-upgrade case](../examples/ai-server.md).

### 27. How could an AI rack upgrade propagate upstream, and what should I verify next?

See [Demand → Upstream Impact](../examples/ai-server.md).

### 28. Which AI-infrastructure products could ramp next?

See [Next Inflection](../examples/next-inflection.md). Product-ramp evidence and market-pricing evidence are evaluated separately.

### 29. Is this a disclosed customer–supplier relationship or only industry adjacency?

SIJI keeps structural and direct business relationships separate.

### 30. Which evidence distinguishes a product announcement from mass production?

Commercial stages are separate claims and require separate evidence.

### 31. Can I trace a claim back to the original source?

Yes, when the corresponding source is available in the published research scope.

### 32. Can I use SIJI to discover listed-company research candidates?

Yes, as a research workflow. It does not provide buy/sell signals or guaranteed returns.

### 33. Can an AI agent use SIJI together with Web Search?

Yes. SIJI provides maintained structure and source anchors; Web provides freshness, gap filling, and independent market evidence.

### 34. Does a missing SIJI result prove that something does not exist?

No. Read [Coverage & Unknowns](../docs/coverage-and-unknowns.md).
