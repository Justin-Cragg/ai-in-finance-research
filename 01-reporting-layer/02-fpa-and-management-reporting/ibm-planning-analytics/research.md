# IBM Planning Analytics (TM1)

*Layer: Reporting → **FP&A & management reporting** (enterprise planning, budgeting, forecasting on the TM1 engine) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | IBM |
| **Product** | IBM Planning Analytics (TM1 engine) — as a Service (PAaaS, AWS/Azure), on Cloud, Certified Containers, and Local (on-prem); Planning Analytics Workspace (PAW) and Excel add-in |
| **AI brand** | **Planning Analytics Assistant / Planning Analytics Agent** (add-on); **MCP server tools**; extension via **watsonx Orchestrate** agents |
| **AI maturity** | **Stage 3→4**: in-product assistant plus MCP tools for custom agents across all deployment models (with OAuth, from Apr 2026) |
| **Models used** | Moved from IBM Granite 4 (watsonx.ai) to **GPT-OSS 120B on Amazon Bedrock** (Jul 2026) [3] |
| **NZ relevance** | **Long-established TM1 installed base** in NZ corporates, public sector and NFPs. NZ partner **CorPlan** (Auckland & Wellington) holds IBM **Platinum** status for Planning Analytics and runs NZ user events [5][6]; NZ example: **Presbyterian Support Central** [7]. AI now available in IBM's **Sydney** region [3] |

## Executive summary
- TM1 is the **incumbent many NZ finance teams already run**, often for 10–20 years. The AI question for those clients is "what do we get without migrating?". In 2026 the answer became substantial.
- **Planning Analytics Agent** (in PAW) offers natural-language chat over planning models, **Explain Cell**, **Variance Analysis** and **Chart Insights**. Answers are grounded in TM1 logic, so the AI explains *the model's* calculations rather than guessing. [2][3]
- **MCP server tools** went from PAaaS-only (Feb 2026) to **every deployment model, including on-prem Local** (Apr 2026, OAuth). That's unusual: it gives even on-premise TM1 customers a governed route into Claude, Copilot or custom agents. [1][4]

## How the AI works — plain English

### Planning Analytics Assistant / Agent [2][3]
| Feature | What it does |
|---|---|
| **Natural-language chat** | Ask questions of planning cubes; answers grounded in TM1 rules and hierarchies |
| **Explain Cell** | "Why is this number what it is?" Traces drivers and calculations behind a cell |
| **Variance Analysis** | Explains movements vs budget/forecast |
| **Chart Insights** | Narrates what a chart is showing |
| **Data Explorer** | Builds data views from a plain-English request |
| **Forecasting & simulation** | Baseline statistical forecasts, on-demand forecasting, scenario impact |

### MCP tools and custom agents [1][4]
- MCP tools expose things like "which cubes could answer this question?", "look up members" and "get data from Data Explorer", so an external agent can navigate TM1 safely.
- **watsonx Orchestrate** agents add multi-step automation with **human-in-the-loop approvals**, so a plan or forecast can trigger, or be updated by, agent workflows elsewhere in the enterprise. [2]

### Model change (Jul 2026) [3]
- IBM swapped its own Granite models for **GPT-OSS 120B on Amazon Bedrock** for a "substantial leap in model capability". It's a notable signal that even IBM is pragmatic about which LLM sits under the product. AI available in Dallas, Frankfurt and **Sydney**; 13 languages.

## Where it lands in the finance process
| Process | AI help | Human still owns |
|---|---|---|
| Monthly reporting | Explain Cell / variance narratives from the TM1 model | Board commentary |
| Budget & forecast | Statistical baseline; scenario simulation | Assumptions, approvals |
| Model support | NL navigation of complex cubes; reduces reliance on the one TM1 expert | Model governance |
| Cross-system automation | Orchestrate agents with approval steps | Approval decisions |

## Governance & control considerations
- **Licensing**: Data Explorer needs Planning Analytics Assistant licensing; MCP tools for custom agents are part of the **Planning Analytics Agent add-on**. [1][3]
- **Rollout lag by deployment**: PAaaS first; on Cloud next (2.1.23); **Local (on-prem) "future release"** for the in-product agent. Check which features a client's version actually has. [3]
- Model processing via Amazon Bedrock. Confirm the region (Sydney) and data-handling terms for NZ public-sector clients.

## Presentation talking points
- **"AI without migration"**: unlike HFM on-prem, legacy TM1 estates now get MCP access. A useful counterpoint to the "AI is a cloud dividend" theme.
- IBM moving from Granite to GPT-OSS shows that **the model is becoming a swappable component**. Value sits in the governed model and business logic.

## Sources
1. IBM Community — *IBM Planning Analytics Introduces the Next Wave of MCP tools and Agents* (2 Feb 2026): https://community.ibm.com/community/user/blogs/sami-el-cheikh1/2026/02/02/ibm-planning-analytics-introduces-the-next-wave-of
2. IBM — *Planning Analytics AI*: https://www.ibm.com/products/planning-analytics/ai
3. IBM Community — *A New AI Foundation for the IBM Planning Analytics Agent* (24 Jul 2026): https://community.ibm.com/community/user/blogs/sami-el-cheikh1/2026/07/24/a-new-ai-foundation-for-ibm-planning-analytics-age
4. IBM Community — *Introducing IBM Planning Analytics Assistant MCP Server Tools for Every Deployment Model* (26 Apr 2026): https://community.ibm.com/community/user/blogs/sami-el-cheikh1/2026/04/26/introducing-ibm-planning-analytics-assistant-mcp-s
5. ChannelLife NZ — *CorPlan attains IBM Platinum status for Planning Analytics*: https://channellife.co.nz/story/corplan-attains-ibm-platinum-status-for-planning-analytics
6. IBM Partner Plus directory — *CorPlan New Zealand*: https://ibm.com/partnerplus/directory/company/0026
7. CorPlan — *PSC acquires IBM Planning Analytics from CorPlan* (Nov 2020): https://corplan.co.nz/2020/11/17/press-release-psc-aquires-ibm-planning-analytics-from-corplan/
