# AI in Finance — Research Repository (NZ market)

*Purpose: evidence base for two Deloitte presentations — (1) AI in financial reporting, (2) AI in virtual CFO services. Audience: CFO / Financial Controller. Round 1 researched 5 Oct 2026; round 2 (reporting layer split into three sub-layers + SME/vCFO tier) 5 Oct 2026.*

## Folder structure
```
ai-finance-research/
├── README.md                        ← this file: framework, index, cross-layer themes
├── 01-reporting-layer/
│   ├── 00-layer-overview.md         ← three sub-layers, top 5 per sub-layer, themes
│   ├── 01-consolidation-and-close/
│   │   ├── 00-sublayer-overview.md
│   │   ├── oracle-epm/  onestream/  blackline/  floqast/  cch-tagetik/
│   ├── 02-fpa-and-management-reporting/
│   │   ├── 00-sublayer-overview.md  ← enterprise top 5 + SME/vCFO tier
│   │   ├── workday-adaptive-planning/  anaplan/  jedox/  ibm-planning-analytics/  prophix/
│   │   └── sme-vcfo-tier/  fathom/  spotlight-reporting/
│   └── 03-external-reporting/
│       ├── 00-sublayer-overview.md  ← NZ context (no XBRL mandate, CRD narrowing)
│       ├── workiva/  caseware/
├── 02-erp-layer/
│   ├── 00-layer-overview.md
│   ├── xero/  myob/  microsoft-dynamics-365/  sap/  oracle-netsuite-and-fusion/
├── 03-data-layer/
│   ├── 00-layer-overview.md
│   ├── microsoft-fabric-power-bi/  snowflake/  databricks/  aws-redshift-quick/  google-bigquery-looker/
├── 04-general-ai-layer/
│   ├── 00-layer-overview.md
│   ├── microsoft-365-copilot/  chatgpt-openai/  claude-anthropic/  gemini-google/  perplexity/
└── 05-integrating-saas-layer/
    └── 00-layer-overview.md         ← placeholder with proposed sub-segments
```
Each tool folder contains `research.md` with: snapshot table, CFO executive summary, how the AI works (plain English), finance-process mapping, governance/cost considerations, presentation talking points, and numbered sources.

## The layer model — and where we've challenged it

