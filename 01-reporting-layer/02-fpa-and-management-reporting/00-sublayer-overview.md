# Reporting Layer → FP&A & Management Reporting — NZ Market Leaders & AI Overview

*Last researched: 5 Oct 2026 · Audience: CFO / FC · Parent: [Reporting layer overview](../00-layer-overview.md)*

## What this sub-layer is
The tools that turn closed numbers into **forward-looking plans and internal decision packs**: budgeting, reforecasting, scenario and driver-based planning, workforce/sales/operational planning, KPI dashboards and the **monthly management report and board pack**.

It splits into two tiers that matter to different decks:
- **Enterprise / mid-market planning platforms** (deck 1, AI in financial reporting).
- **SME / vCFO reporting tools** sitting on Xero/MYOB (deck 2, AI in virtual CFO services). This tier is now researched (round 1 deferred it).

## Top 5 in the NZ market — enterprise / mid-market planning platforms

| # | Supplier / product | Sweet spot | Why it's top 5 in NZ | AI maturity* | Headline AI |
|---|---|---|---|---|---|
| 1 | **[Workday Adaptive Planning](workday-adaptive-planning/research.md)** | Mid / upper-mid FP&A | Most common FP&A tool in NZ mid-market, usually bought stand-alone; strong local partners (Fusion5) | Stage 2→3 | Adaptive Decision Intelligence (Monte Carlo, commit-to-plan); MCP to Claude/ChatGPT/Gemini |
| 2 | **[Anaplan](anaplan/research.md)** | Enterprise connected planning | Large ANZ enterprise footprint (e.g. Holcim ANZ); cross-functional planning | Stage 3 | Role-based agents, CoModeler, CFO-office agent suite; "LLM talks, engine calculates" |
| 3 | **[Jedox](jedox/research.md)** | Excel-native mid-market FP&A | **Visible, growing NZ presence**: Elevate events in Auckland and Christchurch (Jul 2026), NZ customer ANZCO Foods, Auckland VAR | Stage 3→4 | JedoxAI Reporting/Planning/Modeling agents; **Jedox MCP** with governed write-back |
| 4 | **[IBM Planning Analytics (TM1)](ibm-planning-analytics/research.md)** | Enterprise / public sector incumbent | Long-standing NZ TM1 base; NZ Platinum partner CorPlan (Auckland & Wellington) | Stage 3→4 | Planning Analytics Agent (Explain Cell, variance); **MCP tools on every deployment incl. on-prem** |
| 5 | **[Prophix](prophix/research.md)** | Mid-market planning + consolidation | Acquired ANZ partner Forest Grove (100+ ANZ customers) in 2025 | Stage 3→4 | Prophix One autonomous agents (Budgeting, Reporting, Planning, Consolidation); MCP server |

\*Maturity stages defined in the root README.

### Suites that are also strong FP&A choices (researched under Consolidation & close)
| Suite | FP&A angle | AI note |
|---|---|---|
| **Oracle EPM Planning (EPBCS)** | Common in NZ Oracle/HFM estates; arguably top 3 in NZ enterprise FP&A on installed base | Predictive Planning, Advanced Predictions, IPM Insights, Planning Agent (roadmap) — see [Oracle EPM](../01-consolidation-and-close/oracle-epm/research.md) |
| **OneStream** | Planning on the same model as consolidation | SensibleAI Forecast (AutoML + external drivers) — see [OneStream](../01-consolidation-and-close/onestream/research.md) |
| **Microsoft Power BI** | The most-used *management reporting* tool in NZ finance teams, but a BI tool | Copilot in Power BI — see [Data layer → Fabric/Power BI](../../03-data-layer/microsoft-fabric-power-bi/research.md) |

### How the top 5 were chosen
No NZ market-share data exists for FP&A software. Ranking is judgement based on (a) visible NZ partner and customer evidence (local partners, NZ events, named NZ customers), (b) global analyst position, and (c) relevance to Deloitte NZ clients. Dedicated FP&A platforms are ranked; multi-job suites (Oracle, OneStream) are covered once, under Consolidation & close. **Validate with Deloitte NZ's EPM practice.**

### Considered but not in the top 5
| Product | Why not top 5 (NZ) | AI note |
|---|---|---|
| **Planful** | Good mid-market fit; thin NZ presence (served via Australian reseller Forpoint) | Analyst Assistant (Oct 2025), Planner Assistant (Apr 2026), Planful Predict |
| **Pigment** | Fast-growing AI-first planning platform; APAC "growing" but little NZ evidence; covered by NZ trade press | Analyst, Modeler, Planner (preview), Supervisor agents; MCP server |
| **Board** | Niche NZ presence | AI capabilities not researched this round |
| **CCH Tagetik planning** | Small NZ base | Planning Sentinel agents — see [CCH Tagetik](../01-consolidation-and-close/cch-tagetik/research.md) |

## SME / vCFO tier

