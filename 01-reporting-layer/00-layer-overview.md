# Reporting Layer — Market Leaders in NZ & AI Overview

*Last researched: 5 Oct 2026 (round 2: split into three sub-layers) · Audience: CFO / FC*

## What this layer is
The systems that take ledger data and turn it into **consolidated, controlled, decision-ready numbers and narrative**. Round 1 treated this as one layer. Round 2 splits it into the **three jobs** the original list ("HFM, Workiva, Workday, Planful") was mixing:

| Sub-layer | The job | Key question for a CFO | Folder |
|---|---|---|---|
| **1. Consolidation & close** | Close tasks, reconciliations, matching, journals, intercompany, group consolidation | "Are the numbers right, and can we prove it?" | [01-consolidation-and-close/](01-consolidation-and-close/00-sublayer-overview.md) |
| **2. FP&A & management reporting** | Budgets, forecasts, scenarios, KPI dashboards, monthly management and board packs. **Includes the SME / vCFO tier** | "What do the numbers mean, and what happens next?" | [02-fpa-and-management-reporting/](02-fpa-and-management-reporting/00-sublayer-overview.md) |
| **3. External reporting** | Statutory financial statements, annual reports, disclosure checklists, climate statements, XBRL | "Is what we publish complete, consistent and compliant?" | [03-external-reporting/](03-external-reporting/00-sublayer-overview.md) |

```
 ledger (ERP) ──► 1. CONSOLIDATION & CLOSE ──► 2. FP&A & MANAGEMENT REPORTING ──► internal decisions / board
                    recs · matching · journals      plans · forecasts · mgmt packs
                    intercompany · consolidation    (SME tier: Fathom · Spotlight · Xero/Syft)
                              │
                              └────────────────► 3. EXTERNAL REPORTING ──► statutory FS · annual report · climate statement
                                                   tie-out · disclosure checklist · narrative
```

## Top 5 by sub-layer (summary)

| Sub-layer | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| **Consolidation & close** | Oracle EPM (HFM→FCCS, ARCS) | OneStream | BlackLine | FloQast | CCH Tagetik |
| **FP&A & mgmt reporting** (enterprise / mid) | Workday Adaptive Planning | Anaplan | Jedox | IBM Planning Analytics | Prophix |
| **FP&A & mgmt reporting** (SME / vCFO tier) | Fathom | Spotlight Reporting (NZ) | Syft → Xero Analytics | *(Calxa considered)* | — |
| **External reporting** | Workiva | Caseware | Oracle Narrative Reporting* | Word/Excel + M365 Copilot* | Sustainability data platforms (Toitū, IBM Envizi) |

\*Researched elsewhere in the repo: Oracle under Consolidation & close; Copilot under the General AI layer. Multi-job suites (Oracle EPM, OneStream) have one home folder in Consolidation & close and are cross-referenced from the other sub-layers.

**Rankings are informed judgement**; no published NZ market-share data exists for any of these categories. See each sub-layer overview for the method and the "considered" list. **Validate with Deloitte NZ's EPM, Audit & Assurance and Sustainability practices before presenting.**

## AI maturity by sub-layer

| Sub-layer | Typical maturity | Most advanced example | Where AI is landing first |
|---|---|---|---|
| Consolidation & close | **Stage 3**, with OneStream at 4 | OneStream (MCP Finance Agentic Layer); BlackLine Verity Prepare multi-agent recs | **Reconciliation preparation** (up to 92% less prep time, BlackLine) |
| FP&A & mgmt reporting | **Stage 3→4** enterprise; **Stage 2** SME | Jedox / IBM / Prophix / Workday all with MCP; Anaplan "LLM talks, engine calculates" | **Explaining variances** and **drafting commentary** |
| External reporting | **Stage 3** (Workiva) but **Stage 2 in practice for most NZ entities** | Workiva Tie-Out / Knowledge; Caseware Disclosure Checklist Agent (US) | **Checking**: tie-out, disclosure checklists, XBRL validation |

Maturity stages are defined in the root README.

