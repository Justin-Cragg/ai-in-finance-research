# ERP Layer — Market Leaders in NZ & AI Overview

*Last researched: 5 Oct 2026 · Audience: CFO / FC*

## What this layer is
The **system of record** for transactions: general ledger, AP, AR, cash, fixed assets, inventory/procurement. AI here acts directly on transactions — capturing, matching, coding, accruing, reconciling — so it carries the highest control significance of any layer.

> **Challenges on the original framing**
> 1. **Microsoft Dynamics 365 was missing** — Business Central has the largest mid-market ERP footprint in NZ and F&O is a leading enterprise ERP. It's in the top 5.
> 2. **Xero is accounting software, not an ERP** (no manufacturing/advanced inventory). It belongs in this layer for the decks — it's the ledger for most vCFO clients — but label the layer **"ERP & accounting systems"**.
> 3. **Treat Oracle as one supplier with two products** — NetSuite (upper-mid-market) and Fusion (enterprise). Their AI stories differ.
> 4. **TechnologyOne** dominates NZ local government, education and the public sector — worth a mention if the audience includes public sector CFOs.

## Top 5 suppliers in the NZ market

| # | Supplier | NZ segment | Why top 5 | AI maturity* | Headline AI | How AI is priced |
|---|---|---|---|---|---|---|
| 1 | **Xero** | SME / vCFO | NZ-founded; dominant SME ledger; 5m subscribers globally | Stage 3→4 | JAX agents (auto bank rec, doc capture, month-end agent via XeroForce); Claude-powered; Xero data in Claude/ChatGPT/M365 Copilot | Bundled tiers (Xero Ultra for growing businesses) |
| 2 | **MYOB** | SME → mid-market (Acumatica) | #2 SME brand; MYOB Acumatica a leading NZ mid-market ERP | Stage 2→3 | Drafts-first Acumatica AI (AP bill entry, anomaly detection, read-only AI assistant); Microsoft partnership features due late 2026 | MYOB-managed model included (Acumatica 2026.1) |
| 3 | **Microsoft Dynamics 365** | Mid-market (BC/Wiise) → enterprise (F&O) | Largest NZ mid-market footprint | Stage 3→4 | BC Payables & Sales Order agents, Agent Designer, built-in MCP; F&O Account Reconciliation Agent; finance agents in Excel/Outlook | **Copilot Credits** (consumption) |
| 4 | **SAP** | Large enterprise | Largest NZ corporates; ECC → S/4HANA 2027 deadline | Stage 3 | Joule; Dispute Resolution agent; Accruals agent (restricted, GA Q1 2027); AI-assisted error/asset explanations | Base bundled; premium = **AI Units** |
| 5 | **Oracle** (NetSuite + Fusion) | Upper mid (NetSuite) / enterprise (Fusion) | NetSuite growing as Xero "graduation" path; Fusion in large enterprise/public sector | Stage 3→4 | Fusion: Payables/Ledger/Planning/Payments agents + 22 agentic apps (e.g. Collectors Workspace). NetSuite: MCP AI Connector, Ask Oracle, AI Canvas | **Included** at no extra cost (Fusion); NetSuite contract-specific |

\*Maturity stages defined in the root README.

### How the top 5 were chosen
No vendor publishes audited NZ customer counts. Ranking reflects partner-channel depth and observable market activity [1], vendor scale, and relevance across Deloitte's two audiences (enterprise reporting and vCFO/SME). **Considered:** TechnologyOne (public sector), SAP Business One, Acumatica direct, SYSPRO, Infor, Wiise (counted under Microsoft).

## Cross-cutting themes for the decks
1. **From "copilot" to "agent".** 2025 was assistants that answer; 2026 is agents that draft invoices, propose accruals and reconcile — with humans approving. Oracle's "agentic applications" go further: whole processes run continuously.
2. **Drafts-first is the norm.** Every vendor's finance agents propose and a human posts (MYOB explicitly; SAP accruals; D365 reconciliation; Xero action summaries). This is the control design to emphasise.
3. **Your policy manual becomes the program.** SAP's accruals agent reads a plain-language policy PDF; Xero/BC agent builders take natural-language instructions. Quality of documented policy = quality of automation.
4. **The ERP is opening to any AI front-end via MCP** — NetSuite AI Connector, Business Central MCP server, Xero in Claude/ChatGPT/Copilot. Permissions follow the ERP role; role design becomes an AI control.
5. **AI pricing is diverging** — included (Oracle) vs consumption credits (Microsoft, SAP, Workday). CFOs need to budget AI as variable opex.
6. **Cloud migration is the gate.** Best AI is in SAP S/4HANA Cloud, Oracle Fusion (26A+), D365 cloud — on-prem/legacy (ECC, EBS) gets little.
7. **SME/vCFO:** Xero and MYOB's agents automate bookkeeping and month-end, shifting the vCFO model from processing to **supervising agents across a client portfolio** and selling advisory (cash forecasting, scenarios, benchmarks).

## Tool folders
- `xero/research.md`
- `myob/research.md`
- `microsoft-dynamics-365/research.md`
- `sap/research.md`
- `oracle-netsuite-and-fusion/research.md`

## Sources
1. Equerra — *Best ERP Software NZ 2026* (segment leadership; "no vendor publishes definitive NZ customer counts"): https://equerra.com/resources/best-erp-software-nz-2026
2. iStart NZ — *ERP Buyer's Guide*: https://istart.co.nz/nz-buyers-guide-items/erp-buyers-guide/
3. OpsUI — *ERP NZ (2026) buyer's guide*: https://opsui.co.nz/blog/erp-nz-guide/
4. Tool-level sources are listed in each tool's research.md.
