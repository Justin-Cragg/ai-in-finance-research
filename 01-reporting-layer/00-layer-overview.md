# Reporting Layer — Market Leaders in NZ & AI Overview

*Last researched: 5 Oct 2026 · Audience: CFO / FC*

## What this layer is
The systems that take ledger data and turn it into **consolidated, controlled, decision-ready numbers and narrative**: consolidation & close, account reconciliation, FP&A/planning, management reporting, and external/statutory reporting (annual reports, XBRL, climate statements).

> **Challenge on the original framing:** "HFM, Workiva, Workday, Planful" mixes three different jobs. For the decks it is cleaner to show the reporting layer as three sub-layers:
> 1. **Consolidation & close** (Oracle EPM/HFM, OneStream, CCH Tagetik)
> 2. **Planning & management reporting / FP&A** (Workday Adaptive, Anaplan, Planful, Board, Jedox)
> 3. **External / statutory reporting** (Workiva)
>
> And for the **vCFO deck** a fourth, SME tier matters more than any of the enterprise tools: **Fathom, Spotlight Reporting, Syft (now Xero)** — see below.

## Top 5 in the NZ market (enterprise / upper mid-market)

| # | Supplier / product | Primary job | Why it's top 5 in NZ | AI maturity* | Headline AI |
|---|---|---|---|---|---|
| 1 | **Oracle EPM** (Hyperion HFM → Cloud EPM/FCCS) | Consolidation, close, planning, narrative reporting | Largest legacy installed base among NZ corporates & public sector; HFM migration wave to 2030 | Stage 3 | Broadest module-by-module AI: IPM Insights, GenAI narratives, journal/consolidation/recon assistants |
| 2 | **OneStream** | Unified consolidation + planning + reporting | Gartner MQ Leader; main HFM replacement competitor; NZ partners | Stage 4 | SensibleAI Agents (GA May 2026) + MCP "Finance Agentic Layer" into Copilot/ChatGPT/Claude |
| 3 | **Workday Adaptive Planning** | FP&A, management reporting | Most common FP&A tool in NZ mid/upper-mid market; strong local partners | Stage 2→3 | Adaptive Decision Intelligence (Monte Carlo, commit-to-plan), ML anomaly detection, MCP |
| 4 | **Workiva** | Annual report, XBRL, sustainability, GRC | De-facto external-reporting platform for listed/large entities; climate statements | Stage 3→4 | Tie-Out, Roll-Forward, XBRL Validation, Sustainability Disclosure agents; Workiva Knowledge |
| 5 | **Anaplan** | Connected planning (finance + ops) | Large ANZ enterprise footprint; cross-functional planning | Stage 3 | Role-based agents (Finance Analyst, CoModeler), "LLM talks, engine calculates" |

\*Maturity stages defined in the root README.

### How the top 5 were chosen
There is no published NZ market-share data for CPM/EPM. Ranking is a judgement based on: (a) global analyst position (Gartner MQ Financial Close & Consolidation 2025 leaders include OneStream and CCH Tagetik [1][2]; Apps Run The World EPM vendor rankings [3]), (b) visible NZ/ANZ partner ecosystem and customer stories, (c) relevance to Deloitte NZ clients. **Validate with Deloitte NZ's EPM practice before presenting.**

### Considered but not in the top 5
| Product | Why not top 5 (NZ) | AI note |
|---|---|---|
| **Planful** | Credible mid-market FP&A + consolidation tool but thin NZ presence (served via Australian reseller Forpoint) [4] | Analyst Assistant (Oct 2025) and Planner Assistant (Apr 2026) — natural-language forecasting grounded in Planful Predict [5] |
| **CCH Tagetik** (Wolters Kluwer) | Gartner Leader globally; smaller NZ base | Embedded GenAI and ML |
| **IBM Planning Analytics (TM1)**, **Board**, **Jedox**, **Prophix** | Niche/legacy pockets in NZ | Varying |
| **Microsoft Power BI** | Arguably the most-used *management reporting* tool in NZ finance teams — but it's a BI tool. Covered under the **Data layer** (Microsoft Fabric) | Copilot in Power BI |

