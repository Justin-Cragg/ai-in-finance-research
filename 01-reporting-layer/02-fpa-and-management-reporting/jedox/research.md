# Jedox

*Layer: Reporting → **FP&A & management reporting** (planning, budgeting, forecasting, management reporting; Excel-friendly) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Jedox (private, Germany) |
| **Product** | Jedox planning platform: web, **Excel add-in**, Integrator (ETL), Models marketplace |
| **AI brand** | **JedoxAI**: Reporting, Planning, Modeling and Knowledge agents; Planning Wizards (ML forecasting); **Jedox MCP** |
| **AI maturity** | **Stage 3→4**: in-product agents plus an MCP connector that opens governed planning data to ChatGPT / Copilot / Claude / Gemini (separate add-on licence) |
| **Infrastructure** | JedoxAI runs on **Microsoft Azure**; data processed transiently, not used to train models; conversations not stored after logout [3] |
| **NZ relevance** | **Visible and growing NZ presence**: Jedox Elevate events in **Auckland (22 Jul 2026)** and **Christchurch (23 Jul 2026)** [4][5]; NZ customer **ANZCO Foods** presented on replacing spreadsheet-based weekly modelling [5]; Auckland VAR **Visual Intelligence** and ANZ Diamond partner Minerva [6][7]. Popular with NZ mid-market, food/primary and manufacturing groups that want "Excel-like but governed" |

## Executive summary
- Jedox is the **Excel-native** FP&A choice. Finance teams keep the spreadsheet look and feel but gain a central database, workflow and version control. That's why it does well in NZ mid-market groups that have outgrown Excel but don't want an Anaplan-scale programme.
- **JedoxAI is a four-agent "intelligence engine"**: **Reporting Agent** (KPI and variance insights in business language, builds views from plain English), **Planning Agent** (driver analysis, revenue/demand forecasting, churn prediction, anomaly detection), **Modeling Agent** (speeds up model and integration build) and **Knowledge Agent** (in-product help, script generation). [1][2]
- **Jedox MCP** gives external AI tools (ChatGPT, Copilot, Gemini, Claude, custom agents) **governed access to planning models, KPIs, hierarchies and business logic**, including **write-back aligned to approval workflows**. It respects existing Jedox permissions and is a separately licensed add-on. [8]

## How the AI works — plain English

### Planning Wizards — explainable ML forecasting [2]
- Learn from historical and real-time data to produce **explainable forecasts** for revenue, cash flow and demand, then run "what-if" scenarios on top.

### JedoxAI agents [1][2]
| Agent | What it does |
|---|---|
| **Reporting Agent** | Reads Dynatables and KPIs, pinpoints the drivers of performance, explains them in plain English; builds views and ad-hoc reports from natural language; outputs presentation-ready material |
| **Planning Agent** | Driver analysis, revenue and demand forecasting, churn prediction, **anomaly detection** |
| **Modeling Agent** | Accelerates data integration, model build and report creation |
| **Knowledge Agent** | Answers "how do I…" questions from the knowledge base and Academy; generates and reviews Integrator scripts |

### Jedox 26 release (May 2026) [9]
- Natural-language creation and refinement of views; conversational ad-hoc exploration; JedoxAI inside the Integrator for script generation and troubleshooting; native Python support.

### Jedox MCP [8]
- A **governed connection layer**: the AI tool sees the *planning context* (business logic, hierarchies), not raw tables. Read *and* write-back are possible, with write-back running through approval processes and human oversight. Decision lineage is maintained for audit.

## Where it lands in the finance process
| Process | AI help | Human still owns |
|---|---|---|
| Monthly management reporting | Reporting Agent explains KPI movements and drafts insight | Narrative to the board |
| Budget / reforecast | ML baseline via Planning Wizards; scenario what-ifs | Assumptions, targets |
| Operational planning (demand, weekly modelling) | Planning Agent forecasting and anomaly flags | Operational decisions |
| Model maintenance | Modeling and Knowledge Agents reduce key-person risk | Model design governance |

## Governance & control considerations
- Data residency: JedoxAI processing stays in the customer's Azure region for most regions [3]. **Confirm the region for NZ tenancies** (likely Australia).
- Jedox MCP needs its **own add-on licence**, so budget for it separately. [8]
- MCP write-back is powerful. Restrict it to approved assistants and keep it behind Jedox workflow approvals.

## Presentation talking points
- **"Keep Excel, lose the risk"**: Jedox is the realistic FP&A step for many NZ mid-market groups, and now has an AI layer and MCP like the enterprise suites.
- NZ proof point: **ANZCO Foods** moving weekly modelling beyond the spreadsheet (Jedox Elevate Christchurch 2026). [5]
- Shows the MCP pattern isn't just for the giants. Mid-market planning tools are opening up to the client's chosen AI front door too.

## Sources
1. Jedox Knowledge Base — *JedoxAI*: https://knowledgebase.jedox.com/jedox/ai/jedoxai.htm
2. Jedox — *AI for FP&A: Plan the future with JedoxAI*: https://www.jedox.com/en/platform/ai/
3. Jedox Knowledge Base — *JedoxAI FAQ* (Azure hosting, data handling): https://knowledgebase.jedox.com/jedox/ai/jedoxai-faq.htm
4. Jedox — *Jedox Elevate 2026 Auckland* (22 Jul 2026): https://www.jedox.com/en/roadshow/auckland/
5. Jedox — *Jedox Elevate 2026 Christchurch* (23 Jul 2026; ANZCO Foods session): https://www.jedox.com/en/elevate/christchurch/
6. Jedox — *Partner: Visual Intelligence (Auckland)*: https://www.jedox.com/en/partner/visual-intelligence/
7. Minerva — *Jedox* (ANZ Diamond Partner 2026): https://minerva.com.au/platforms/jedox/
8. Jedox — *Jedox MCP: Connect enterprise AI to trusted planning data*: https://www.jedox.com/en/platform/mcp/
9. Jedox — *Jedox 26 Major Release* (May 2026): https://www.jedox.com/en/blog/jedox-26-major-release/
