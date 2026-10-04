# OneStream

*Layer: Reporting (unified consolidation, close, planning, reporting) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | OneStream (taken private by Hg in a US$6.4bn deal announced Jan 2026, completed ~Apr 2026) [5] |
| **Product** | OneStream unified CPM platform (consolidation, close, account reconciliation, planning, reporting) |
| **AI brand** | **SensibleAI** — Forecast, Studio, Agents; plus the **Finance Agentic Layer** (MCP) |
| **AI maturity** | **Stage 4 – Open agentic** (governed agents GA, exposed to ChatGPT/Copilot/Claude/Gemini via MCP) |
| **Analyst position** | Leader, 2025 Gartner Magic Quadrant for Financial Close & Consolidation [4] |
| **NZ relevance** | Growing ANZ footprint; typical target is HFM replacement for mid/large groups. Local partners include Power Tech Consulting (NZ) [6] |

## Executive summary
- OneStream's pitch is **"one governed financial data model, AI on top"** — because consolidation, planning and reporting share one model, AI answers come from the same numbers the board sees.
- **May 2026: SensibleAI Agents went GA** (Forecast, Finance Analyst, Search Analyst, Deep Analysis) along with the **Finance Agentic Layer**, which lets staff ask OneStream questions *from inside* Copilot, ChatGPT, Claude or Gemini — with OneStream identity and permissions enforced. [1]
- The most "open" AI architecture in this layer — relevant if the client's strategy is "Copilot/ChatGPT is our front door".

## How the AI works — plain English

### SensibleAI Forecast (predictive ML)
- An **AutoML** engine: it tests many model types per forecast line, picks and tunes the best, and blends internal data with **external drivers** (macro indicators, operational signals, weather, etc.). [2]
- Built for high-volume forecasting (thousands of SKU/site/customer series) where spreadsheets fail.
- **Explainability is the differentiator**: users see the drivers and model behaviour — important when the forecast is challenged by the board or auditor. [2]

### SensibleAI Studio (AI building blocks)
- A library of prebuilt ML and GenAI routines — anomaly detection, time-series analysis, data diagnostics, natural-language query, automated narrative commentary — that can be dropped into close, planning or reporting workflows without a separate data-science stack. [2]

### SensibleAI Agents (GA May 2026) [1]
| Agent | What it does |
|---|---|
| **Finance Analyst Agent** | Ask finance questions in plain English; returns tables, charts, variance explanations from live OneStream data |
| **Forecast Agent** | Natural-language questions about forecasts, grounded in real-time forecast data |
| **Search Analyst Agent** | Searches policies, memos and unstructured docs with source attribution |
| **Deep Analysis Agent** | Reads large document sets (contracts, compliance material) and connects patterns to answer complex questions |

### Finance Agentic Layer (MCP)
- Uses the open **Model Context Protocol** so external AI assistants can call OneStream "as a tool". Every request is **authenticated against the user's OneStream identity**, role permissions are applied, and activity is logged in OneStream. [1]
- Example given: a user in ChatGPT asks for an executive dashboard; ChatGPT pulls the governed OneStream report and formats it. [1]

## Where it lands in the finance process
| Process | AI help |
|---|---|
| Close & consolidation | Anomaly detection on intercompany/balances; analyst agent explains movements |
| Reporting | Auto-commentary; Q&A over the reporting model; answers from Copilot/Teams |
| FP&A | ML baseline forecasts with external drivers; forecast Q&A |
| Policy / technical accounting | Search & Deep Analysis agents over policies and contracts |

## Governance & control considerations
- Strong story: permissions and audit trail travel with the request even when the front-end is a third-party LLM. [1]
- Watch: the third-party LLM still sees the returned data — client AI policy must cover which assistants are approved.
- Ownership change (Hg private equity) — worth monitoring roadmap/pricing, but no announced change to AI direction. [5]

## Presentation talking points
- Best illustration of the **"system of record + any AI front door"** pattern that's emerging across this whole stack (Workiva, Workday, Anaplan are following).
- Contrast with Oracle: Oracle builds assistants inside its own UI; OneStream also pushes its data *out* to the assistant the user already uses.

## Sources
1. PR Newswire — *OneStream Unlocks Agentic AI for the Office of the CFO with Finance Agentic Layer; GA of SensibleAI Agents* (19 May 2026): https://www.prnewswire.com/news-releases/onestream-unlocks-agentic-ai-for-the-office-of-the-cfo-with-finance-agentic-layer-announces-general-availability-of-sensible-ai-agents-302775010.html
2. OneStream blog — *What Is SensibleAI Studio, Agents, and Forecast?*: https://www.onestream.com/blog/what-is-sensibleai-studio-agents-and-forecast/
3. ISG/Ventana — *OneStream Roadmap for AI and Agents*: https://research.isg-one.com/analyst-perspectives/onestream-roadmap-for-ai-and-agents
4. OneStream — *Leader in the 2025 Gartner MQ for Financial Close and Consolidation*: https://www.onestream.com/news/onestream-again-recognized-as-a-leader-in-the-2025-gartner-magic-quadrant-for-financial-close-and-consolidation-solutions/
5. Bloomberg — *Hg to take OneStream private in $6.4bn deal* (Jan 2026): https://www.bloomberg.com/news/articles/2026-01-06/buyout-firm-hg-to-take-onestream-private-in-6-4-billion-deal ; Alternatives Watch (completion, Apr 2026): https://www.alternativeswatch.com/2026/04/02/onestream-goes-private-again-6-4-billion-sale-hg-kkr/
6. Power Tech Consulting (NZ) — OneStream: https://www.powertechconsulting.co.nz/products/onestream/
