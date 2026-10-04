# Reporting Layer → External Reporting — NZ Market Leaders & AI Overview

*Last researched: 5 Oct 2026 · Audience: CFO / FC · Parent: [Reporting layer overview](../00-layer-overview.md)*

## What this sub-layer is
The "last mile" from approved numbers to **published, assured documents**: statutory financial statements and notes, annual and half-year reports, disclosure checklists, **climate statements** (NZ CRD regime), sustainability reports, regulatory returns and (where required) XBRL.

### NZ context that shapes this sub-layer
- **No XBRL mandate.** NZ financial statements are filed with the Companies Office / Disclose register without a prescribed digital format. The XRB has published a position paper on digital financial reporting (May 2024), but there's no mandate yet [1]. XBRL-centric tools (Workiva's XBRL agents, Certent, DFIN) matter less here than in the US/EU.
- **Climate statements are narrowing.** The CRD regime's listed-issuer threshold rose from NZ$60m to **NZ$1bn market cap** (~164 → ~76 reporting entities) [2]. The FMA reviewed **62 climate statements** in year two and wants better physical-risk, data-quality and GHG-assurance disclosure, not more volume [3].
- **Most NZ statutory accounts are produced in Caseware, practice tools or Word/Excel**, not a disclosure-management platform. Workiva dominates only at the large listed / large public-entity end.

## Top 5 in the NZ market

| # | Supplier / product | Who uses it in NZ | AI maturity* | Headline AI |
|---|---|---|---|---|
| 1 | **[Workiva](workiva/research.md)** | Listed issuers, large public entities: annual report, climate statement, GRC | Stage 3→4 | Tie-Out, Roll-Forward, XBRL Validation, Sustainability Disclosure agents; Workiva Knowledge; MCP |
| 2 | **[Caseware](caseware/research.md)** (Working Papers / Cloud Financials) | Accounting and audit firms, corporates, government-related entities preparing statutory FS; NZ Tier 1/Tier 2 templates | Stage 2 in ANZ (Stage 3 in US) | **Caseware Verity** (May 2026): Disclosure Checklist Agent (US only so far), document intelligence, risk suggestions; AiDA assistant |
| 3 | **Oracle EPM Narrative Reporting** | Oracle/HFM-estate groups producing board packs and annual-report sections from EPM | Stage 3 | GenAI commentary, preparer-note summaries, **causality analysis** (Jun 2026), Reporting Agent — see [Oracle EPM](../01-consolidation-and-close/oracle-epm/research.md) |
| 4 | **Microsoft Word / Excel + Microsoft 365 Copilot** | The de-facto annual report toolset for most NZ entities outside Workiva | Stage 2→3 | Drafting, summarising, comparing to prior year; Copilot agents — see [General AI → Microsoft 365 Copilot](../../04-general-ai-layer/microsoft-365-copilot/research.md) |
| 5 | **Sustainability data platforms** (Toitū Envirocare eManage; IBM Envizi) | Emissions inventories and data feeding climate statements | Stage 0–1 (Toitū); Stage 1–2 (Envizi) | Toitū: no AI announced (NZ$18m digitisation programme) [4]; Envizi: watsonx NLP for emissions data categorisation, AI forecasting [5] |

\*Maturity stages defined in the root README.

### How the top 5 were chosen
External reporting in NZ is **concentrated**: there's one dominant disclosure-management platform (Workiva), one dominant statutory-accounts tool (Caseware), and everyone else uses EPM-native narrative tools or Office. Rather than pad the list with US SEC-filing tools that barely operate in NZ, the top 5 reflects **how NZ entities actually produce external reports**. Two slots point to tools researched elsewhere in this repo (Oracle Narrative Reporting, Microsoft 365 Copilot). **Validate with Deloitte NZ Audit & Assurance and the Sustainability practice.**