## SME / vCFO tier (critical for the Virtual CFO deck)
These sit on top of Xero/MYOB and are the reporting tools vCFO practices actually use.

| Product | NZ angle | AI capability (summary) |
|---|---|---|
| **Spotlight Reporting** | NZ-founded advisory reporting/forecasting platform for accountants [6] | "Spotlight AI" generates/reformats commentary in executive summaries and action plans; AI suggestions [7] |
| **Fathom** | Very widely used by NZ/AU accountants for management reporting & consolidation | **Commentary Writer** (Feb 2026, Pro plan) — AI-generated commentary and analysis on reports [8] |
| **Syft → Xero Analytics** | Acquired by Xero (2024) and being built into Xero's core analytics [9] | See ERP layer → Xero |

*Recommendation:* if the vCFO deck needs depth here, add these as a "Reporting – SME tier" folder in a later pass.

## Cross-cutting themes for the decks
1. **Predict → Explain → Act.** Every vendor has moved from ML forecasting (predict) to GenAI commentary (explain) to agents that run journals, tie-outs or scenarios (act).
2. **System of record + any AI front door.** OneStream, Workiva, Workday and Anaplan all now expose governed data to Copilot/ChatGPT/Claude/Gemini via MCP. The finance platform keeps permissions and audit trail; the chat tool becomes the interface.
3. **"LLM talks, engine calculates."** Trustworthy finance AI keeps arithmetic in deterministic engines; the LLM only handles language (Anaplan explicit; Oracle/OneStream similar).
4. **AI is a cloud dividend.** On-prem HFM gets nothing — the AI case is now part of the HFM migration business case (Premier Support to Dec 2030).
5. **Commercial models are shifting to consumption** (Workday Flex Credits; advanced tiers at Workiva) — AI needs its own budget line.
6. **Human-in-the-loop by design** — tick-marks, commit-to-plan, approval chains — maps directly to internal control frameworks.

## Tool folders
- `oracle-epm/research.md`
- `onestream/research.md`
- `workday-adaptive-planning/research.md`
- `workiva/research.md`
- `anaplan/research.md`

## Sources
1. OneStream — *Leader in 2025 Gartner MQ for Financial Close and Consolidation*: https://www.onestream.com/news/onestream-again-recognized-as-a-leader-in-the-2025-gartner-magic-quadrant-for-financial-close-and-consolidation-solutions/
2. Wolters Kluwer — *CCH Tagetik Leader in 2025 Gartner MQ for FCC*: https://www.wolterskluwer.com/en/news/pr-2025-cch-tagetik-leader-gartner-magic-quadrant-financial-close-consolidation
3. Apps Run The World — *Top 10 EPM Software Vendors*: https://www.appsruntheworld.com/top-10-epm-software-vendors-and-market-forecast/
4. Forpoint — *Planful ANZ reseller agreement*: https://forpoint.com.au/forpoint-strengthens-planful-reach-over-anz-with-new-reseller-agreement/
5. Planful — *Planner Assistant launch* (29 Apr 2026): https://planful.com/pressrelease/planful-launches-planner-assistant/
6. SmartCompany — *NZ startup Spotlight Reporting closes $5m Series A*: https://www.smartcompany.com.au/startupsmart/new-zealand-startup-spotlight-reporting-closes-5-million-series-a-round-to-rapidly-expand-globally/
7. Spotlight Reporting: https://www.spotlightreporting.com/
8. Fathom — *What's new*: https://www.fathomhq.com/whats-new-in-fathom
9. Xero blog — *Xero to acquire Syft*: https://blog.xero.com/news-events/xero-to-acquire-syft/
