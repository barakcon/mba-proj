## Create a lean architecture diagram for the AdoptAI product.

The diagram should show a simple left-to-right data flow with three horizontal rows, one row per department:
1. R&D
2. Sales
3. Marketing

Use three main vertical sections across the diagram:

Left section: Data Sources
This section shows the systems/tools where usage and activity data comes from.

Middle section: AdoptAI Usage Visibility
This section represents AdoptAI as the intelligence layer that gives visibility into how AI/tools are being used across each department. Keep this section simple. Do not show detailed steps like ingest, normalize, benchmark, or recommend. Just show that AdoptAI provides usage visibility and connects source data to business performance metrics.

Right section: Performance Metrics
This section shows the business or operational metrics that AdoptAI maps usage data to. Make these look like measurable KPI/metric outputs, not generic labels.

Data flow:
For each department row, show arrows moving from:
Data Sources -> AdoptAI Usage Visibility -> Performance Metrics

Rows:

R&D row:
- Data Sources: Claude, Cursor, Git, Jira
- Performance Metrics: SDLC, DORA

Sales row:
- Data Sources: Salesforce, Gong, Outreach, ZoomInfo, and other sales tools
- Performance Metrics: New Logos, New ARR, New Expansions

Marketing row:
- Data Sources: HubSpot, Google Analytics, LinkedIn Ads, Meta Ads, Glean
- Performance Metrics: Referrals, Leads, Exposure

Design requirements:
- Keep the architecture simple and clean.
- Focus on the data areas and the flow between them.
- Avoid unnecessary details.
