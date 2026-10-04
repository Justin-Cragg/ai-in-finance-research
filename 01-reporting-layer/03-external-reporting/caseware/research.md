# Caseware

*Layer: Reporting → **External reporting** (statutory financial statements, disclosure checklists, audit/assurance workpapers) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Caseware International (private, Canada). Owns its former ANZ distributor, **Caseware Australia & New Zealand**, acquired May 2023 [5] |
| **Products in scope** | **Caseware Working Papers** (desktop), **Caseware Cloud / Cloud Financials** (financial statement preparation), audit & assurance apps, IDEA data analytics |
| **AI brand** | **Caseware AiDA** (GenAI assistant, Oct 2024) → **Caseware Verity** (agentic AI platform, May 2026) with **Agentic Suites** |
| **AI maturity** | **Stage 3 – Embedded agents** in the US (Disclosure Checklist Agent GA); **Stage 2 in ANZ** until Verity reaches local products |
| **NZ relevance** | The **workhorse for NZ statutory financial statements**: used by accounting and audit firms, corporates and government-related entities. Ships NZ templates (e.g. Tier 1 and Tier 2 RDR general purpose statements) [6]. ANZ cloud data is **hosted in Australia (AWS NSW)** [7] |

## Executive summary
- In NZ, **most statutory accounts aren't produced in Workiva**. They're produced in Caseware (or in practice tools from Xero/MYOB) by finance teams and their accountants. If the external-reporting deck is meant to resonate beyond NZX top-50 issuers, Caseware is the tool to talk about.
- **AiDA (Oct 2024)** was a reactive GenAI assistant: it answered methodology and standards questions, extracted key terms from documents with source links, and explained anomalies. [1][2]
- **Caseware Verity (launched 20 May 2026, CwX 2026)** is an agentic platform that **plans and executes multi-step work** with citation-backed suggestions and human sign-off. First agentic suite: the **Disclosure Checklist Agent**. It reads the draft financial statements, works through the disclosure checklist, and returns **answers with citations to where in the accounts each disclosure is (or isn't)**. Beta firms saved **~2.7 hours per checklist run**. [2][3]

## How the AI works — plain English

### Caseware Verity agents [2][3][4]
| Agent | What it does | Status |
|---|---|---|
| **Disclosure Checklist Agent** | Reviews draft FS against the disclosure checklist; cites the location of each disclosure and explains its reasoning | **GA, US only** (May 2026) [4] |
| **Document Intelligence Agent** | Extracts information from source documents into workpapers | Closed beta |
| **Risk Suggestion Agent** | Suggests engagement-specific risks using multi-year data | Alpha |

### AiDA (still the assistant layer) [1]
- Context-aware Q&A over engagement files and standards; explains charts and anomalies; surfaces methodology guidance.

### Rollout
- Caseware says Verity will roll out "across the ecosystem over time", varying by product area and deployment, with packaging and pricing to follow. It cites US$100m+ of R&D investment. [3]

## Where it lands in the finance process
| Process | AI help | Human still owns |
|---|---|---|
| Statutory financial statements | (Cloud Financials automates drafting from TB with embedded disclosure logic) | Accounting policy and judgement |
| Disclosure checklist | Agent completes the first pass with citations | Review, conclusions |
| Audit / review engagements | Document extraction, risk suggestions | Professional judgement, opinion |

## Governance & control considerations
- **NZ availability is the key caveat.** The Disclosure Checklist Agent is US-only today, and the NZ checklist (NZ IFRS, PBE standards, tiers) would need local content. Ask Caseware ANZ for the roadmap. [4]
- Data residency: ANZ cloud data is held in Australia. [7]
- **Naming clash:** "Verity" is also BlackLine's AI brand (close and reconciliation). Different companies and products, so take care on slides.

## Presentation talking points
- **The disclosure checklist is the "tie-out" of the mid-market.** Tedious, rule-based and citation-friendly, it's a prime early target for agents, just as Workiva targets tie-out for listed issuers.
- Covers **both decks**: finance teams preparing their own statutory accounts, and accounting firms and vCFO practices preparing them for clients.

## Sources
1. Caseware — *Caseware Unveils AiDA, its AI-Powered Digital Assistant* (Oct 2024): https://www.caseware.com/news/caseware-unveils-aida-launches-new-esg-solution-at-cwx-london
2. Caseware blog — *From AiDA to agentic: how Caseware's AI has evolved* (Caseware Verity): https://www.caseware.com/resources/blog/from-aida-to-agentic-how-casewares-ai-has-evolved
3. Accounting Today — *Caseware rolls out 'Verity' AI platform and agents* (20 May 2026): https://www.accountingtoday.com/news/caseware-rolls-out-verity-ai-platform-and-agents
4. Caseware — *Caseware Verity Disclosure Checklist Agent* (US availability): https://www.caseware.com/products/disclosure-checklist-agent
5. PR Newswire — *Caseware International Acquires Longstanding Distributor in Australia & New Zealand* (3 May 2023): https://www.prnewswire.com/apac/news-releases/caseware-international-acquires-longstanding-distributor-in-australia--new-zealand-301811983.html
6. Caseware — *Sample accounts 2026 – Cloud Financials* (NZ Tier 1 / Tier 2 RDR templates): https://my.caseware.com/s/article/Sample-accounts-2026-Cloud-Financials?language=en_US
7. Caseware ANZ — *Caseware Financials launches in Australia* (Sept 2024; AWS NSW hosting): https://www.caseware.com/au/news/caseware-financials-launches-in-australia/
