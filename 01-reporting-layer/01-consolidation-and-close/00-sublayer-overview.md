# Reporting Layer → Consolidation & Close — NZ Market Leaders & AI Overview

*Last researched: 5 Oct 2026 · Audience: CFO / FC · Parent: [Reporting layer overview](../00-layer-overview.md)*

## What this sub-layer is
Everything between "the ledger is posted" and "the group numbers are locked": **close task management, account reconciliations, transaction and intercompany matching, journal review, flux analysis, currency translation, eliminations and group consolidation**.

Two kinds of tool live here, and NZ groups often run one of each:
- **Consolidation engines** — produce the group numbers (Oracle FCCS/HFM, OneStream, CCH Tagetik).
- **Close & reconciliation overlays** — control the work *before* consolidation (BlackLine, FloQast, Oracle ARCS).

> **Scope change from round 1:** the "Close, reconciliation & matching" sub-segment previously parked in the Integrating SaaS placeholder now lives here. BlackLine, FloQast and Trintech are close tools, not bolt-on transaction SaaS.

## Top 5 in the NZ market (enterprise / upper mid-market)

| # | Supplier / product | Type | Why it's top 5 in NZ | AI maturity* | Headline AI |
|---|---|---|---|---|---|
| 1 | **[Oracle EPM](oracle-epm/research.md)** (HFM → FCCS, ARCS) | Consolidation + recs | Largest legacy HFM base among NZ corporates and public sector; HFM support to 2030 drives migrations | Stage 3 | Consolidation Journals/Process assistants, ARCS matching assistants, IPM Insights outliers in close |
| 2 | **[OneStream](onestream/research.md)** | Unified consolidation + planning | Main HFM-replacement competitor; Gartner Leader (4×, furthest in vision 2026) | Stage 4 | SensibleAI Agents + MCP Finance Agentic Layer |
| 3 | **[BlackLine](blackline/research.md)** | Close & recs overlay | Best-known reconciliation platform in NZ enterprise; NZ country manager since 2019; Sydney data centre | Stage 3 | **Verity Prepare** multi-agent recs (GA Jul 2026, up to 92% less prep time); Vera AI team lead |
| 4 | **[FloQast](floqast/research.md)** | Close & recs overlay (mid-market) | ANZ expansion 2023 (Sydney HQ); **Xero integration** reaches NZ mid-market and CAS firms | Stage 3 | **Transform** builds agents from last month's audited close; COSO AI governance module |
| 5 | **[CCH Tagetik](cch-tagetik/research.md)** | Consolidation suite | Gartner Leader (3×), global top-3 consolidation engine; **small NZ base** (APAC "developing") | Stage 3 | Expert AI: intercompany matching agents, data-lineage agents, Planning Sentinel |

\*Maturity stages defined in the root README.

### How the top 5 were chosen
No published NZ market-share data exists for close or consolidation software. Ranking is a judgement based on: (a) **2026 Gartner MQ for Financial Close & Consolidation** (Leaders: Oracle, OneStream, CCH Tagetik; HighRadius named Challenger) [1][2][3]; (b) visible NZ presence (local staff, partners, events, data hosting); (c) relevance to Deloitte NZ clients. Positions 4–5 are lower-confidence: FloQast has the stronger NZ reach, Tagetik the stronger analyst position. **Validate with Deloitte NZ's EPM / finance transformation practice.**

