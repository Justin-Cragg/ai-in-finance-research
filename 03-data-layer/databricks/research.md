# Databricks

*Layer: Data (lakehouse — data engineering, analytics, ML/AI) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Databricks (private) |
| **Product** | Databricks Data Intelligence Platform (lakehouse); Azure Databricks; Databricks on AWS/GCP |
| **AI brand** | **Genie / Genie One**, **AI/BI**, **Agent Bricks**, **Lakebase**, Unity Catalog (Metrics, Business Glossary), Unity AI Gateway |
| **AI maturity** | **Stage 4** – production agent platform (100k+ deployed agents claimed) and business-user agent (Genie One) |
| **NZ relevance** | Fast-growing in ANZ (70%+ annual ANZ growth reported FY24 [5]); NZ country manager appointed [6]; NZ partners e.g. Theta. **No NZ-hosted region on AWS** (nearest: Sydney) [4]; Azure NZ North availability not confirmed — verify |

## Executive summary
- Databricks is the **"build your own finance AI" platform** — strongest where a finance or analytics team has data engineers/data scientists and wants custom models and agents.
- **Data + AI Summit (Jun 2026):** **Genie One** — an "agentic coworker" for business users across web, mobile, Slack and Teams that answers questions, creates documents, runs scheduled tasks and takes actions via MCP tools; moved to **pay-as-you-go** pricing (150 free DBUs/user/month) from Jul 2026. [1][2]
- **Unity Catalog business semantics** — Business Glossary, Domains and governed **Metrics** (KPIs reusable across dashboards and agents) — is Databricks' answer to "will the AI use our definition of EBITDA?" [2]

## How the AI works — plain English

### 1. Genie (business-user analytics) [2]
- Ask a question in plain English → Genie writes and runs the query on governed data, returns tables/charts and explanations.
- **Genie One** extends this into a coworker that also produces documents and runs recurring tasks.
- **Migrate from Power BI/Tableau (beta):** drop in a Tableau or Power BI file and Genie Code builds an AI/BI dashboard from it. [2]

### 2. Governed semantics — Unity Catalog [2]
- **Business Glossary** (authoritative definitions linked to data), **Domains** (business-aligned grouping), **Metrics** (governed KPIs). These feed the "Genie Ontology", improving agent accuracy.

### 3. Agent Bricks (build custom agents) [1][2]
- Full developer platform: choice of models, frameworks (LangGraph, CrewAI, Claude Code SDK), managed memory via **Lakebase** (serverless Postgres), isolated sandbox execution, and **automated evaluation** with synthetic tasks and "LLM judges".
- **Unity AI Gateway:** hard spend caps on external model providers and unified tracing of model and MCP activity. [1]

## Finance use cases
| Use case | How |
|---|---|
| Custom forecasting (demand, cash, revenue) | ML on lakehouse data; deploy as agent tools |
| Finance self-serve Q&A | Genie / Genie One over governed Metrics |
| Document-heavy processes (contracts, invoices) | Agent Bricks extraction agents with evaluation |
| BI rationalisation | Power BI/Tableau → AI/BI migration (beta) |

## Considerations
- Requires stronger in-house data engineering capability than Fabric or Snowflake's business-user tools.
- **Spend controls** on AI gateway and pay-as-you-go Genie One pricing — finance should set budgets/alerts. [1][2]
- **Data residency:** no NZ region on AWS; check Azure Databricks in NZ North vs Australia East if in-country hosting matters. [4]

## Presentation talking points
- Databricks vs Snowflake is converging on the same picture: **governed semantics + business-user agent + agent-building platform**. The differentiator for NZ clients is often skills and hosting, not AI features.
- The **automated evaluation** ("LLM judges") point is important for audit: how do you test an agent before it touches finance data?

## Sources
1. Enterprise DNA — *Databricks DAIS 2026: the actual announcements* (15–18 Jun 2026): https://enterprisedna.co/resources/news/databricks-dais-2026-live-announcements-agent-bricks/
2. Qubika — *Everything Databricks announced at DAIS 2026*: https://qubika.com/blog/everything-databricks-announced-dais-data-ai-summit-2026/
3. Databricks blog — *Agent Bricks: Data + AI Summit 2026*: https://www.databricks.com/blog/agent-bricks-dais-2026
4. Databricks docs — *Supported AWS regions*: https://docs.databricks.com/aws/en/resources/supported-regions
5. Databricks — *Over 70% annual growth in ANZ* (Mar 2024): https://www.databricks.com/company/newsroom/press-releases/databricks-sees-over-70-annual-growth-anz-market-enterprise-ai
6. Reseller News — *Databricks appoints Carol Brown as NZ country manager*: https://www.reseller.co.nz/article/2126827/databricks-appoints-carol-brown-as-new-zealand-country-manager.html
7. IT Brief NZ — *Databricks expands ANZ presence* (Apr 2025): https://itbrief.co.nz/story/databricks-expands-anz-presence-boosting-ai-capabilities
