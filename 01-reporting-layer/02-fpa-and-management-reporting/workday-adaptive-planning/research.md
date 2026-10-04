# Workday Adaptive Planning (and Workday Financials agents)

*Layer: Reporting → **FP&A & management reporting** (plus a consolidation-lite capability) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Workday |
| **Products in scope** | Workday Adaptive Planning (stand-alone or with Workday Financials); Workday Illuminate agents for finance |
| **AI brand** | **Workday Illuminate** (agents); **Adaptive Decision Intelligence** (conversational planning) |
| **AI maturity** | **Stage 2→3** – solid ML (forecasting, anomaly detection); agents and conversational planning in early adopter / 2026 rollout |
| **NZ relevance** | Very common mid-market/upper-mid FP&A tool in NZ, often bought stand-alone on top of non-Workday ERPs. Local partners e.g. Fusion5 [6]; Workday runs an "Elevate New Zealand" event [7] |

## Executive summary
- **Most NZ customers use Adaptive *without* Workday Financials** — so the relevant AI is what is inside Adaptive itself: ML forecasting, anomaly detection and (new) Decision Intelligence.
- **Adaptive Decision Intelligence (launched May 2026, early adopter)**: ask a planning question in plain English, combine plan data with CRM/HR data, run Monte Carlo scenarios, and **commit the chosen scenario back into the governed plan** — aimed squarely at "shadow spreadsheets". Broader availability expected later in 2026. [1][2]
- Workday is also opening Adaptive to **Claude, ChatGPT and Gemini via MCP** on a governed semantic layer ("Adaptive Data Foundation"). [3]

## How the AI works — plain English

### 1. Predictive ML (available now)
- **Predictive Forecaster** — ML model produces a baseline forecast from history for comparison with the planner's view (scalability improved in 2026 R1). [4]
- **Anomaly detection** — uses **at least 24 months of actuals** to learn expected patterns and flags data points that deviate, directly in dashboards. [4]

### 2. Adaptive Decision Intelligence (conversational scenario planning) [1][2]
Four layers working together:
1. **Natural-language questions** across plan *and* operational data (e.g. "Why did the North region miss revenue?" → combines actuals, sales pipeline and staffing).
2. **Scenario modelling with Monte Carlo simulation** — produces a range of outcomes with probabilities, not a single number.
3. **Side-by-side scenario comparison.**
4. **Commit-to-plan** — the selected scenario flows back into the governed plan with full traceability and approvals.

### 3. Open AI access — MCP + Adaptive Data Foundation [3]
- A governed **semantic layer** supplies near-real-time data and business definitions so that external LLMs (Claude, ChatGPT, Gemini) can query Adaptive and get traceable, audit-ready answers.

### 4. Workday Illuminate finance agents (for Workday Financials customers) [5]
| Agent | What it does |
|---|---|
| Financial Close Agent | Automates and gives real-time visibility over the close workflow |
| Cost & Profitability Agent | Define allocation rules in natural language |
| Financial Test Agent | Continuously monitors financials for fraud and compliance exceptions |

Agents announced Sept 2025 for 2026 availability. Commercially consumed via **Workday Flex Credits** — an annual credit allocation included in the subscription, with top-ups, usable across all Workday agents. [5]

## Where it lands in the finance process
| Process | AI help |
|---|---|
| Monthly management reporting | Anomaly flags on dashboards; Q&A on variances |
| Budget / reforecast | ML baseline; Monte Carlo scenario ranges; commit to plan |
| Board / CFO decision support | Cross-system "why" questions (finance + CRM + HR) |
| Close (Workday Financials only) | Close agent, continuous controls testing |

## Governance & control considerations
- Commit-to-plan with traceability is a strong control answer to "AI changed my budget". [2]
- Decision Intelligence is **early adopter only** — no published customer outcomes yet; position as emerging. [2]
- Flex Credits = consumption-based AI cost; finance teams should budget for AI usage, not just licences. [5]

## Presentation talking points
- Adaptive is the **most likely tool in a NZ mid-market or vCFO-adjacent client** — use it to show where FP&A AI is going (from a forecast number → a probability distribution).
- "Shadow spreadsheet" framing resonates strongly with FCs.

## Sources
1. CFO Dive — *Workday launches AI tool aimed at easing FP&A workflows* (27 May 2026): https://www.cfodive.com/news/workday-launches-ai-tool-aimed-easing-fpa-workflows/821270/
2. UC Today — *How Effective is Workday Adaptive Decision Intelligence?*: https://uctoday.com/workday-adaptive-decision-intelligence-review
3. Workday — *Adaptive Planning AI Innovations*: https://www.workday.com/en-us/products/adaptive-planning/ai-innovation.html
4. QMetrix — *Workday Adaptive Planning 2026 R1 Release Review*: https://qmetrix.com.au/article/workday-adaptive-planning-release-2026-r1-review-march-2026/
5. CPA Practice Advisor — *Workday rolls out group of new AI agents, debuts Flex Credits* (Sept 2025): https://www.cpapracticeadvisor.com/2025/09/22/workday-rolls-out-group-of-new-ai-agents-debuts-flex-credits/169401/
6. Fusion5 NZ — Workday Adaptive Planning: https://www.fusion5.co.nz/corporate-performance-management/workday-adaptive-planning/
7. Workday — *Elevate New Zealand*: https://www.workday.com/en-au/elevate-new-zealand.html
