# Snowflake

*Layer: Data (cloud data platform / warehouse) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Snowflake (NYSE: SNOW) |
| **Product** | Snowflake AI Data Cloud |
| **AI brand** | **Cortex AI** — Cortex Agents, Cortex Sense, **CoWork** (formerly *Snowflake Intelligence*), **CoCo** (formerly *Cortex Code*), Semantic Views, AI Agent Identity |
| **AI maturity** | **Stage 4** – GA business-user agent (CoWork), governed agent identities, MCP gateway (Natoma acquisition) |
| **NZ relevance** | **Has an NZ region (AWS Asia Pacific (New Zealand), ap-southeast-6, Auckland)** — the only one of the "big two" lakehouse/warehouse vendors with in-country hosting today [3] |

## Executive summary
- Snowflake's thesis: *"The model is not your unique advantage. It's when you combine models with your data."* Its AI is about letting finance ask questions of governed warehouse data — accurately. [1]
- **CoWork (GA, June 2026)** is a business-user AI agent over Snowflake data: governed dashboards ("Artifacts"), Deep Research across data, memory of user preferences — with an **Excel add-in**, Slack and iOS. [1]
- **Accuracy depends on semantics**: Cortex Sense assembles data + business definitions at query time; Snowflake cites **86% accuracy on structured questions with full business context** vs generic models alone. **Semantic Views** let finance define "revenue", "gross margin" etc. once. [1]

## How the AI works — plain English

### 1. The semantic layer — "teach the AI your chart of accounts"
- **Semantic Views** define shared business logic (metrics, joins, definitions) without SQL; **Semantic View Autopilot** (preview) auto-generates them from existing tables. [1]
- **Cortex Sense** pulls data, definitions and operational knowledge together at query time so answers use *your* definitions. [1]
- Snowflake has told customers to move from **Cortex Analyst** (text-to-SQL) to **Cortex Agents** (multi-step reasoning + tools) (Aug 2026). [2]

### 2. Agents for business users and builders [1]
| Capability | What it does | Status |
|---|---|---|
| **CoWork** (ex-Snowflake Intelligence) | Personal agent: ask questions, Deep Research, persistent dashboards; Excel add-in, Slack, iOS, Google Drive/Salesforce connectors | GA |
| **CoCo** (ex-Cortex Code) | Coding agent for data teams; scheduled automations | GA |
| **Cortex Training** | Fine-tune open-weight models inside Snowflake without moving data | Preview |
| **Cortex AISQL functions** | Call LLMs from SQL (classify, extract, summarise text — e.g. contract terms, invoice descriptions) | GA (earlier releases) |

### 3. Governance for agents [1][4]
- **AI Agent Identity (GA)**: each agent gets its own identity, access policies and data masking, separate from human users, with full audit trail.
- **MCP gateway** via Natoma acquisition: governs agents' calls to external systems.
- Unified monitoring and **cost management** for agent workloads.

## Finance use cases
| Use case | How |
|---|---|
| Self-serve finance Q&A | CoWork over governed finance marts with Semantic Views |
| Board pack data prep | Agents assemble multi-source data (ERP + CRM + ops) |
| Unstructured finance data | AISQL to extract terms from contracts, leases, invoices |
| Excel-centric teams | CoWork Excel add-in |

## Considerations
- **Consumption pricing** (credits) — AI queries add compute cost; monitor via cost management.
- Value depends on investing in the **semantic layer** — a finance data-governance task, not just IT.
- NZ residency: AWS Auckland region available [3]; check which Cortex models run in-region vs cross-region.

## Presentation talking points
- The "86% with business context" stat is a good illustration of why **finance definitions/semantic models are now an AI asset**.
- Agent Identity = the data-layer version of segregation of duties.

## Sources
1. Atlan — *Snowflake Summit 2026: all the announcements* (1–4 Jun 2026): https://atlan.com/know/snowflake/summit-2026-announcements/
2. Snowflake docs — *Aug 28, 2026: transition from Cortex Analyst to Cortex Agents*: https://docs.snowflake.com/en/release-notes/2026/other/2026-08-28-cortex-analyst-transition-cortex-agents
3. Snowflake docs — *Supported cloud regions*: https://docs.snowflake.com/en/user-guide/intro-regions
4. Snowflake — *Advances AI security for the agentic enterprise*: https://www.snowflake.com/en/news/press-releases/snowflake-advances-the-trusted-agentic-enterprise-era-with-unified-monitoring-and-cost-management/
5. SiliconANGLE — *Snowflake moves up the AI stack* (Jun 2026): https://siliconangle.com/2026/06/02/snowflake-moves-ai-stack-system-intelligence-still-built/
6. Snowflake — *Cortex AI for financial services*: https://www.snowflake.com/en/blog/cortex-ai-financial-services/
