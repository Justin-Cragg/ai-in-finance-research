# Microsoft Fabric & Power BI

*Layer: Data (unified analytics platform: OneLake, data engineering, warehouse, Power BI) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Microsoft |
| **Products** | **Microsoft Fabric** (OneLake, Data Factory, Warehouse, Real-Time, Data Science) incl. **Power BI** |
| **AI brand** | **Fabric IQ**, ontology, **Fabric data agents**, **Copilot in Power BI / Fabric**; surfaces in **Microsoft 365 Copilot** (Chat, Cowork) |
| **AI maturity** | **Stage 3→4** – Fabric IQ GA, feeds M365 Copilot; data agents and ontology in preview |
| **NZ relevance** | **Most likely data/BI platform in a NZ finance team** — Power BI is ubiquitous for management reporting; Fabric runs in Azure **New Zealand North** with Power BI and all Fabric workloads available [3] |

## Executive summary
- **The user's original list missed Microsoft** — for most NZ finance teams the "data layer" *is* Power BI (and increasingly Fabric). It also anchors the Microsoft ERP (Dynamics) and general-AI (Copilot) stories.
- **Fabric IQ (GA, FabCon 2026)**: a shared "intelligence layer" combining OneLake data, **Power BI semantic models** and **ontologies**, so people and agents get consistent business meaning. It flows into **Microsoft 365 Copilot Chat and Cowork** — so an FC can ask Copilot about the numbers and it answers from the governed Power BI model. [1]
- **Existing Power BI semantic models become AI assets** — the measures finance has already built (DAX) can be reused in the ontology. [1]

## How the AI works — plain English

### 1. Fabric IQ & ontology — business meaning for AI [1]
- **Fabric IQ** connects data, metrics and operational context once; any Copilot or agent reuses it.
- **Ontology creation (preview)**: define business rules in natural language, link them to entities (customer, product, cost centre) and relationships, reuse Power BI measures.

### 2. Copilot in Power BI [1][4]
- Ask questions of reports, generate report pages and **narrative summaries** of visuals, write DAX.
- **Agentic app creation (preview)**: describe a data application in natural language; Copilot builds it with authentication and security.

### 3. Fabric data agents [1][5]
- Configurable agents scoped to specific data (lakehouse, warehouse, semantic model) that answer questions; can be plugged into **Copilot Studio** agents and M365 Copilot. Ontology integration improves explainability. (Preview enhancements.)

### 4. Microsoft 365 Copilot integration [1]
- Business context from Fabric IQ available in **Copilot Chat and Cowork** "without additional token costs" (per Microsoft).

## Finance use cases
| Use case | How |
|---|---|
| Management reporting | Copilot narrative summaries on Power BI board/month-end packs |
| "Ask the numbers" in Teams/Outlook | M365 Copilot grounded by Fabric IQ |
| Finance data products | Fabric data agents over GL/sub-ledger marts |
| Excel-heavy FP&A | Copilot in Excel + Power BI semantic models |

## Considerations
- **Capacity-based pricing**: Copilot/AI consumes Fabric capacity (Fabric Copilot Capacity billing) — size and monitor. [4]
- Several AI features are **preview** — check GA before client commitments. [1]
- Strong **NZ residency** position (NZ North). [3]
- Governance: the quality of AI answers = the quality of the Power BI semantic model; certify finance models.

## Presentation talking points
- "You've already built your AI's brain — it's your Power BI model." Strong, practical message for NZ FCs.
- Microsoft is the only vendor spanning ERP (Dynamics), data (Fabric) and general AI (Copilot) — an integrated-stack argument vs best-of-breed.

## Sources
1. Microsoft Azure blog — *FabCon and SQLCon 2026 (Barcelona): data foundation for Microsoft Copilot and agents*: https://azure.microsoft.com/en-us/blog/fabcon-and-sqlcon-2026-in-barcelona-building-the-data-foundation-for-microsoft-copilot-and-agents/
2. CloudNews — *Microsoft brings Fabric IQ to Copilot with Power BI data*: https://cloudnews.tech/microsoft-brings-fabric-iq-to-copilot-to-answer-with-power-bi-data/
3. Microsoft Learn — *Fabric region availability* (New Zealand North): https://learn.microsoft.com/en-us/fabric/admin/region-availability
4. Microsoft Learn — *Copilot for Microsoft Fabric and Power BI: FAQ*: https://learn.microsoft.com/en-us/fabric/fundamentals/copilot-faq-fabric ; *Fabric Copilot Capacity*: https://learn.microsoft.com/en-us/fabric/enterprise/fabric-copilot-capacity
5. Microsoft Learn — *Fabric data agent tenant settings*: https://learn.microsoft.com/en-us/fabric/data-science/data-agent-tenant-settings
6. Microsoft Fabric community — *Fabric September 2026 feature summary*: https://community.fabric.microsoft.com/blog/fbc_fabricupdatesblogs/fabric-september-2026-feature-summary/5325825
