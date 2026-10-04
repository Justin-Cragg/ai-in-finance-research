# Oracle — NetSuite (mid-market) & Fusion Cloud ERP (enterprise)

*Layer: ERP · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Oracle |
| **Products** | **Oracle NetSuite** (upper-mid-market cloud ERP); **Oracle Fusion Cloud ERP** (enterprise) |
| **AI brand** | NetSuite: **NetSuite Next**, Ask Oracle, AI Canvas, SuiteAgents, **NetSuite AI Connector Service (MCP)**. Fusion: **AI Agent Studio**, finance agents, **Fusion Agentic Applications** |
| **AI maturity** | Fusion **Stage 3→4** (22 agentic apps in 26B, included at no extra cost); NetSuite **Stage 3** with MCP open access (NetSuite Next rolling out, US-first) |
| **NZ relevance** | NetSuite is gaining traction in NZ's upper mid-market (often companies outgrowing Xero) [7]; Fusion is used by a smaller set of large NZ enterprises/public sector. Same vendor as the reporting layer's Oracle EPM |

## Executive summary
- **Oracle includes its ERP AI in the subscription** — Fusion's finance agents and the 22 agentic applications in Release 26B carry **no additional licence cost**, a clear contrast to SAP AI Units and Microsoft Copilot Credits. [2][3]
- **Fusion agents:** Payables, Ledger, Planning, Payments agents; plus "agentic applications" such as **Collectors Workspace** that run whole processes (e.g. collections) and escalate only for judgement. [2][3]
- **NetSuite:** the **AI Connector Service (MCP)** (Oct 2025) lets Claude or ChatGPT read/write NetSuite under the user's own role; **NetSuite Next** adds Ask Oracle (natural-language query), AI Canvas, narratives and agentic workflows — but **Ask Oracle is US/Canada-only today**, other countries planned. [4][5][6]
- **SuiteWorld is 25–28 Oct 2026** — expect new announcements; revisit this note after. [6]

## How the AI works — plain English

### Oracle Fusion Cloud ERP
**Finance agents (announced Oct 2025, built with AI Agent Studio)** [2]
| Agent | What it does |
|---|---|
| **Payables Agent** | Takes invoices from email/portals/EDI/PDF → extracts data, matches PO/receipt, codes accounting, checks tax/policy, routes approval |
| **Ledger Agent** | Continuous monitoring of the ledger; answer questions in natural language; auto-creates adjustment journals |
| **Planning Agent** | Trend/variance analysis, event-driven predictions, what-if |
| **Payments Agent** | Evaluates early-payment discounts, virtual cards, financing; manages bank interactions and exceptions |

**Fusion Agentic Applications (Mar 2026, Release 26B)** [3]
- A step beyond single agents: **multiple agents coordinated to run an end-to-end process**. Finance examples: **Collectors Workspace** (continuously prioritises and performs collections outreach to reduce DSO) and **Claims Settlement Workspace** (claim → cash reconciliation).
- 22 shipped in 26B, included in Fusion subscriptions; requires 26A+, not available for E-Business Suite/on-prem. [3]

### Oracle NetSuite
| Capability | How it works | Availability |
|---|---|---|
| **AI Connector Service (MCP)** | OAuth 2.0; external AI (Claude, ChatGPT, any MCP client) can query records, saved searches, reports and SuiteQL and write data — **with exactly the permissions of the logged-in role** [4] | Launched Oct 2025 |
| **SuiteAgents** | Agents built with SuiteCloud that run *inside* NetSuite — currently a developer product [4] | Developer |
| **Ask Oracle** | Plain-English questions over NetSuite data instead of building saved searches [5] | US/Canada; more countries planned [6] |
| **AI Canvas** | Collaborative workspace / scenario planning on live ERP data [5] | NetSuite Next rollout |
| **Narrative summaries & report narratives** | Explains trends in plain language [5] | NetSuite Next |
| **Agentic workflows** | Payment proposals, vendor selection, reconciliations — choose "approve" or "autonomous" mode [8] | Rolling out |
| **Intelligent Close Manager; AI bank transaction matching** | Close status across subsidiaries; reconciliation suggestions trained on history [5] | Tier-dependent |
| **NetSuite EPM agents** | Continuous reconciliation and NL planning [5] | Requires NetSuite EPM licence |

## Where it lands in the finance process
| Process | Fusion | NetSuite |
|---|---|---|
| AP | Payables Agent | Bill capture / agentic workflows |
| AR / collections | Collectors Workspace (agentic app) | — |
| Close & recs | Ledger Agent | Close Manager, AI bank matching, EPM agents |
| Analysis | Planning Agent | Ask Oracle, AI Canvas, MCP into Claude/ChatGPT |

## Governance considerations
- MCP permission model = the role's permissions, "no more, no less" — a clean control answer, but role design (esp. write access) becomes critical. [4]
- Choose "approve" vs "autonomous" mode deliberately per workflow. [8]
- Regional rollout lags — validate NZ availability before demoing. [6]

## Presentation talking points
- **Price of AI differs radically by ERP vendor:** Oracle "included", SAP "AI Units", Microsoft "Copilot Credits", Workday "Flex Credits".
- NetSuite + MCP is a live, demonstrable example of **Claude/ChatGPT operating on ERP data under ERP permissions** — the pattern behind custom finance agents (e.g. AP posting skills built on SuiteTalk REST).

## Sources
1. Oracle Fusion Insider — *Agentic AI in ERP — four agents you can use today*: https://blogs.oracle.com/fusioninsider/agentic-ai-in-erp-four-agents-you-can-use-today
2. Oracle — *Oracle AI Agents help finance leaders…* (15 Oct 2025): https://www.oracle.com/news/announcement/ai-world-oracle-ai-agents-help-finance-leaders-accelerate-business-insights-and-boost-efficiency-2025-10-15/
3. Forsys — *Oracle Fusion Agentic Applications explained (March 2026 launch)*: https://www.forsysinc.com/blog/oracle-fusion-agentic-applications-explained-what-the-march-2026-launch-means-for-your-erp/
4. KORE1 — *NetSuite MCP Connector and SuiteAgents, explained*: https://www.kore1.com/netsuite-mcp-connector/
5. BrokenRubik — *NetSuite AI 2026: native features, MCP and custom agents*: https://www.brokenrubik.com/blog/netsuite-ai-guide
6. Versich — *NetSuite SuiteWorld 2026: dates, agenda, AI*: https://versich.com/blog/netsuite-suiteworld-2026/
7. Equerra — *Best ERP Software NZ 2026*: https://equerra.com/resources/best-erp-software-nz-2026
8. Gravity — *NetSuite AI Agent: what NetSuite Next actually ships in 2026*: https://gravity.fast/blog/netsuite-ai-agent/