## Cross-cutting themes for the decks
1. **Predict → Explain → Act, at different speeds per sub-layer.** FP&A has been "predicting" for a decade and is now "acting" (scenario agents, commit-to-plan). Close jumped straight to agents that *prepare* work. External reporting is still mainly "checking", for good reason: published documents carry legal liability.
2. **Preparer → reviewer everywhere.** BlackLine, FloQast, Oracle ARCS, Caseware and Workiva all frame the human as reviewer and signer of agent-prepared work. Internal-control documentation and audit evidence need to catch up. Who is the "preparer" when an agent prepared it?
3. **System of record + any AI front door (MCP).** OneStream, Workiva, Workday, Jedox, IBM Planning Analytics (incl. on-prem TM1) and Prophix all expose governed data via MCP. **New in round 2:** this is no longer an enterprise-only pattern. Mid-market planning tools have it too, often as a **separately licensed add-on**.
4. **"LLM talks, engine calculates."** Trustworthy finance AI keeps arithmetic in deterministic engines (Anaplan explicit; IBM "grounded in TM1 logic"; Prophix "deterministic, explainable"). Fathom's **symbolic attribution** brings the same idea to SME packs.
5. **Your own history becomes the training data.** FloQast Transform builds agents from last month's audited close; Workiva Knowledge drafts from your prior filings and memos; BlackLine Verity Match learns from past matches. Finance's own records are now AI assets.
6. **Governance of the agents is becoming a product feature.** FloQast's COSO AI module, BlackLine's confidence scores and "glass box", Tagetik's data-lineage agents and Workiva's tick-marks are all aimed at the **external auditor**, not just the FC.
7. **AI is (mostly) a cloud dividend, with one exception.** On-prem HFM gets nothing (support to Dec 2030). But IBM has extended MCP tools to on-prem TM1, so "migrate to get AI" is not universal.
8. **Commentary is commoditised.** From Fathom and Spotlight to Oracle Narrative Reporting, drafted variance commentary is now standard. Differentiation is moving to **context** (business context set once), **traceability** and **advice/actions**.
9. **Commercial models are shifting to consumption and add-ons.** Workday Flex Credits, BlackLine platform pricing, Jedox MCP add-on, IBM Planning Analytics Agent add-on, Workiva advanced tiers. AI needs its own budget line.
10. **NZ availability lags.** Caseware's agent is US-only, Workiva benchmarking leans on SEC filings, and AI data is typically processed in Australia (BlackLine, Caseware, IBM Sydney). **Check NZ availability, NZ-standard content and data region before client use.**

## Deck mapping
| Deck | Sub-layers | Lead examples |
|---|---|---|
| **AI in financial reporting** | All three | Close: BlackLine Verity Prepare, Oracle/OneStream (HFM migration). FP&A: Workday Adaptive, IBM TM1 MCP. External: Workiva Tie-Out, Caseware disclosure checklist |
| **AI in virtual CFO services** | FP&A (SME tier), Consolidation & close (FloQast + Xero), External (Caseware) | Fathom Commentary Writer, Spotlight AI Action Plans, Xero/Syft, FloQast for CAS firms |

## Changes from round 1
- Split into three sub-layer folders; existing tool research moved (Oracle EPM, OneStream → close; Workday Adaptive, Anaplan → FP&A; Workiva → external).
- **New tool research (9 docs):** BlackLine, FloQast, CCH Tagetik, Jedox, IBM Planning Analytics, Prophix, Fathom, Spotlight Reporting, Caseware. The external-reporting landscape (Toitū, Envizi, Certent) is covered in that sub-layer's overview.
- "Close, reconciliation & matching" moved here from the Integrating SaaS placeholder.
- SME / vCFO tier (round 2 item (a) in the root README) is now researched within FP&A & management reporting.

## Sources
Each sub-layer overview and tool folder carries its own numbered sources. Key analyst references:
1. OneStream — *4x Leader, furthest in vision, 2026 Gartner MQ for Financial Close & Consolidation*: https://www.prnewswire.com/news-releases/onestream-named-a-4x-leader-and-placed-furthest-in-vision-in-the-2026-gartner-magic-quadrant-for-financial-close-and-consolidation-solutions-302710058.html
2. Wolters Kluwer — *CCH Tagetik 3x Leader, 2026 Gartner MQ for FCC*: https://www.wolterskluwer.com/en/news/pr-2026-cch-tagetik-leader-in-gartner-magic-quadrant-for-financial-close-consolidation-solutions
3. Apps Run The World — *Top 10 EPM Software Vendors*: https://www.appsruntheworld.com/top-10-epm-software-vendors-and-market-forecast/
