# Google Cloud — BigQuery & Looker (Agentic Data Cloud)

*Layer: Data (warehouse + BI) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Google Cloud |
| **Products** | **BigQuery** (warehouse/lakehouse), **Looker** (governed BI + semantic layer, LookML), Gemini Enterprise |
| **AI brand** | **Gemini in BigQuery**, **Conversational Analytics**, **data agents** (Data Engineering, Data Science, Looker Dashboard, Deep Research), managed MCP servers |
| **AI maturity** | **Stage 3→4** – GA data engineering agent and Looker conversational analytics; much else in preview |
| **NZ relevance** | Smaller NZ finance footprint than Microsoft/AWS; common in digital-native and marketing-analytics teams. **Important caveat: Gemini in BigQuery only offers processing residency in US or EU — Oceania data is processed globally** [2] |

## Executive summary
- Google's strength is **Looker's semantic layer (LookML)** — governed metric definitions that ground Gemini's answers — plus BigQuery's scale.
- 2026 "Agentic Data Cloud": **Looker Conversational Analytics agent (GA)**, **embedded conversational analytics (GA)**, **Data Engineering Agent (GA)**; Deep Research, BigQuery conversational analytics with agentic root-cause analysis, and Gemini Enterprise "front door" in preview. [1]
- **NZ residency is the weak point** for GenAI features: Gemini in BigQuery processing is only jurisdiction-bound for US/EU. [2]

## How the AI works — plain English [1]
| Capability | What it does | Status |
|---|---|---|
| **Looker Conversational Analytics agent** | Ask questions in plain English; grounded in LookML semantic model | GA |
| **Looker Dashboard Agent** | Q&A and AI summaries inside dashboards | Preview |
| **Conversational Analytics in BigQuery** | NL query with reasoning; agentic root-cause analysis and scheduled actions | Preview (agentic) |
| **Data Engineering Agent** | Builds/fixes pipelines from natural language | GA |
| **Deep Research Agent** | Research plan across internal docs, BigQuery tables and the web | Preview |
| **Gemini Enterprise front door** | Publish BigQuery/Looker agents to business users | Preview |
| **Managed MCP servers** (databases GA; Looker preview) | Let any MCP-capable AI client query governed data | GA / Preview |

## Finance use cases
| Use case | How |
|---|---|
| Variance root-cause | BigQuery conversational analytics with agentic RCA |
| Governed KPI Q&A | Looker conversational agent over LookML finance metrics |
| Embedded finance analytics | Looker embedded conversational analytics in internal apps |

## Considerations
- **Data residency** (above) is a material issue for NZ public sector and regulated entities. [2]
- Many agent features are preview.

## Presentation talking points
- Use Google to make the **semantic layer** point (LookML) and the **residency** point — the same AI feature can be acceptable or not depending on where it processes data.

## Sources
1. Google Cloud blog — *New data agents across the Agentic Data Cloud* (2026): https://cloud.google.com/blog/products/data-analytics/new-data-agents-across-the-agentic-data-cloud
2. Google Cloud docs — *Where Gemini in BigQuery processes your data*: https://docs.cloud.google.com/bigquery/docs/gemini-locations
3. Google Cloud blog — *Conversational Analytics in Google Data Cloud in Q3'26*: https://cloud.google.com/blog/products/data-analytics/conversational-analytics-in-google-data-cloud-in-q326
4. Rittman Analytics — *Google Next 2026: what's new for Looker, BigQuery and agentic analytics*: https://blog.rittmananalytics.com/google-next-2026-whats-new-for-looker-bigquery-data-platforms-and-agentic-analytics-732cb3c1aa1b
5. Google NZ blog — *Bringing our first cloud region to Aotearoa New Zealand*: https://blog.google/intl/en-nz/company-news/2022_08_bringing-our-first-cloud-region-to-nz/
