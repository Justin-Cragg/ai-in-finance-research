# Workiva

*Layer: Reporting → **External reporting** (annual reports, XBRL, sustainability/climate statements, GRC) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Workiva (NYSE: WK) |
| **Product** | Workiva platform — financial reporting, sustainability/ESG & carbon, GRC/controls, connected data |
| **AI brand** | **Workiva AI** — purpose-built agents, Agent Studio, Workiva Knowledge, Intelligent Companion, Workiva MCP |
| **AI maturity** | **Stage 3→4** – specialised reporting agents (Jul 2026) + MCP gateway |
| **Models used** | Frontier models from Google, AWS/Anthropic and Microsoft/OpenAI; customer prompts/outputs not used for training [3] |
| **NZ relevance** | The "last mile" tool for annual reports and **climate statements** under the NZ Climate-Related Disclosures (CRD) regime. Note the regime is being narrowed (listed-issuer threshold raised from NZ$60m to NZ$1bn market cap; reporting entities ~164 → ~76), which shrinks the mandatory market [5] |

## Executive summary
- Workiva sits **after** consolidation: it turns approved numbers into the annual report, notes, XBRL and sustainability report — so its AI is about **drafting, checking and tying-out**, not forecasting.
- **July 2026: specialised agents launched** — Tie-Out, Benchmarking and Sustainability Disclosure — plus **Workiva Knowledge**, a reusable knowledge base grounded in the company's own filings, memos and auditor guidance. [1] Amplify (Sept 2026) added Roll Forward + Prep and XBRL Validation agents. [2]
- **Agent Studio** lets finance build their own agents by describing a workflow — no code. [3]

## How the AI works — plain English

### Specialised reporting agents [1][2]
| Agent | What it does | How |
|---|---|---|
| **Roll Forward + Prep** | Gets next period's report ready | Updates dates, resets labels, renames folders, rolls historical figures forward using a blueprint |
| **Tie-Out** | Checks every number agrees across the document | Flags mismatches, explains them in plain English, links to source; reviewer applies tick-marks individually or in bulk |
| **Validation (XBRL)** | Fixes tagging errors faster | Translates cryptic XBRL validation messages into plain-English cause + fix |
| **Benchmarking Insights** | "What do our peers disclose that we don't?" | Analyses peer filings for gaps/outlier wording; drafts language with citations to peer filings (*note: SEC filings — limited NZ peer coverage*) |
| **Sustainability Disclosure** | Draft and gap-check sustainability reports | Drafts/validates against ESRS and ISSB; produces gap assessments and compliance scorecards |

### Workiva Knowledge (the "intelligence layer")
- Customers upload accounting memos, policies, prior filings and auditor guidance; AI drafting is **grounded in and cites** that material, and it compounds cycle-to-cycle. [1][2]

### Agent Studio & Intelligent Companion
- No-code agent builder ("describe your workflow") and an in-platform chat companion. [3]

### Workiva MCP
- Connects Workiva data to the enterprise's own AI tools while Workiva remains the system of record; every interaction is logged against the user *and* the connecting tool. [2][3]

## Where it lands in the finance process
| Process | AI help | Human still owns |
|---|---|---|
| Annual / half-year report | Roll-forward, tie-out, drafting from knowledge base | Disclosure judgement, sign-off |
| XBRL / regulatory filing | Validation explanations | Tagging decisions |
| Climate / sustainability statement | Drafting + gap check vs ISSB-aligned standards | Scenario analysis, materiality |
| Controls / audit readiness | Audit trail of every AI action | Control design |

## Governance & control considerations
- Human-in-the-loop is designed in (tick-marks, overrides), and all agent output is traceable to source. [2]
- Agents are in **advanced solution tiers** — check licensing. [1]
- Data privacy: encryption in transit; no training on customer prompts/outputs. [3]

## Presentation talking points
- The clearest example of AI that **makes the audit file stronger, not weaker** — every check is evidenced.
- Tie-out is a universally recognised pain point; good live demo candidate.
- NZ caveat: CRD scope narrowing means Workiva's NZ growth story is more about annual-report efficiency than mandatory climate reporting. [5]

## Sources
1. Workiva Investor Relations — *Workiva Launches Specialized AI Agents and Intelligence Layer* (29 Jul 2026): https://investor.workiva.com/news-releases/news-release-details/workiva-launches-specialized-ai-agents-and-intelligence-layer
2. Workiva blog — *Agents, Oversight, and Governance: What's New for Financial Reporting at Amplify 2026*: https://www.workiva.com/blog/agents-oversight-and-governance-whats-new-financial-reporting-amplify-2026
3. Workiva — *Workiva AI*: https://www.workiva.com/platform/workiva-ai
4. SiliconANGLE — *Workiva bets on trust as AI agents enter financial reporting* (15 Sept 2026): https://siliconangle.com/2026/09/15/workiva-bets-trust-ai-agents-enter-financial-reporting-amplify/
5. ESG News — *New Zealand lifts climate reporting thresholds*: https://esgnews.com/new-zealand-lifts-climate-reporting-thresholds-to-revive-capital-markets/
6. PwC NZ — *Finding value in a shifting climate reporting landscape* (2026): https://www.pwc.co.nz/insights-and-publications/2026-publications/finding-value-in-a-shifting-climate-reporting-landscape.html