### Considered but not in the top 5
| Product | Why not top 5 (NZ) | AI note |
|---|---|---|
| **Trintech** (Cadency enterprise / Adra mid-market) | Credible BlackLine alternative; customers concentrated in France, Australia, US [4]; no visible NZ presence found | Sept 2026: Data Access, Accruals Intelligence and Exception Management agents; earlier Flux and Variance Analysis agents [5] |
| **SAP S/4HANA Group Reporting & Advanced Financial Closing** | Relevant for SAP-centric NZ groups; part of the ERP | See [ERP layer → SAP](../../02-erp-layer/sap/research.md) (Joule agents, accruals agent) |
| **Workday Financials close** | Only for Workday Financials customers (rare in NZ) | Financial Close Agent; see [Workday Adaptive](../02-fpa-and-management-reporting/workday-adaptive-planning/research.md) |
| **Microsoft Dynamics 365 / Business Central consolidation** | Native ERP consolidation for many NZ mid-market groups | See [ERP layer → D365](../../02-erp-layer/microsoft-dynamics-365/research.md) |
| **HighRadius** | Gartner Challenger 2026; strength in O2C/treasury; limited NZ | AI-led close and reconciliation automation (not researched in depth) |
| **Prophix One** | Mid-market planning + consolidation | Consolidation Agent; see [FP&A → Prophix](../02-fpa-and-management-reporting/prophix/research.md) |
| **Numeric** | AI-native US close start-up; not in NZ | AI-native flux and close automation (not researched in depth) |
| **SME consolidation** (Fathom, Spotlight Multi, Calxa, Xero/Syft) | How most NZ SME groups actually consolidate | See [SME / vCFO tier](../02-fpa-and-management-reporting/00-sublayer-overview.md#sme--vcfo-tier) |

## What AI is doing in close & consolidation (themes)
1. **The reconciliation is the first unit of work AI is taking over.** BlackLine Verity Prepare, Oracle ARCS assistants, FloQast agents and Trintech's exception agent all target rec preparation: high volume, rule-bound, well evidenced.
2. **Preparer → reviewer.** Every vendor frames the human role as reviewing and signing off agent-prepared work. Control documentation (who is the preparer?) needs to catch up.
3. **Agents built from your own audited history.** FloQast Transform builds agents from prior closes; BlackLine Verity Match learns from historical matches; Trintech's accruals agent learns from past estimates. The firm's past close is now training data.
4. **Governance of the agents is becoming a product.** FloQast's COSO AI module, BlackLine's "glass box" with confidence scores, and Tagetik's data-lineage agents all aim to satisfy the external auditor, not just the FC.
5. **Consolidation engines differentiate on AI and openness.** All three Gartner Leaders ship agentic AI. OneStream is furthest on openness (MCP), Oracle on breadth, Tagetik on regulatory and ESG depth.
6. **Continuous close is getting real.** FloQast Detect and Oracle IPM Insights flag anomalies *during* the period, not on workday 3.

## Deck use
- **AI in financial reporting deck:** headline stat (BlackLine: up to 92% less rec prep time); "preparer → reviewer" control slide; HFM migration = AI business case (Oracle/OneStream).
- **vCFO deck:** FloQast + Xero for CAS firms running close across a client portfolio; SME consolidation sits in the FP&A sub-layer's SME tier.

## Tool folders
- [oracle-epm/research.md](oracle-epm/research.md)
- [onestream/research.md](onestream/research.md)
- [blackline/research.md](blackline/research.md)
- [floqast/research.md](floqast/research.md)
- [cch-tagetik/research.md](cch-tagetik/research.md)

## Sources
1. Wolters Kluwer — *CCH Tagetik 3x Leader in 2026 Gartner MQ for Financial Close and Consolidation*: https://www.wolterskluwer.com/en/news/pr-2026-cch-tagetik-leader-in-gartner-magic-quadrant-for-financial-close-consolidation-solutions
2. PR Newswire — *OneStream Named a 4x Leader and Placed Furthest in Vision in the 2026 Gartner MQ for FCC* (MQ published 9 Mar 2026): https://www.prnewswire.com/news-releases/onestream-named-a-4x-leader-and-placed-furthest-in-vision-in-the-2026-gartner-magic-quadrant-for-financial-close-and-consolidation-solutions-302710058.html ; Oracle — *Gartner MQ for FCC*: https://www.oracle.com/performance-management/gartner-financial-close-magic-quadrant/
3. HighRadius — *Named a Challenger in the 2026 Gartner MQ for FCC*: https://www.highradius.com/resources/Blog/highradius-named-a-challenger-in-the-2026-gartner-magic-quadrant-for-financial-close-and-consolidation-solutions/
4. Apps Run The World — *Trintech Cadency Close Management customers*: https://www.appsruntheworld.com/customers-database/products/view/trintech-cadency-close-management
5. Trintech — *Trintech Launches Three New AI Agents to Advance Governed Autonomous Finance* (28 Sept 2026): https://www.trintech.com/news/trintech-launches-three-new-ai-agents-to-advance-governed-autonomous-finance/
6. Tool-level sources are in each tool folder.
