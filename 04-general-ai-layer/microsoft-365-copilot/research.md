# Microsoft 365 Copilot

*Layer: General AI (productivity assistant) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Microsoft |
| **Product** | Microsoft 365 Copilot (Chat, Word, **Excel**, PowerPoint, Outlook, Teams), **Copilot Cowork**, finance agents in Microsoft 365, Copilot Studio, Agent 365 |
| **Models** | Multi-model: OpenAI models plus **Anthropic Claude** (via Frontier programme; Copilot Cowork built with Anthropic) [1] |
| **AI maturity** | **Stage 4** – agents in Office apps, long-running Cowork tasks, enterprise agent control plane |
| **NZ relevance** | Default enterprise AI in NZ because most organisations are on Microsoft 365. **No NZ in-country Copilot processing announced** — Australia is the nearest in-country option [3] |

## Executive summary
- **Copilot works where finance already works — Excel, Outlook, Teams — and on data the firm already holds** (SharePoint, mail, Power BI via Fabric IQ, Dynamics/SAP via finance agents).
- **March 2026 ("Wave 3")**: agentic editing GA in Excel and Word; **Copilot Cowork** for long-running multi-step work (built with Anthropic); Claude available in Copilot chat; **Agent 365** control plane (US$15/user/month) and **Microsoft 365 E7** bundle (US$99/user/month) from 1 May 2026. [1]
- **Finance agents in Microsoft 365**: **Financial Reconciliation** and **Variance Analysis** agents working from Excel/Outlook, connected to **Dynamics 365 Finance and SAP**, with separate licensing. [2]

## How the AI works — plain English
| Capability | What it does for finance |
|---|---|
| **Excel agentic editing / Agent Mode** | Describe the model or analysis; Copilot builds/edits the workbook step by step and explains changes [1][4] |
| **Copilot Cowork** | Breaks a complex request (e.g. "prepare the month-end pack from these files") into steps across files and tools, with visible progress [1] |
| **Financial Reconciliation agent** | Compares data across sources; classifies matched / unmatched / possible matches; surfaces exceptions [2] |
| **Variance Analysis agent** | Drafts structured commentary on variances for management/board reporting, pulling from ERP [2] |
| **Work IQ / Fabric IQ grounding** | Answers grounded in your mail, files, meetings and Power BI semantic models [1] |
| **Copilot Studio + Agent 365** | Build custom finance agents; inventory, secure and monitor all agents centrally [1] |

## Governance & commercial considerations
- Inherits Microsoft 365 permissions — **oversharing in SharePoint becomes an AI risk**; permission hygiene first.
- **Data residency:** in-country processing promised for Australia, UK, US, India, UAE by end-2026 — **not NZ**. [3]
- Licensing layers: Copilot seat, finance-agent licensing, Copilot Credits for agents, Agent 365 / E7. [1][2]
- Finance agents expose ERP data-quality issues rather than fix them. [2]

## Presentation talking points
- For most NZ finance teams Copilot is the **"front door"** — and ERP/reporting vendors are now plugging into it (OneStream, Xero, SAP).
- Multi-model Copilot (OpenAI + Claude) shows the general layer is becoming model-agnostic.

## Sources
1. Microsoft — *Powering Frontier Transformation with Copilot and agents* (9 Mar 2026): https://www.microsoft.com/en-us/copilot/blog/2026/03/09/powering-frontier-transformation-with-copilot-and-agents/
2. PrimeAI — *Microsoft Copilot for Finance setup guide (2026)*: https://www.primeai.solutions/blog/microsoft-copilot-finance-setup ; Microsoft Learn — *Finance agents in Microsoft 365, 2026 release wave 1*: https://learn.microsoft.com/en-us/copilot/release-plan/2026wave1/finance-agents/planned-features
3. Microsoft — *In-country data processing for 15 countries* (Nov 2025, updated Apr 2026): https://www.microsoft.com/en-us/copilot/blog/2025/11/04/microsoft-offers-in-country-data-processing-to-15-countries-to-strengthen-sovereign-controls-for-microsoft-365-copilot/
4. Microsoft — *Vibe working: Agent Mode and Office Agent* (Sept 2025): https://www.microsoft.com/en-us/copilot/blog/2025/09/29/vibe-working-introducing-agent-mode-and-office-agent-in-microsoft-365-copilot/
5. A Guide to Cloud — *Microsoft 365 Copilot data residency & sovereignty for ANZ*: https://www.aguidetocloud.com/blog/microsoft-365-copilot-data-residency-anz-government/
