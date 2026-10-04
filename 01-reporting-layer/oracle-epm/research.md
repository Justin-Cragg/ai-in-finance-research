# Oracle EPM (Hyperion HFM → Oracle Fusion Cloud EPM)

*Layer: Reporting (consolidation, close, planning, management & narrative reporting) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Oracle |
| **Products in scope** | Hyperion Financial Management (HFM, on-prem); Oracle Fusion Cloud EPM — Financial Consolidation & Close (FCCS), Planning/EPBCS, Narrative Reporting, Account Reconciliation (ARCS), Tax Reporting, Profitability & Cost Mgmt, Enterprise Data Management (EDM) |
| **AI brand** | "IPM" (Intelligent Performance Management) for ML; Generative AI + "Assistants"/"Agents" built on Oracle AI Agent Studio |
| **AI maturity (see root framework)** | **Stage 3 – Embedded agents** across most modules; ML forecasting is mature (since 2016) |
| **NZ relevance** | Deep legacy HFM/Hyperion installed base among NZ corporates and public sector; HFM customers are the obvious "move to cloud to get AI" conversation |

## Executive summary (for a CFO / FC)

- **The AI is only in the cloud.** HFM on-prem gets no meaningful AI. HFM 11.2 has Premier Support to **December 2030**, so the AI story is a migration story: HFM → FCCS. [3]
- **Oracle has the broadest module-by-module AI footprint in this layer** — ML forecasting, anomaly detection, GenAI narratives and, through 2026, conversational assistants for journals, consolidation runs, reconciliations, tasks and reporting. [1]
- **Delivered inside the quarterly update cycle at no separate AI line item historically**, but Generative AI now requires environments on the **26.04 update or later** — customers who defer updates lose access. [2]

## How the AI works — plain English

### 1. Predictive ML (mature)
- **Predictive Planning / Auto Predict** — statistical time-series models run against history to produce a baseline forecast that planners compare against their own numbers. [1]
- **Advanced Predictions (Aug 2025)** — multivariate forecasting: the model is given drivers (revenue drivers, headcount, macro indicators) not just the account's own history. [1]
- **Predictive Cash Forecasting (Apr 2024)** — daily/weekly cash forecasts from cash data streams. [1]
- **Bring Your Own ML** — data science teams can plug their own trained models into Planning. [1]

### 2. IPM Insights — "the system reviews the numbers before you do"
- Scheduled ML jobs scan actuals/forecasts and flag **anomalies, forecast bias and prediction variances**, then surface them on a dashboard with a confidence/impact score. GenAI narrative summaries of the insights were added in April 2025. [1][4]
- Extended into **FCCS (Jul 2025)** to flag outliers during the close, into Profitability (allocation behaviour) and into Tax Reporting (period-movement variances, Oct 2026). [1]

### 3. Generative AI (narrative & explanation)
- **Narrative Reporting** — GenAI drafts management commentary on key movements, variances and trends (Oct 2024), summarises preparer notes across a report package (Aug 2025), and **causality analysis** identifies which dimension members drove a value change (Jun 2026). [1]
- **Consolidation Job Analytics (Jul 2025)** — GenAI explains what happened in a consolidation run (performance, issues). [1]

### 4. Agents & assistants (2025–26) — natural-language control of the close
| Assistant / agent | What it does | Timing [1] |
|---|---|---|
| Consolidation Journals Assistant | Create/manage journals and workflow actions via chat | Oct 2026 |
| Consolidation Process Assistant | Run integrations and consolidations conversationally | Oct 2026 |
| Consolidation Diagnosis Agent | Diagnoses performance issues in data retrieval | Aug 2026 |
| ARCS assistants (×4) + Transaction Matching Assistant | Suggest matches for exceptions, auto-assign preparers/reviewers | Dec 2025 – Jun 2026 |
| Task Manager assistants | Review tasks; admins build close schedules by chat | Jun 2026 |
| Reporting Agent | Answers natural-language questions about report data; causal "top contributor" analysis | Jul / Oct 2026 |
| Planning Agent | Conversational drill-down, variance explanation, what-if | Roadmap |

These are built on **Oracle AI Agent Studio** (shared with Oracle Fusion ERP), which also lets customers build custom agents; the older Oracle Digital Assistant EPM skills are de-supported Nov 2026. [1][2]

## Where it lands in the finance process

| Process | AI help | Human still owns |
|---|---|---|
| Month-end close | Outlier flags pre-review, journal & consolidation by chat, task orchestration | Judgement on adjustments, sign-off |
| Reconciliations | ML match suggestions, auto-assignment | Approving exceptions |
| Group reporting | Drafted commentary, causal drivers, Q&A on reports | Final narrative, disclosure judgement |
| FP&A | Baseline ML forecast, driver-based predictions, Monte Carlo | Assumptions, targets |

## Governance & control considerations
- AI operates inside the EPM security model (same dimensions/roles), which is the key selling point vs. exporting to a general LLM.
- Release-cadence dependency: GenAI only on 26.04+ — IT change control needs to keep pace. [2]
- Agent actions (posting journals, running consolidations) need to be mapped into SOX-style/internal control frameworks — who is the "preparer" when an assistant posts?

## Presentation talking points
- "Your HFM isn't getting smarter" — AI is a cloud-only dividend; the 2030 support horizon frames the business case. [3]
- Oracle shows the progression from **predict → explain → act** better than any other single vendor in this layer.
- Good demo candidates: IPM Insights on a close, Narrative Reporting auto-commentary.

## Sources
1. EPMI — *Oracle Cloud EPM AI: A Module-by-Module Guide to Embedded Intelligence*: https://epmi.com/blog/oracle-cloud-epm-ai-a-module-by-module-guide-to-embedded-intelligence/
2. Oracle — *Cloud EPM September 2026 What's New*: https://docs.oracle.com/en/cloud/saas/readiness/epm/2026/epm-sep26/26sep-epm-wn-t77898.htm
3. US-Analytics — *HFM: Deciding on Your Next Steps* (HFM 11.2 Premier Support to Dec 2030): https://www.us-analytics.com/hyperionblog/hyperion-financial-management-deciding-on-your-next-steps
4. Oracle docs — *About IPM Insights*: https://docs.oracle.com/en/cloud/saas/planning-budgeting-cloud/pfusa/insights_about.html
5. Oracle — *FCCS data sheet*: https://www.oracle.com/a/ocom/docs/applications/epm/oracle-financial-consolidation-and-close-ds.pdf
