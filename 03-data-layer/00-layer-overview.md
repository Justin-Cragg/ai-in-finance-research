# Data Layer — Market Leaders in NZ & AI Overview

*Last researched: 5 Oct 2026 · Audience: CFO / FC*

## What this layer is
Where finance data from the ERP, reporting tools and operational systems is combined, governed and analysed: data warehouses/lakehouses, the **semantic layer** (agreed definitions of revenue, margin, EBITDA…) and **BI**. For AI, this layer decides whether an agent's answer uses *your* numbers and *your* definitions.

> **Challenges on the original framing**
> 1. **"Are we missing any?" — yes: Microsoft Fabric / Power BI.** For most NZ finance teams the data layer *is* Power BI, and Fabric runs in Azure NZ North. It's #1 for NZ finance relevance.
> 2. **The hyperscalers (AWS, Google) belong here too** — they host most finance SaaS and offer their own warehouse + BI + model platforms.
> 3. **Make the semantic layer explicit.** Every vendor's 2026 AI pitch hinges on it (Snowflake Semantic Views, Databricks Unity Metrics, Fabric IQ/Power BI models, Looker LookML). It's the slide that explains *why finance must own data definitions*.
> 4. **BI tools** (Power BI, Tableau, Qlik) sit between Data and Reporting layers — suggest treating BI as part of Data for the decks.

## Top 5 suppliers in the NZ market

| # | Supplier / product | Why top 5 in NZ | AI maturity* | Headline AI | NZ hosting |
|---|---|---|---|---|---|
| 1 | **Microsoft Fabric & Power BI** | Power BI ubiquitous in NZ finance; Microsoft-centric enterprise IT | Stage 3→4 | Fabric IQ (GA) → answers in M365 Copilot; Copilot in Power BI; data agents | ✅ Azure NZ North (all Fabric workloads) |
| 2 | **Snowflake** | Leading cloud warehouse in ANZ enterprise; NZ region | Stage 4 | CoWork business agent (GA, Excel add-in); Cortex Agents; Semantic Views; Agent Identity | ✅ AWS Auckland |
| 3 | **Databricks** | Fastest-growing lakehouse in ANZ; data-science-heavy teams | Stage 4 | Genie One coworker; Agent Bricks; Unity Catalog Metrics; AI Gateway spend caps | ⚠️ No AWS NZ region; Azure NZ North unconfirmed |
| 4 | **AWS** (Redshift, SageMaker, Quick, Bedrock) | Hosts much of NZ's finance SaaS; Auckland region | Stage 3→4 | Amazon Quick agents & Flows; SageMaker Data Agent; **Claude in-region on Bedrock** | ✅ Auckland (Sept 2025) |
| 5 | **Google Cloud** (BigQuery, Looker) | Smaller finance footprint; strong in digital/marketing analytics | Stage 3→4 | Looker conversational analytics (GA); BigQuery agentic RCA; data agents | ⚠️ Gemini in BigQuery processing only US/EU-bound; Oceania processed globally |

\*Maturity stages defined in the root README.

### How the top 5 were chosen
No public NZ market-share data. Ranking reflects NZ finance-team prevalence (Power BI), in-country hosting, ANZ vendor momentum and partner presence. **Considered:** Oracle Autonomous Data Warehouse / Fusion Data Intelligence (Oracle ERP shops), **SAP Business Data Cloud** (SAP shops), Tableau (Salesforce), Qlik, Teradata, dbt (semantic layer tooling).

## Cross-cutting themes for the decks
1. **Semantic layer = finance's AI asset.** Snowflake cites 86% accuracy on structured questions *with* business context; every vendor now builds AI on governed metric definitions. Finance must own those definitions.
2. **The business-user agent has arrived in the data layer** — Snowflake CoWork, Databricks Genie One, Amazon Quick, Fabric IQ via Copilot. These compete with the "General" layer for the finance user's attention.
3. **Agents need identities and budgets.** Snowflake Agent Identity, Databricks AI Gateway spend caps, Fabric capacity billing — governance and cost control move into the data platform.
4. **Data residency differentiates in NZ.** In-country: Fabric (NZ North), Snowflake & AWS Bedrock/Claude (Auckland). Not in-country: Databricks on AWS (Sydney), Gemini in BigQuery (global processing for Oceania).
5. **Testing AI before it touches the numbers** — Databricks' automated evaluation / LLM judges — a theme for audit and assurance conversations.

## Tool folders
- `microsoft-fabric-power-bi/research.md`
- `snowflake/research.md`
- `databricks/research.md`
- `aws-redshift-quick/research.md`
- `google-bigquery-looker/research.md`

## Sources
1. Microsoft Learn — *Fabric region availability*: https://learn.microsoft.com/en-us/fabric/admin/region-availability
2. Snowflake docs — *Supported cloud regions*: https://docs.snowflake.com/en/user-guide/intro-regions
3. Databricks docs — *Supported AWS regions*: https://docs.databricks.com/aws/en/resources/supported-regions
4. AWS — *Bedrock in Asia Pacific (New Zealand)*: https://aws.amazon.com/blogs/machine-learning/run-generative-ai-inference-with-amazon-bedrock-in-asia-pacific-new-zealand/
5. Google Cloud docs — *Where Gemini in BigQuery processes your data*: https://docs.cloud.google.com/bigquery/docs/gemini-locations
6. Atlan — *Snowflake Summit 2026 announcements*: https://atlan.com/know/snowflake/summit-2026-announcements/
7. Tool-level sources are listed in each tool's research.md.
