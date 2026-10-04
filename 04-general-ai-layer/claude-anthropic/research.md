# Claude (Anthropic)

*Layer: General AI · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Anthropic |
| **Products** | Claude (Pro/Max/Team/Enterprise), **Claude Cowork**, Claude Code, **Claude for Excel / PowerPoint / Word** add-ins, **Claude for Financial Services**, Claude Managed Agents, Claude in Microsoft 365 Copilot |
| **AI maturity** | **Stage 4** – finance agent templates, Office add-ins, MCP connectors (the protocol Anthropic created, now used by OneStream, Workiva, NetSuite, BC, Snowflake etc.) |
| **NZ relevance** | Powers **Xero's JAX** and is accessible on Xero data (Mar 2026 partnership) [3]; **Claude runs in-region in Auckland via AWS Bedrock** with an AU/NZ routing option — the clearest in-country GenAI option for NZ [4] |

## Executive summary
- **May 2026: 10 finance agent templates**, including two directly relevant to corporate finance — **General Ledger Reconciler** and **Month-End Closer** (runs the close checklist, prepares journals, produces reports) — plus **Statement Auditor**, Valuation Reviewer and research agents. Delivered as **Cowork/Claude Code plugins** and via Excel, PowerPoint and Word add-ins (GA). [1]
- **Claude for Excel** tracks and explains every change with links to the cells it touched — designed for reviewability. [2]
- **Model Context Protocol (MCP)** — Anthropic's open standard — is now how ERP and reporting vendors expose governed data to *any* AI assistant (see Reporting and ERP layers).

## How the AI works — plain English
| Capability | What it does |
|---|---|
| **Finance agent templates** [1] | Pre-built workflows: Pitch Builder, Meeting Preparer, Earnings Reviewer, Model Builder, Market Researcher, Valuation Reviewer, **GL Reconciler**, **Month-End Closer**, **Statement Auditor**, KYC Screener |
| **Agent Skills** [2] | Packaged finance methods — DCF with sensitivities, comparable companies, due-diligence data processing, earnings analysis |
| **Office add-ins** [1][2] | Excel (build/modify models with traceable changes), PowerPoint, Word GA; Outlook coming |
| **Claude Cowork** | Desktop agent that works across files and connected apps for multi-step tasks (Microsoft's Copilot Cowork was built in partnership with Anthropic [5]) |
| **Connectors / MCP** [1][2] | Data providers (LSEG, Moody's, D&B, IBISWorld, etc.) and business systems (Xero, NetSuite AI Connector, OneStream, Workiva, Snowflake…) |
| **Custom skills** | Organisations can encode their own processes (e.g. AP posting, vendor bill workflows against an ERP API) as reusable skills |

## Governance considerations
- Business data shared via Xero integration is used only for the session, not for training. [3]
- **NZ residency**: consumer/enterprise Claude apps process outside NZ; **Claude on AWS Bedrock in Auckland** offers in-region inference. [4]
- Agents act with the permissions of connected-system credentials — role design in the ERP is the control.

## Presentation talking points
- **Month-End Closer / GL Reconciler** show a general-purpose AI moving into the controller's core job — a strong vCFO slide.
- Live demo potential: Claude + NetSuite/Xero via MCP (e.g. reconciling, drafting a vendor bill for approval).
- Anthropic → Xero → NZ: a neat local narrative.

## Sources
1. Anthropic — *Agents for financial services* (5 May 2026): https://www.anthropic.com/news/finance-agents
2. Anthropic — *Advancing Claude for Financial Services* (27 Oct 2025): https://www.anthropic.com/news/advancing-claude-for-financial-services
3. Business Wire — *Xero and Anthropic collaborate…* (26 Mar 2026): https://www.businesswire.com/news/home/20260326956055/en/Xero-and-Anthropic-Collaborate-to-Bring-AI-Powered-Financial-Intelligence-to-Millions-of-Small-Businesses
4. AWS — *Amazon Bedrock in Asia Pacific (New Zealand)* (26 Mar 2026): https://aws.amazon.com/blogs/machine-learning/run-generative-ai-inference-with-amazon-bedrock-in-asia-pacific-new-zealand/
5. Microsoft — *Copilot Cowork built with Anthropic; Claude in Copilot* (Mar 2026): https://www.microsoft.com/en-us/copilot/blog/2026/03/09/powering-frontier-transformation-with-copilot-and-agents/
