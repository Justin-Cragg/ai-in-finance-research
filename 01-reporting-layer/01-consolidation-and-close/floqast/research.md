# FloQast

*Layer: Reporting → **Consolidation & close** (close management, reconciliations, journal entries, flux analysis, SOX/internal audit) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | FloQast (private, US) — passed **US$200m ARR** (Jan 2026); 3,500+ accounting teams globally [3] |
| **Products in scope** | Close Management, Reconciliations, Journal Entry Management, Flux/Variance Analysis, Compliance (SOX), Internal/Operational Audit; **FloQast Transform** (agent builder) |
| **AI brand** | **FloQast AI Agents**, **Transform**, **Detect**, **AI Assistant**, COSO AI Governance module |
| **AI maturity** | **Stage 3 – Embedded agents**, with an unusually strong **auditability** story (agents built from already-audited work, COSO-mapped controls) |
| **NZ relevance** | Expanded into **Australia & New Zealand in March 2023** with a Sydney HQ and ANZ MD [4]. **Native Xero integration** aimed at APAC multi-entity groups and client-accounting (CAS) firms [5], so it's one of the few enterprise-grade close tools that reaches NZ businesses running Xero. Also integrates with NetSuite, SAP, Workday, Microsoft and Sage Intacct [1] |

## Executive summary
- FloQast is built **"by accountants, for accountants"**. It sits on top of the ERP and Excel, and organises the close checklist, reconciliations and review sign-offs. Lighter and faster to deploy than BlackLine, so it fits **mid-market** teams well.
- **Its AI pitch is "auditable agents".** **FloQast Transform** (TakeControl, Sept 2026) can take the files from a close your team has *already finished and had reviewed*, reverse-engineer the workflow, and **build an AI agent that runs that process next month**. The agent comes documented and tested against numbers the team already approved, ready to show the auditor. [1][2]
- **COSO AI Governance module** (Sept 2026): FloQast hired the COSO chair and is building COSO's generative-AI framework into the product. Agent capabilities are mapped to risks and controls, and **audit evidence is captured automatically while the agent runs**. [2]

## How the AI works — plain English

### FloQast AI Agents (Mar 2025 →) [6]
- Started with a **Journal Entry Agent** (drafts recurring JEs) and a **Data Transformation Agent** (cleans and standardises messy data using plain-English instructions). Custom agents followed for reconciliations, tasks, financial insights and compliance.
- Design goal: **"turn preparers into reviewers"**.

### TakeControl 2026 launches (Sept 2026) [1][2]
| Product | What it does | Plain English |
|---|---|---|
| **Transform** | Builds an agent from prior-period close files | "Show it last month's finished rec; it learns the steps and does next month's" |
| **Detect** | Continuous GL anomaly monitoring by account and subsidiary *during* the period | Problems flagged when they're posted, not on workday 3 |
| **AI Assistant (JE review)** | First-pass review of every journal entry, with structural validation and an **audit-risk score** before approval | A second pair of eyes on every journal |
| **Operational Audits** | AI drafts the audit plan, executes tests, generates an exec report | Internal audit for non-SOX areas |
| **COSO AI Governance module** | Maps agents to COSO risks/controls; auto-captures evidence | The control framework for the agents themselves |

### Earlier capabilities (2025)
- **AI Variance Analysis** (detects and explains material flux), **AI Detections** (GL monitoring), **AI Testing** (internal audit). [6]

## Where it lands in the finance process
| Process | AI help | Human still owns |
|---|---|---|
| Close checklist | Agents run recurring steps; Transform automates proven workflows | Close calendar, judgement items |
| Journals | Agent drafts; AI Assistant risk-scores before approval | Approval |
| Flux / variance review | Auto-explanations of material movements | Challenge and commentary |
| Reconciliations | Agent-prepared recs | Review and sign-off |
| SOX / internal audit | AI-drafted plans and testing; COSO-mapped evidence | Control design, conclusions |

## Governance & control considerations
- **Strongest "explain it to the auditor" story in the sub-layer.** Agents are derived from reviewed work and tested against approved numbers, and evidence is captured as they run. [1][2]
- FloQast's own survey stats are worth quoting: **88%** of organisations have deployed AI in at least one function but only **38%** have AI governance policies, and **30%** of GenAI projects are abandoned after pilot. [1]
- NZ caveat: ANZ team is Sydney-based; check local implementation partner capacity and data hosting region.

## Presentation talking points
- **"Your last close is the training data."** Transform is the clearest example of AI learning from a team's own approved work rather than generic rules.
- Good for the **vCFO deck too**: the Xero integration and multi-client support mean CAS firms can run a FloQast-style close across a client portfolio. [5]
- Contrast: BlackLine = enterprise scale and matching depth; FloQast = mid-market, accountant-friendly, audit-first AI.

## Sources
1. FloQast — *TakeControl 2026 Recap: AI accounting announcements*: https://www.floqast.com/blog/takecontrol-2026-recap
2. GlobeNewswire — *FloQast Introduces New AI Accounting Innovations at TakeControl 2026 and Names COSO Chair Lucia Wind as SVP of Risk & Audit Advisory* (16 Sept 2026): https://www.globenewswire.com/news-release/2026/09/16/3363412/0/en/floqast-introduces-new-ai-accounting-innovations-at-takecontrol-2026-and-names-coso-chair-lucia-wind-as-svp-of-risk-audit-advisory.html
3. FloQast — *FloQast Hits $200 Million ARR Milestone* (20 Jan 2026): https://www.floqast.com/press-releases/floqast-hits-200-million-arr
4. FloQast — *FloQast Global Momentum Continues with Expansion into Australia, New Zealand* (Mar 2023): https://www.floqast.com/press-releases/floqast-global-momentum-continues-with-expansion-into-australia-new-zealand
5. FloQast blog — *Enhancing Accounting Processes with FloQast and Xero* (17 Feb 2025): https://www.floqast.com/blog/enhancing-accounting-processes-with-floqast-and-xero
6. CPA Practice Advisor — *FloQast Launches Auditable AI Agents* (25 Mar 2025): https://www.cpapracticeadvisor.com/2025/03/25/floqast-launches-auditable-ai-agents/157868/
