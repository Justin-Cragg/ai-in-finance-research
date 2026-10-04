# SAP (S/4HANA Cloud + Joule)

*Layer: ERP (enterprise) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | SAP |
| **Products** | SAP S/4HANA Cloud (Public & Private Edition, typically via **RISE with SAP**); legacy SAP ECC; SAP Business One (SME) |
| **AI brand** | **Joule** (copilot + agents), **Joule Studio** (custom agents), "SAP Business AI" |
| **AI maturity** | **Stage 3** – embedded AI assists GA; finance agents rolling out (several in restricted availability) |
| **NZ relevance** | Installed base among NZ's largest corporates (dairy/primary sector, manufacturing, utilities). **ECC mainstream maintenance ends 31 Dec 2027**, so most NZ SAP clients are mid-migration — AI is now part of that business case [5] |

## Executive summary
- **Joule's AI is cloud-only and best on S/4HANA Cloud Public Edition** — another "migrate to get the AI" story, sharpened by the 2027 ECC deadline. Only ~34% of ECC users have completed migration (SAPinsider benchmark). [5]
- **Finance capabilities today** are mostly *assistive*: explaining errors, fixed-asset depreciation, extracting payment advices, proposing settlement rules, and a **Dispute Resolution Agent** for AR. [1]
- **Accounting Accruals Agent** (announced Sept 2026, restricted availability, GA target Q1 2027) shows the direction: reads your **plain-language accrual policy handbook**, proposes accruals with reasoning, accountant accepts/adjusts/rejects. [2]
- **Watch the commercials:** base AI is bundled; premium agents consume prepaid **AI Units** that expire after 12 months. [2][3]

## How the AI works — plain English

### Embedded AI-assisted features (S/4HANA Cloud, Q1 2026) [1]
| Feature | What it does |
|---|---|
| **Dispute Resolution Agent** | Root-causes invoice disputes by checking invoices, sales orders, deliveries, pricing agreements and tax rules; recommends resolution |
| AI-assisted **payment advice processing** | Extracts amounts, references, currencies from varied remittance formats; self-learning |
| AI-assisted **error explanation** / **e-invoicing error handling** | Turns cryptic system errors into plain-English cause + fix |
| AI-assisted **fixed asset explanations** | Explains how an asset value/depreciation was calculated |
| AI-assisted **settlement rule proposal** | Proposes cost settlement receivers and percentages |
| AI-assisted **sales order creation** | Creates sales orders from PDF/image POs |

### Accounting Accruals Agent — step by step [2]
1. Finance writes a **plain-language PDF policy** (categories, methods, GL accounts, reversal timing).
2. Accountant asks Joule for accrual proposals for a period/company code.
3. Agent reads the policy + history, applies rules.
4. Proposals come with an explanation of which policy and calculation were used.
5. Accountant accepts, adjusts or rejects before posting.

> This "policy document as the program" pattern is a powerful slide: **your accounting manual becomes the agent's instructions.**

### Platform
- **Joule Studio** — build custom agents; **Microsoft 365 Copilot integration** surfaces SAP approvals/workflows in Teams and Outlook. [4]

## Commercials (CFO-relevant) [3]
- **Business AI Base**: bundled into RISE / S/4HANA Cloud (interactive Joule, embedded features).
- **Business AI Premium**: prepaid **AI Units**; agent actions draw down units; unused units expire after 12 months. [2]
- Third-party licensing advisors warn that bundled allowances can be exhausted quickly by scheduled agents and recommend negotiating fixed unit pricing, overage caps and usage reporting rights. *(Advisor estimates, not SAP list prices.)* [3]

## Governance considerations
- Human accept/adjust/reject before posting on accruals. [2]
- Region availability varies; "some capabilities may require an additional subscription". [2]
- NZ Privacy Act 2020 and data sovereignty should be considered separately from Australia in ANZ programmes. [5]

## Presentation talking points
- The ECC 2027 deadline + AI = the strongest "why now" for SAP clients.
- Use the accruals agent to show how agents encode accounting policy — and why policy quality now matters more.

## Sources
1. SAP News — *SAP Business AI: Release Highlights Q1 2026*: https://news.sap.com/2026/04/sap-business-ai-release-highlights-q1-2026/
2. ERP Today — *SAP releases Accounting Accruals Agent for month-end close* (24 Sept 2026): https://erp.today/sap-accounting-accruals-agent-month-end-close
3. Redress Compliance — *SAP Joule Pricing 2026: AI Units and Agent Costs*: https://redresscompliance.com/sap-joule-ai-units-licensing-pillar-2026
4. Savic Technologies — *SAP Joule 40+ AI agents: Q1 2026 releases* (treat status claims with caution — ERP Today is more recent): https://www.savictech.com/insights/sap-joule-agentic-platform-40-agents-2026/
5. SAPinsider — *SAP S/4HANA migration in ANZ: pragmatic paths before 2027*: https://sapinsider.org/sap-s4hana-migration-anz-2027/
6. SAP Discovery Center — *Dispute Resolution Agent (Private Edition)*: https://discovery-center.cloud.sap/ai-feature/bbf06e89-a47a-4a80-a619-97fa7ba6af92/
