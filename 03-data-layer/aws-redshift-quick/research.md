# AWS — Amazon Redshift, SageMaker Unified Studio, Amazon Quick & Bedrock

*Layer: Data (cloud data warehouse, analytics, AI platform) · Last researched: 5 Oct 2026*

| | |
|---|---|
| **Vendor** | Amazon Web Services |
| **Products** | **Amazon Redshift** (warehouse), **SageMaker Unified Studio** (data + AI workspace), **Amazon Quick Suite** (agentic BI/workspace, evolved from QuickSight), **Amazon Bedrock** (foundation models) |
| **AI brand** | Amazon Quick (chat agents, Flows, Research), SageMaker Data Agent, Bedrock (Claude, Nova) |
| **AI maturity** | **Stage 3→4** – business-user agents (Quick) and in-region frontier models (Bedrock) |
| **NZ relevance** | **AWS Asia Pacific (New Zealand) region, Auckland, opened Sept 2025** [5]; **Claude models run in-region on Bedrock** with an AU/NZ-only cross-region routing option [4] — the strongest NZ data-residency story for generative AI. Many NZ finance tools (Xero, Workiva, Snowflake etc.) run on AWS |

## Executive summary
- AWS is a **platform/builder choice** rather than a finance-user product — but it underpins much of the finance SaaS stack and offers the best NZ residency for GenAI.
- **Amazon Quick** turns BI into agents: chat agents query Redshift, run regression/Monte Carlo/scenario models; **Flows** schedule them. AWS's own finance team cut per-customer deep-dive analysis from ~6 hours to ~10 minutes and automated weekly business reviews. [1]
- **SageMaker Data Agent** (Mar 2026) converts plain-English questions to SQL on Redshift/Athena, proposing a step-by-step plan first. [2]

## How the AI works — plain English

### Amazon Quick Suite [1][3]
- **Chat agents** connected to enterprise data (Redshift, S3, apps) for interactive analysis.
- **Flows**: automate recurring analyses (e.g. every Monday 6am produce regional revenue insights).
- Successor to QuickSight dashboards, adding research and automation.

### SageMaker Unified Studio + Data Agent [2]
- Single workspace for data engineering, SQL analytics and ML. Data Agent writes and debugs SQL ("Fix with AI") with schema awareness.

### Amazon Bedrock in NZ [4]
- Claude (Opus, Sonnet, Haiku) and Amazon Nova 2 Lite available in Auckland; **AU geographic profile** keeps inference within Auckland/Sydney/Melbourne; data at rest stays in source region.

## Finance use cases
| Use case | How |
|---|---|
| Portfolio-wide customer/risk analysis | Quick chat agent over Redshift with Monte Carlo [1] |
| Weekly business review automation | Quick Flows [1] |
| Custom finance agents with NZ residency | Bedrock (Claude) in Auckland + Redshift |
| Analyst SQL productivity | SageMaker Data Agent |

## Considerations
- More assembly required than Fabric/Snowflake; typically partner- or engineering-led.
- Strong residency, but confirm each service (Redshift, Quick, SageMaker) is available in ap-southeast-6 for a given client.

## Presentation talking points
- **Residency is solvable**: "Your GenAI can run in Auckland" is a powerful message for NZ boards wary of offshore AI.
- AWS finance's own results are a credible "customer zero" case study. [1]

## Sources
1. AWS ML blog — *How AWS Finance teams reclaimed hundreds of hours with Amazon Quick* (7 Jul 2026): https://aws.amazon.com/blogs/machine-learning/how-aws-finance-teams-reclaimed-hundreds-of-hours-with-amazon-quick/
2. AWS What's New — *Amazon SageMaker Data Agent in the Query Editor* (30 Mar 2026): https://aws.amazon.com/about-aws/whats-new/2026/03/amazon-sagemaker-data-agent-query-editor
3. AWS BI blog — *QuickSight evolves to Amazon Quick Suite*: https://aws.amazon.com/blogs/business-intelligence/reimagine-business-intelligence-amazon-quicksight-evolves-to-amazon-quick-suite/
4. AWS ML blog — *Run generative AI inference with Amazon Bedrock in Asia Pacific (New Zealand)* (26 Mar 2026): https://aws.amazon.com/blogs/machine-learning/run-generative-ai-inference-with-amazon-bedrock-in-asia-pacific-new-zealand/
5. GCN — *AWS launches New Zealand cloud region with three zones* (Sept 2025): https://gcn.com/aws-launches-new-zealand-cloud-region-three-zones/9235/
6. AWS — *AI for finance teams (Amazon Quick)*: https://aws.amazon.com/quick/finance/