### Considered but not in the top 5
| Product | Why not top 5 (NZ) | AI note |
|---|---|---|
| **CCH Tagetik Disclosure Management / ESG** | Small NZ base | ESG and IFRS data-entry agents; regulatory data lineage — see [CCH Tagetik](../01-consolidation-and-close/cch-tagetik/research.md) |
| **insightsoftware Certent Disclosure Management** | Workiva's main lower-cost rival globally; US/EU XBRL focus; little NZ evidence | 2026 edition: narratives that auto-update when numbers change; built-in XBRL tagging [6] |
| **DFIN ActiveDisclosure, Toppan Merrill Bridge, IRIS CARBON** | US SEC / EDGAR or XBRL-centric | — |
| **Xero / MYOB practice tools** (statutory and special-purpose FS for SMEs) | High volume in NZ SMEs, produced by accounting practices | See [ERP layer → Xero](../../02-erp-layer/xero/research.md) / [MYOB](../../02-erp-layer/myob/research.md) |
| **Spotlight Sustain** | ESG reporting for SME advisors (free for SVCFOs from Mar 2026) | See [Spotlight Reporting](../02-fpa-and-management-reporting/sme-vcfo-tier/spotlight-reporting/research.md) |
| **Other carbon platforms** (BraveGen, Cogo, Sumday, Persefoni, Watershed) | Fragmented NZ market; Sumday (Australian, "AI-native", Xero-linked) worth watching | Varies |

## What AI is doing in external reporting (themes)
1. **"Checking" agents come before "writing" agents.** The highest-value early AI is verification: Workiva Tie-Out, Caseware Disclosure Checklist Agent, Workiva XBRL Validation. It's rule-based, citation-friendly, and makes the **audit file stronger**.
2. **Grounded drafting from your own knowledge base.** Workiva Knowledge (memos, policies, prior filings) and Oracle's preparer-note summaries draft only from approved sources, with citations, because external reports carry legal liability.
3. **Narrative linked to numbers.** Certent's auto-updating narratives, Oracle's causality analysis and Workiva's roll-forward attack the classic annual-report error: text that no longer matches the final numbers.
4. **Climate data is the weak link, not the drafting.** The FMA's findings (physical risk, data quality, GHG assurance) are about the data, and NZ's leading emissions tools have little AI yet. Drafting agents (Workiva Sustainability Disclosure) can't fix weak inputs.
5. **US-first availability.** Caseware's agent is US-only and Workiva's benchmarking leans on SEC filings. **Check NZ availability and NZ-standard content (NZ IFRS, PBE, NZ CS 1–3)** before promising anything to clients.

## Deck use
- **AI in financial reporting deck:** "AI that makes the audit file stronger" (tie-out + disclosure checklist); live demo candidate is Workiva Tie-Out; NZ CRD scope-narrowing caveat.
- **vCFO deck:** Caseware for practices preparing client statutory accounts; Copilot in Word for SME annual reports.

## Tool folders
- [workiva/research.md](workiva/research.md)
- [caseware/research.md](caseware/research.md)

## Sources
1. XRB — *Digital Financial Reporting: XRB Position Paper* (May 2024): https://www.xrb.govt.nz/dmsdocument/5118/ ; IFRS Foundation — *New Zealand filing profile*: https://www.ifrs.org/content/dam/ifrs/publications/jurisdictions/filing-profiles/new-zealand-18-november-2015.pdf
2. ESG News — *New Zealand lifts climate reporting thresholds*: https://esgnews.com/new-zealand-lifts-climate-reporting-thresholds-to-revive-capital-markets/
3. FMA — *Climate disclosures improving, but sharper focus needed on physical risks and impacts* (26 May 2026): https://www.fma.govt.nz/news/all-releases/media-releases/crd-reporting-insights-2026/
4. Toitū Envirocare — *Climate-related disclosures*: https://www.toitu.co.nz/solutions/climate-related-disclosures/ ; BusinessDesk — *Toitū Envirocare's $18m digitisation to make it the 'Xero' of emissions certification*: https://businessdesk.co.nz/article/sustainable-finance/toitu-envirocares-18m-digitisation-to-make-it-the-xero-of-emissions-certification
5. IBM — *IBM Envizi*: https://www.ibm.com/products/envizi ; Technology Magazine — *IBM watsonx powers sustainability progress*: https://technologymagazine.com/data-and-data-analytics/ibm-watsonx-new-technology-powers-sustainability-progress
6. insightsoftware — *How Certent Disclosure Management simplifies regulatory reporting*: https://insightsoftware.com/blog/how-certent-disclosure-management-simplifies-regulatory-reporting/
7. Sentrient — *Top Workiva alternatives for Australian business*: https://www.sentrient.com.au/blog/workiva-alternatives
8. Tool-level sources are in each tool folder.
