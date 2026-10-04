# General AI Layer — Market Leaders in NZ & AI Overview

*Last researched: 5 Oct 2026 · Audience: CFO / FC*

## What this layer is
Horizontal AI assistants and agent platforms used across the business — not built for finance, but increasingly the **"front door"** through which finance staff reach ERP, reporting and data systems (via connectors and MCP).

> **Challenges on the original framing**
> 1. **This layer is no longer "general" vs "specialist".** Every general assistant now ships finance-specific agents (Claude Month-End Closer, Copilot Reconciliation/Variance agents, ChatGPT for Excel, Gemini Financial Research Agent).
> 2. **Its real role is the front door.** The ERP/reporting vendors are plugging *into* these tools (OneStream, Workiva, Xero, NetSuite, Business Central all via MCP). The architecture slide should show the general layer sitting **on top of** all other layers, not beside them.
> 3. **Consider a separate "agent orchestration & governance" layer** — Copilot Studio/Agent 365, Snowflake Agent Identity, Databricks AI Gateway, Oracle AI Agent Studio — the control plane for agents across the stack.

## Top 5 in the NZ market

| # | Supplier / product | Why top 5 in NZ | AI maturity* | Finance-relevant headline | NZ data residency |
|---|---|---|---|---|---|
| 1 | **Microsoft 365 Copilot** | Default enterprise AI; NZ orgs overwhelmingly on M365 | Stage 4 | Excel agentic editing; Copilot Cowork; Reconciliation & Variance agents linked to D365/SAP; multi-model (OpenAI + Claude) | ❌ Not on in-country list (Australia is) |
| 2 | **ChatGPT (OpenAI)** | Most-used by NZ individuals: ~10m msgs/day, >⅓ work-related; Air NZ, One NZ, Genesis clients | Stage 4 | ChatGPT for Excel; FS edition; Xero connector | ❌ AU at-rest only; inference US |
| 3 | **Claude (Anthropic)** | Powers Xero JAX; Excel/PowerPoint/Word add-ins; inside M365 Copilot | Stage 4 | **Month-End Closer, GL Reconciler, Statement Auditor** agents; MCP standard | ✅ via AWS Bedrock Auckland (in-region) |
| 4 | **Gemini (Google)** | Workspace organisations; Deloitte a launch partner for FS edition | Stage 3→4 | Gemini in Sheets; Financial Research Agent with confidence scores | ⚠️ Limited for Oceania |
| 5 | **Perplexity** | Leading research-first assistant; moving into enterprise | Stage 3→4 | Cited research; Finance Computer; M365 & Snowflake integrations | ⚠️ Not specified |

\*Maturity stages defined in the root README.

### How the top 5 were chosen
NZ-specific tool share data is scarce. NZ AI adoption is broad but shallow — reported at **91% of businesses, yet only 4% using AI to transform core operations** [1]; typical NZ organisation is "experimenting" (2.4/5 maturity) [2]. Ranking reflects Microsoft 365 prevalence, OpenAI's published NZ usage [3], Anthropic's Xero partnership and NZ in-region availability, Google Workspace share, and Perplexity's research niche. **Considered:** xAI Grok, Meta AI, Mistral, DeepSeek (often blocked on governance grounds).

## Cross-cutting themes for the decks
1. **Broad but shallow adoption in NZ** — 91% use AI, 4% transform core ops [1]; top-decile NZ businesses get 14× the AI output per worker of the typical business [3]. That gap *is* the opportunity.
2. **Excel is the battleground** — Copilot, ChatGPT, Claude and Gemini (Sheets) all now build/edit models with traceable changes. Review controls over AI-built spreadsheets are an immediate need.
3. **General assistants are acquiring finance jobs** — month-end close, reconciliations, variance commentary — overlapping with ERP-native agents. Expect "which agent owns the close?" debates.
4. **Front door + MCP** — finance data flows to the assistant under the source system's permissions. Role design and approved-tool lists become finance controls.
5. **NZ data residency is a genuine differentiator** — none of the big assistant apps offers NZ in-country processing; Claude on Bedrock in Auckland is the in-country option today.
6. **Model plurality** — Microsoft runs OpenAI and Anthropic models; Perplexity routes across 20+; Workiva uses Google, Anthropic and OpenAI. Clients should avoid single-model lock-in.

## Tool folders
- `microsoft-365-copilot/research.md`
- `chatgpt-openai/research.md`
- `claude-anthropic/research.md`
- `gemini-google/research.md`
- `perplexity/research.md`

## Sources
1. NZ Herald — *AI adoption hits 91% of NZ businesses, but use to transform core operations falls to 4%* (premium): https://www.nzherald.co.nz/business/ai-adoption-hits-91-of-nz-businesses-but-use-to-transform-core-operations-falls-to-4/premium/OL64JRBISVERTED3NQTN3PXHHA/
2. Cairn — *AI adoption in New Zealand: the 2026 data* (citing AI Forum NZ Blueprint, May 2026): https://cairn.nz/blog/ai-adoption-in-new-zealand-the-2026-data-and-a-practical-guide
3. 1News — *Kiwis send 10 million ChatGPT messages a day* (4 Sept 2026): https://www.1news.co.nz/2026/09/04/kiwis-send-10-million-chatgpt-messages-a-day-as-work-use-climbs/
4. Microsoft — *In-country data processing for Microsoft 365 Copilot*: https://www.microsoft.com/en-us/copilot/blog/2025/11/04/microsoft-offers-in-country-data-processing-to-15-countries-to-strengthen-sovereign-controls-for-microsoft-365-copilot/
5. AI Forum NZ — *AI in Action* report: https://aiforum.org.nz/wp-content/uploads/2025/03/AI-in-Action_March2025-Report-compressed.pdf
6. Tool-level sources are listed in each tool's research.md.
