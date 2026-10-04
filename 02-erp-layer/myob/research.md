# MYOB (MYOB Business & MYOB Acumatica)

*Layer: ERP / accounting (SME → mid-market) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | MYOB (Australian; private, KKR-owned) |
| **Products** | **MYOB Business** (SME accounting); **MYOB Acumatica** (mid-market cloud ERP, ANZ-localised Acumatica) |
| **AI brand / partners** | AI features on **AWS Bedrock** (Acumatica AI Studio/Automation) [3]; **5-year Microsoft partnership** (Apr 2026) using Microsoft Foundry, Copilot Studio and Agent 365 [1] |
| **AI maturity** | **Stage 2→3** – practical embedded AI shipped in Acumatica; SME agents and Microsoft-built features still to come (late 2026) |
| **NZ relevance** | #2 SME accounting brand in NZ behind Xero; MYOB Acumatica is one of the leading NZ mid-market ERPs after Dynamics 365 Business Central [5] |

## Executive summary
- **MYOB Acumatica has eight AI features in production** — AI Assistant (read-only Q&A), AI Automation, AP bill entry, expense receipt scanning, anomaly detection, manufacturing variance detection and more — all **"drafts-first": suggest or flag, never post without human approval.** [2]
- **April 2026: five-year Microsoft partnership** to build cash-flow forecasting and compliance agents for SMEs and natural-language/document AI for mid-market — first joint features expected later in 2026; **none released as at Sept 2026.** [1][2]
- MYOB is behind Xero on agentic AI for SMEs, but the drafts-first design and ANZ data residency are credible control stories.

## How the AI works — plain English

### MYOB Acumatica — shipped features [2][3]
| Feature | How it works |
|---|---|
| **AI Assistant** | Ask plain-English questions about revenue, customers, performance. **Read-only** — cannot change records |
| **AI Automation** (formerly AI Studio, with AWS) | Admins attach custom prompts to any screen (e.g. "summarise this customer's history"); MYOB-managed model, no API key needed on 2026.1 |
| **AP Bill Entry** | Reads supplier invoices and drafts bills for approval |
| **Expense Management** | Mobile receipt photos auto-populate expense claims |
| **Anomaly Detection** | Learns normal patterns across expenses/invoices and flags statistical outliers |
| **Production Variance Anomaly Detection** | Same for manufacturing costs, labour time, efficiency |
| Cross-Sell Assistant / Auto Complete | Sales suggestions; text prediction |

### Roadmap
- **Microsoft partnership** [1]: SME agents for **cash-flow forecasting** and **compliance readiness**; mid-market contextual insights, natural-language query, AI document processing; governance via Agent 365.
- **Global Acumatica features without ANZ dates** [2]: MCP access for Claude/Gemini, case-summary and file-tagging agents.

## Data & governance
- Customer data stored in Australia; processing may occur via Anthropic, AWS and Microsoft infrastructure, which may process but not store or train on data (per MYOB policy). [2] — **NZ clients should confirm this meets their data sovereignty position.**
- Drafts-first design maps cleanly to segregation of duties. [2]
- MYOB's own research: 29% of ANZ SMEs have adopted dedicated AI tooling. [1]

## Presentation talking points
- Contrast the two ANZ SME platforms: **Xero = Anthropic/open agentic; MYOB = Microsoft/AWS, drafts-first.**
- For vCFOs with mixed client bases, AI capability is becoming a factor in which ledger to recommend.

## Sources
1. Microsoft Source Asia — *MYOB and Microsoft sign five-year strategic partnership* (8 Apr 2026): https://news.microsoft.com/source/asia/2026/04/08/myob-and-microsoft-sign-five-year-strategic-partnership/
2. Auboros — *MYOB Acumatica AI Features: What's Real in 2026* (Sept 2026): https://www.auboros.com/blog/ai-erp-australia-8/myob-acumatica-ai-australia
3. MYOB — *MYOB Acumatica launches new AI Studio in collaboration with AWS*: https://www.myob.com/au/press-releases/myob-acumatica-launches-new-ai-studio-in-collaboration-with-aws
4. IT Brief NZ — *MYOB & Microsoft strike AI deal for small businesses*: https://itbrief.co.nz/story/myob-microsoft-strike-ai-deal-for-small-businesses
5. Equerra — *Best ERP Software NZ 2026*: https://equerra.com/resources/best-erp-software-nz-2026
