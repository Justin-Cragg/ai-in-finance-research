# ChatGPT (OpenAI)

*Layer: General AI · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | OpenAI |
| **Products** | ChatGPT (Plus/Pro/Business/Enterprise), **ChatGPT for Excel**, **ChatGPT for Financial Services**, connectors/apps, agent mode |
| **Models** | GPT-5.5 (ChatGPT for Excel GA) [2]; "GPT-6 Astra" cited for ChatGPT for Financial Services (Sept 2026) [1] |
| **AI maturity** | **Stage 4** – agentic tools, Excel add-in, 50+ connectors incl. ERP (e.g. Xero) |
| **NZ relevance** | **Most-used AI tool by NZ individuals**: ~10m messages/day from NZ; >⅓ work-related (6 pts above global average); NZ enterprise clients include Air New Zealand, One NZ, Genesis Energy [3]. No NZ data residency (Australia available for data at rest; inference in US) [4] |

## Executive summary
- ChatGPT is the **"shadow AI" reality** in most NZ finance teams — staff already use it. The decision for CFOs is whether to govern it (Business/Enterprise) or block it.
- **ChatGPT for Excel** (launched Mar 2026, GA May 2026): build and update models, run scenarios, trace formula logic with cell references. Enterprise admins enable it by role. [2]
- **ChatGPT for Financial Services** (Sept 2026): aimed at investment banking/equity research — bundled datasets, 50+ connectors, firm templates, citation trails, audit logging. Less relevant to corporate finance, but signals direction. [1]

## How the AI works — plain English
| Capability | What it does |
|---|---|
| **ChatGPT for Excel** | Sidebar agent: create models from plain-English descriptions, analyse links across sheets, explain formulas step by step [2] |
| **Connectors / apps** | Pull data from business systems (incl. Xero connector announced Aug 2026) and data providers (FactSet, LSEG, Moody's, MSCI…) [2][5] |
| **Agent mode / deep research** | Multi-step tasks: research, analysis, building files |
| **Outputs** | Excel, Word, PowerPoint, charts with preserved citations (FS edition) [1] |
| **Enterprise controls** | SSO/SCIM, RBAC, workspaces as information barriers, encryption, audit logs via Compliance Platform [1] |

## Governance considerations
- **Data residency:** expanded to Australia (and others) for data at rest only; **inference remains in the US; NZ not listed**. [4]
- Excel add-in disabled by default in Enterprise; enable deliberately. [2]
- NZ OpenAI data: top 10% of NZ businesses generate 14× the output per worker of the typical business — **adoption gap is a strategic risk**. [3]

## Presentation talking points
- "Your people are already using it" — NZ usage stats make the governance case. [3]
- Use the Excel add-in to show the end of manual model-building drudgery — while stressing review controls.

## Sources
1. VentureBeat — *OpenAI launches ChatGPT for Financial Services…* (10 Sept 2026): https://venturebeat.com/data/openai-launches-chatgpt-for-financial-services-with-integrated-data-sources-it-pulls-research-cites-it-and-builds-decks-in-minutes
2. OpenAI — *Introducing ChatGPT for Excel and new financial data integrations*: https://openai.com/index/chatgpt-for-excel/
3. 1News — *Kiwis send 10 million ChatGPT messages a day as work use climbs* (4 Sept 2026): https://www.1news.co.nz/2026/09/04/kiwis-send-10-million-chatgpt-messages-a-day-as-work-use-climbs/
4. Computerworld — *OpenAI expands data residency for enterprise customers* (26 Nov 2025): https://www.computerworld.com/article/4096675/openai-expands-data-residency-for-enterprise-customers.html
5. Xero Blog — *Xerocon Denver 2026* (ChatGPT connector): https://blog.xero.com/product-updates/xerocon-denver-2026-agentic-workflows-ai-era/
