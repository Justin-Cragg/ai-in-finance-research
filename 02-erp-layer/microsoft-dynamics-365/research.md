# Microsoft Dynamics 365 (Business Central & Finance)

*Layer: ERP (mid-market → enterprise) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Microsoft |
| **Products** | **Dynamics 365 Business Central** (mid-market; also sold in NZ as **Wiise**, a localised BC); **Dynamics 365 Finance** (+ Supply Chain, "F&O") for enterprise |
| **AI brand** | **Copilot** (embedded assistance) + **agents** (Payables, Sales Order, Expense, Account Reconciliation, Finance agent in M365) + **Agent Designer**; governed by Copilot Studio / Agent 365 |
| **AI maturity** | **Stage 3→4** – GA agents in BC; MCP server built into BC; deep link to Microsoft 365 Copilot/Excel |
| **NZ relevance** | **Largest mid-market ERP footprint in NZ** (Business Central) and a leading enterprise ERP (F&O) alongside TechnologyOne in public sector [5] — likely the user's missing ERP |

## Executive summary
- **Business Central has GA agents (May 2026):** a **Payables Agent** that reads vendor-invoice emails and drafts purchase invoices, a **Sales Order Agent**, and **Agent Designer** for building custom agents in plain English. An **MCP server** is now built in (cannot be disabled), letting external AI tools call BC under normal user permissions. [2]
- **Dynamics 365 Finance:** an **Account Reconciliation Agent** (production-ready preview) continuously matches subledger to GL and proposes fixes. [3][4]
- **The Microsoft 365 angle is unique:** finance agents work *inside Excel and Outlook* (Financial Reconciliation agent, Finance agent), which is where FCs actually work. [4]
- **Cost model changes:** agents consume **Copilot Credits** — variable, volume-driven costs that peak at month/quarter-end. [1]

## How the AI works — plain English

### Business Central [2]
| Agent / feature | How it works | Status |
|---|---|---|
| **Payables Agent** | Watches a mailbox → OCR/entity extraction (Azure Document Intelligence) → matches vendor & GL accounts → confidence-scores → drafts a purchase invoice for a supervisor | GA, all regions (English). *No PO matching/approvals/anomaly detection yet* |
| **Sales Order Agent** | Reads customer emails, asks clarifying questions, checks capable-to-promise, drafts quote for approval | GA |
| **Expense Agent** | Receipt capture, categorisation, mileage/per diem via web, Outlook or Copilot Chat — for staff without BC licences | Preview (US first) |
| **Agent Designer** | Describe a custom agent in natural language; inherits BC permissions and audit logging | Prototype GA; production from v28.1 |
| **MCP server** | External AI clients (Copilot, Claude, ChatGPT etc.) call BC using the same permission model as humans | Mandatory from v28.0 |
| Core Copilot (bank rec suggestions, marketing text, chat) | Embedded assistance | Included in Essentials/Premium licences [1] |

### Dynamics 365 Finance [3][4]
- **Account Reconciliation Agent** — runs continuously to detect subledger↔GL discrepancies, recommends a disposition (journal, reverse, link), finance accepts/rejects, full activity log and undo. As at Jul 2026 it handles two exception types (voucher amount mismatch; pending accounting not transferred). Requires v10.0.44+, Microsoft-assisted activation.
- **Finance agent (Microsoft 365 Copilot)** — reconciliation, variance analysis and data prep in Excel/Outlook using live Finance data.
- **Financial Reconciliation agent (Excel)** — prepares and cleanses datasets for period-end reconciliations.

## Where it lands in the finance process
| Process | AI help |
|---|---|
| AP | Payables Agent drafts invoices from email |
| Close & reconciliations | Account Reconciliation Agent (F&O); Excel reconciliation agent |
| Variance analysis | Finance agent in Excel/Outlook |
| Custom workflows | Agent Designer / Copilot Studio |

## Governance & cost considerations
- Agents draft, humans approve; permissions and audit logs inherit from the ERP. [2][3]
- **Copilot Credits are consumption-based** — pilot on real volumes, set Azure budget alerts, assign an owner for credit monitoring. [1]
- Sources disagree on whether some agents are included in Premium licences vs metered — **confirm with Microsoft licensing** before quoting. [1][4]
- Commentators flag that agent audit trails lag agent capability — a point for internal audit. [6]

## Presentation talking points
- For most NZ mid-market clients, **"your ERP's AI" = Microsoft's AI** — and it reaches into Excel and Teams.
- The **consumption-cost** point is a practical CFO takeaway: AI turns ERP from fixed licence to variable cost.

## Sources
1. MSDynamicsWorld — *Business Central's AI agents run on consumption billing*: https://msdynamicsworld.com/blog-post/business-centrals-ai-agents-run-consumption-billing-heres-what-means-your-2027-budget
2. Tigunia — *Complete Guide to Business Central AI Agents (Wave 1 2026)*: https://tigunia.com/blog/complete-guide-to-business-central-ai-agents/
3. Logan Consulting — *Dynamics 365 Account Reconciliation Agent*: https://www.loganconsulting.com/blog/dynamics-365-account-reconciliation-agent/
4. DrDynamics — *Every Microsoft first-party AI agent in Dynamics 365*: https://www.drdynamics.co.uk/blog/every-microsoft-first-party-ai-agent-in-dynamics-365
5. Equerra — *Best ERP Software NZ 2026*: https://equerra.com/resources/best-erp-software-nz-2026
6. RouteGet — *Dynamics 365's new finance agents are outrunning the audit trail*: https://routeget.com/technology-consulting/dynamics-365s-new-finance-agents-are-outrunning-the-audit-trail-built-to-explain-them/
7. Microsoft Learn — *Business Central 2026 release wave 1 planned features*: https://learn.microsoft.com/en-us/dynamics365/release-plan/2026wave1/smb/dynamics365-business-central/planned-features
