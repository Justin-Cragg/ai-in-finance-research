# Perplexity

*Layer: General AI (answer engine / research agent) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Perplexity AI |
| **Products** | Perplexity (Pro/Max), **Enterprise Pro / Enterprise Max**, **Perplexity Computer** (multi-step agent), **Comet** browser (incl. Comet for Enterprise), Perplexity Finance |
| **Models** | Model-agnostic — routes across 20+ third-party and in-house models [1] |
| **AI maturity** | **Stage 3→4** – Computer agent with 400+ connectors; finance data integrations |
| **NZ relevance** | 5th-placed general assistant: popular for research among professionals; smaller enterprise footprint than Microsoft/OpenAI/Anthropic/Google. Included because it's the most-used research-first assistant and is moving into enterprise workflows |

## Executive summary
- Perplexity's strength is **cited research** — every answer links to sources — useful for market, competitor, regulatory and company research in finance.
- **Perplexity Computer (Mar 2026)**: multi-step workflows across research, analysis and document creation; **Microsoft 365 integration** (Word, Excel, PowerPoint, Outlook, Teams, May 2026); **Snowflake** warehouse connector with auto-generated semantic layer for natural-language SQL. [1]
- **Finance Computer (Mar 2026)**: 40+ finance tool calls (SEC filings, earnings transcripts, exchange data); institutional data licences (Morningstar, PitchBook, FactSet) connectable from May 2026; private-company data via Forge Global. [1]

## How the AI works — plain English
| Capability | What it does |
|---|---|
| **Answer engine** | Searches the web/connected sources and synthesises an answer with citations |
| **Perplexity Computer** | Plans and executes multi-step tasks across connectors; produces artifacts [1] |
| **Finance Computer** | Finance-specific tools: filings, transcripts, market data [1] |
| **Comet browser** | AI assistant inside the browser that can act on web pages (forms, research, email drafting) [2] |
| **Enterprise controls** | Admin analytics API, custom roles/RBAC with SCIM (Jul 2026), SOC 2 Type II [1][2] |

## Governance considerations
- Agentic browser (Comet) acting on web apps raises **credential and prompt-injection risks** — policy needed before use on finance systems.
- Finance data integrations are US-market-centric (SEC, US exchanges); NZX coverage should be tested.

## Presentation talking points
- Good illustration of **research agents with citations** — the "show your working" standard finance should demand.
- Contrast: general assistants compete on *where they sit* (Copilot in Office, ChatGPT everywhere, Claude in Xero/Excel, Gemini in Workspace, Perplexity in the browser).

## Sources
1. Releasebot — *Perplexity release notes 2026*: https://releasebot.io/updates/perplexity-ai
2. Perplexity — *Introducing Comet for Enterprise Pro* (14 Aug 2025): https://www.perplexity.ai/hub/blog/the-intelligent-business-introducing-comet-for-enterprise-pro
3. Perplexity changelog — *Computer for Pro subscribers, Computer for Slack* (13 Mar 2026): https://www.perplexity.ai/changelog/what-we-shipped---march-13-2026
4. Perplexity — *Computer for buyside professionals*: https://www.perplexity.ai/hub/workshops/perplexity-computer-for-buyside-professionals