| Original layer | Verdict | Change |
|---|---|---|
| Data (Snowflake, Databricks) | Keep, expand | **Add Microsoft Fabric/Power BI** (the NZ default), AWS and Google. Make the **semantic layer** explicit and include BI here |
| ERP (SAP Joule, Xero, NetSuite, Oracle) | Keep, relabel | Rename **"ERP & accounting systems"** (Xero isn't an ERP); **add Microsoft Dynamics 365** (largest NZ mid-market ERP); treat Oracle as one supplier (NetSuite + Fusion); note TechnologyOne for public sector |
| Integrating SaaS | Defer, split | Break into sub-segments (AP, expenses, AR, close/recs, payroll, treasury, tax, iPaaS) — see placeholder |
| Reporting (HFM, Workiva, Workday, Planful) | Keep, split — **done in round 2** | Now three sub-layer folders: **consolidation & close / FP&A & management reporting / external reporting**, each with its own NZ top 5. Close/recs tools (BlackLine, FloQast) moved here from Integrating SaaS. Planful in "considered" (thin NZ presence). **SME/vCFO tier** (Fathom, Spotlight, Syft/Xero) researched inside FP&A for deck 2 |
| General (Copilot, ChatGPT, Claude, Gemini) | Keep, reposition | It's the **front door on top of every layer**, not a peer layer. Added Perplexity as #5 |
| *(missing)* | **Add** | **Agent orchestration & governance** — the control plane for agents (Copilot Studio/Agent 365, Oracle AI Agent Studio, Snowflake Agent Identity, Databricks AI Gateway, Workday Flex Credits) |

**Suggested architecture picture for the decks:**
```
            ┌───────────── General AI "front door" (Copilot · ChatGPT · Claude · Gemini) ─────────────┐
            │                     ↕ MCP / connectors — permissions follow the source system           │
 Agent      │  Reporting: consolidation & close · FP&A · external reporting   (+ SME tier for vCFO)  │
 governance │  Integrating SaaS: AP · expenses · AR · close/recs · payroll · treasury · tax           │
 & cost     │  ERP & accounting: system of record                                                     │
 control    │  Data: warehouse/lakehouse · semantic layer · BI                                         │
            └───────────────────────────────────────────────────────────────────────────────────────┘
```

## AI maturity framework (used in every doc)
| Stage | Label | What it looks like |
|---|---|---|
| 1 | **Predictive ML** | Forecasting, anomaly detection, matching suggestions |
| 2 | **GenAI assist** | Drafted commentary, plain-English explanations, natural-language Q&A |
| 3 | **Embedded agents** | Agents that act inside the product (post journals, propose accruals, tie out reports) with human approval |
| 4 | **Open agentic** | Governed data and actions exposed to any AI front-end (MCP), multi-agent processes, agent identity/cost controls |

## Top 5 by layer (summary)
| Layer | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| **Reporting → Consolidation & close** | Oracle EPM (HFM→FCCS, ARCS) | OneStream | BlackLine | FloQast | CCH Tagetik |
| **Reporting → FP&A & mgmt reporting** | Workday Adaptive | Anaplan | Jedox | IBM Planning Analytics | Prophix |
| **Reporting → SME / vCFO tier** | Fathom | Spotlight Reporting | Syft → Xero Analytics | — | — |
| **Reporting → External reporting** | Workiva | Caseware | Oracle Narrative Reporting | Word/Excel + M365 Copilot | Sustainability data (Toitū, IBM Envizi) |
| **ERP & accounting** | Xero | MYOB | Microsoft Dynamics 365 | SAP | Oracle (NetSuite + Fusion) |
| **Data** | Microsoft Fabric/Power BI | Snowflake | Databricks | AWS | Google Cloud |
| **General AI** | Microsoft 365 Copilot | ChatGPT | Claude | Gemini | Perplexity |

*Rankings are informed judgement (no published NZ market-share data exists for these categories). Validate with the relevant Deloitte NZ practices before presenting.*

## Ten cross-layer themes (storyline seeds)
1. **Predict → Explain → Act.** Every layer has moved from ML predictions to GenAI explanations to agents that do work under approval.
2. **System of record + any AI front door.** OneStream, Workiva, Workday, Xero, NetSuite, Business Central, Snowflake all expose governed data via MCP; permissions and audit trail stay with the source system.
3. **"LLM talks, engine calculates."** Trustworthy finance AI keeps arithmetic in deterministic engines (Anaplan explicit; EPM/ERP vendors similar).
4. **Your policy manual and definitions become the program.** SAP's accruals agent reads a plain-language policy; data-layer AI depends on semantic models (Snowflake: 86% accuracy with business context). Finance-owned documentation and definitions are now AI assets.
5. **Drafts-first, human-in-the-loop is the control norm** — tick-marks (Workiva), commit-to-plan (Workday), accept/adjust/reject (SAP, D365), action summaries (Xero).
6. **AI is a cloud dividend.** HFM on-prem (support to 2030), SAP ECC (maintenance ends 2027), Oracle EBS get little or no AI — AI is now part of every migration business case.
7. **AI pricing is diverging and becoming variable.** Included (Oracle Fusion) vs consumption credits (Microsoft Copilot Credits, SAP AI Units, Workday Flex Credits, Snowflake/Databricks compute). CFOs need an AI opex line and usage monitoring.
8. **NZ data residency is a real differentiator.** In-country: Azure NZ North (Fabric), AWS Auckland (Snowflake; Claude on Bedrock). Not in-country: M365 Copilot processing, ChatGPT inference, Gemini in BigQuery, Databricks on AWS.
9. **NZ adoption is broad but shallow** — 91% of businesses use AI, 4% use it to transform core operations; the top 10% get 14× the AI output per worker. The opportunity is depth, not access.
10. **vCFO model shift:** SME platforms (Xero JAX, MYOB) automate bookkeeping and month-end; general AI (Claude Month-End Closer, Copilot) and SME reporting AI (Fathom Commentary Writer, Spotlight AI) automate packs and commentary — the vCFO moves from **producing** to **supervising agents across a portfolio and advising**.

## Deck mapping
| Deck | Primary layers | Key tools |
|---|---|---|
| **AI in financial reporting** | Reporting (all three sub-layers), Data, ERP (enterprise), General | Oracle EPM, OneStream, BlackLine, Workday Adaptive, Workiva, Caseware, Fabric/Power BI, Snowflake, SAP, D365, Copilot |
| **AI in virtual CFO services** | ERP (SME), Reporting SME tier, General | Xero, MYOB, Fathom, Spotlight, Syft, FloQast (+Xero), Caseware, Claude, ChatGPT, Copilot |

## Caveats & next steps
- Research reflects public sources to 5 Oct 2026; many features are preview/early-access or US-first — **check NZ availability before client use**.
- Upcoming events likely to change content: **NetSuite SuiteWorld (25–28 Oct 2026)**; Anaplan CFO-office agent suite due ~Oct 2026; Workday Adaptive Decision Intelligence broader release later 2026; MYOB–Microsoft first features late 2026.
- Round 2 done: reporting layer split into three sub-layers; SME/vCFO tier (Fathom, Spotlight) researched (former item (a)).
- Suggested next: (b) Integrating SaaS sub-segments (close/recs now covered under Reporting); (c) agent governance layer; (d) NZ case studies/quotes from Deloitte NZ practices; (e) confirm NZ availability of US-first agents (Caseware Disclosure Checklist, Workiva Benchmarking) and NZ data regions.