These sit on top of Xero / MYOB and are what NZ accounting and vCFO practices actually use to produce monthly packs, forecasts and group consolidations.

| # | Product | NZ angle | AI maturity* | Headline AI |
|---|---|---|---|---|
| 1 | **[Fathom](sme-vcfo-tier/fathom/research.md)** | Very widely used by NZ/AU accountants for management reports and consolidation; Access Group-owned | Stage 2 | **Commentary Writer** (Mar 2026): AI commentary with business context and **symbolic attribution** (every figure traceable) |
| 2 | **[Spotlight Reporting](sme-vcfo-tier/spotlight-reporting/research.md)** | **NZ-founded (Petone)**; dedicated SVCFO packaging | Stage 2 | **Spotlight AI** (Jul 2025) drafts highlights and recommendations; **AI Action Plans** (Apr 2026) |
| 3 | **Syft → Xero Analytics** | Built into Xero; Syft included free for practices on qualifying plans | Stage 2→3 | AI insights and JAX Q&A over analytics; native budgeting and benchmarking trailed for H2 2026 — see [ERP layer → Xero](../../02-erp-layer/xero/research.md) |
| — | **Calxa** (considered) | Australian budgeting/cash-flow tool popular with NZ NFPs and multi-entity SMEs; integrates Xero, MYOB, QuickBooks | Stage 1 | Limited verifiable AI; strength is multi-entity budgeting and long-range cash flow |

**SME-tier read-across:** all three leaders have converged on **AI-drafted commentary** in 12 months. Differentiation is shifting to **traceability** (Fathom), **actionability** (Spotlight action plans) and **being inside the ledger** (Xero/Syft + JAX). For a vCFO practice, the stored **business context** each tool asks for is effectively the practice's client knowledge, now a reusable asset.

## What AI is doing in FP&A & management reporting (themes)
1. **From a forecast number to a probability distribution.** ML baselines (Adaptive, Jedox Planning Wizards, IBM, Oracle) are table stakes; Monte Carlo ranges (Adaptive Decision Intelligence) and always-on scenario agents (Tagetik Planning Sentinel, Prophix Autonomous Planning) are the 2026 step.
2. **Explain-the-cell.** IBM Explain Cell, Jedox Reporting Agent, Prophix Reporting Agent and Anaplan Finance Analyst all answer "why is this number what it is?" from the model's own logic. That's the "LLM talks, engine calculates" pattern.
3. **Model-builder agents tackle the key-person problem.** Anaplan CoModeler, Jedox Modeling Agent, Prophix Architect and Pigment Modeler build or extend models from plain English. That matters in NZ, where experienced model builders are scarce.
4. **MCP is now standard, even in the mid-market.** Workday, Jedox, IBM (incl. on-prem TM1) and Prophix all expose governed planning data to the client's chosen AI front door. Licensing is often a separate add-on.
5. **Commentary is commoditised.** From Fathom to Oracle Narrative Reporting, drafting variance commentary is now a standard feature. Value moves to context, traceability and advice.

## Deck use
- **AI in financial reporting deck:** Adaptive (most likely NZ tool) for the forward view; IBM TM1 MCP as a counterpoint to "AI is cloud-only"; "explain-the-cell" demo.
- **vCFO deck:** Fathom vs Spotlight vs Xero/Syft. The monthly pack now drafts itself, so the vCFO's time moves to advice. Spotlight is the NZ-built story.

## Tool folders
- [workday-adaptive-planning/research.md](workday-adaptive-planning/research.md)
- [anaplan/research.md](anaplan/research.md)
- [jedox/research.md](jedox/research.md)
- [ibm-planning-analytics/research.md](ibm-planning-analytics/research.md)
- [prophix/research.md](prophix/research.md)
- SME / vCFO tier: [sme-vcfo-tier/fathom/research.md](sme-vcfo-tier/fathom/research.md), [sme-vcfo-tier/spotlight-reporting/research.md](sme-vcfo-tier/spotlight-reporting/research.md)

## Sources
1. Forpoint — *Planful ANZ reseller agreement*: https://forpoint.com.au/forpoint-strengthens-planful-reach-over-anz-with-new-reseller-agreement/
2. Planful — *Planner Assistant launch* (29 Apr 2026): https://planful.com/pressrelease/planful-launches-planner-assistant/
3. CFOtech NZ — *Pigment launches AI Analyst Agent*: https://cfotech.co.nz/story/pigment-launches-ai-analyst-agent-to-transform-business-plans ; Pigment — *AI info page* (agents, MCP server): https://www.pigment.com/ai-info-about-pigment
4. Xero — *Xero and Syft Together Elevate Advisory Services*: https://www.xero.com/us/campaign/analytics/ ; Digit — *The Best AI Tools for Xero Users in 2026*: https://digit.business/insights/xero/best-ai-tools-xero-users-australia
5. Calxa: https://www.calxa.com/
6. Tool-level sources are in each tool folder.
