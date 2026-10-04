# Anaplan

*Layer: Reporting → **FP&A & management reporting** (connected planning: finance, workforce, sales, supply chain) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Anaplan (private, Thoma Bravo-owned since 2022) |
| **Product** | Anaplan connected planning platform |
| **AI brand** | **Anaplan CoPlanner**, role-based **AI agents** (Finance Analyst, CoModeler, etc.), Anaplan Forecaster, PlanIQ, Agent Studio |
| **AI maturity** | **Stage 3** – role-based agents available; full CFO-office agent suite due ~Oct 2026 |
| **Infrastructure** | Runs agents on **Amazon Bedrock** (multiple foundation models) [2] |
| **NZ relevance** | Used by larger NZ/ANZ enterprises for cross-functional planning (e.g. Holcim Australia & NZ case study [4]); delivered mainly via Australian partners. Primarily a **planning** rather than statutory-reporting tool |

## Executive summary
- Anaplan's AI targets the **"connected planning"** problem — linking finance plans to sales, workforce and supply chain — rather than the statutory close.
- **Dec 2025:** role-based agents (Finance Analyst, Workforce Analyst, Sales Analyst, Supply Chain Analyst) available; **CoModeler** builds planning models from natural-language requests (GA Q1 2026). [1]
- **Jun 2026:** announced a full **Office of the CFO agent suite** (FP&A, treasury, controllership, tax, audit, IR, corp dev…) due by October 2026. Architecture: **LLM for conversation, Anaplan's deterministic engine for the maths** — so numbers are calculated, not "generated". [2]

## How the AI works — plain English

### The design principle: "LLM talks, engine calculates" [2]
The large language model handles the conversation and context; Anaplan's calculation engine does all arithmetic and business logic. This avoids the classic LLM failure of inventing numbers, and every figure is auditable back to the model.

### Agents [1]
| Agent | What it does |
|---|---|
| **Finance Analyst** | Monitors performance, detects deviations, surfaces business drivers, supports month-end |
| **CoModeler** | Builds/extends planning models from plain-English requests (reduces dependence on scarce model builders) |
| Workforce / Sales / Supply Chain Analysts | Same pattern for headcount, revenue, supply & demand |
| **Custom Agent + Agent Studio** | Build your own governed AI analysts |
| Autonomous agents (H1 2026 roadmap) | Spot anomalies and trigger workflows with human oversight |

### Predictive ML
- **Anaplan Forecaster** (Oct 2025) and **PlanIQ** — ML forecasting accessible to business users without data scientists. [1]

### CoPlanner
- Conversational generative-AI layer for asking questions of plans and getting explanations/insights. [3]

## Where it lands in the finance process
| Process | AI help |
|---|---|
| FP&A / reforecast | ML forecasts, agent-driven variance explanation |
| Cross-functional planning | Agents that link finance to sales/workforce/supply plans |
| Model build & change | CoModeler reduces build time and key-person risk |

## Governance & control considerations
- Deterministic-engine design is a strong answer to "can I trust the AI's numbers?" [2]
- Most new agents are 2026 releases — check GA status per agent before positioning. [1][2]

## Presentation talking points
- Use Anaplan to illustrate the **"LLM + deterministic engine"** architecture — a pattern every finance AI tool will need.
- CoModeler addresses a real NZ constraint: scarcity of experienced planning-model builders.

## Sources
1. Anaplan — *Anaplan Introduces New Suite of Role-Based AI Agents* (9 Dec 2025): https://www.anaplan.com/news/anaplan-introduces-new-suite-role-based-ai-agents/
2. Enterprise DNA — *Anaplan Puts AI Agents in the CFO's Office* (Jun/Jul 2026): https://enterprisedna.co/resources/news/anaplan-agentic-enterprise-cfo-finance-agents-2026/
3. Anaplan — *Anaplan CoPlanner*: https://www.anaplan.com/platform/anaplan-coplanner/
4. Anaplan — *Holcim Australia and New Zealand customer story*: https://www.anaplan.com/customers/holcim-anz/
5. ChannelLife NZ — *Anaplan names first Kiwi channel partner*: https://channellife.co.nz/story/anaplan-names-first-kiwi-channel-partner
