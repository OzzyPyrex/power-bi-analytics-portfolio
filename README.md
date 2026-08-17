# Power BI Analytics Portfolio

A private staging index for four completed Power BI dashboard projects. The original PBIX files and source workbooks are intentionally not uploaded because Power BI embeds its data model and these reports contain real operational records, identifiers, employer branding, and sensitive business fields.

## Projects identified

### Contact-centre performance dashboard

- Combines monthly application and individual agent-performance reporting
- Two report pages with KPI cards, trends, comparisons, and detailed operational views
- Most mature local version contains approximately 35 visuals
- Portfolio version should use synthetic agent names, volumes, service levels, and outcomes

### NDLS licensing performance report

- One-page operational report with approximately 12 visuals
- Includes cards, bar and line charts, a pie chart, and detailed table views
- Original model references contact, agent, and disposition fields
- Public release requires synthetic records and removal of client/employer identifiers

### EV grant operations dashboard

- One-page dashboard with approximately 15 visuals
- Covers application review, funding, liability, tax-status, and exception indicators
- Original PBIX contains applicant-level data
- Public release requires a rebuilt synthetic model

### WAV 2026 grant dashboard

- One-page dashboard with approximately seven visuals
- Tracks application funnel, vehicle categories, budget, and operational impact
- Original model includes case references and applicant identifiers
- Public release requires synthetic cases and values

## Publication plan

For each public case study:

1. Rebuild the model with fictional or fully anonymised data.
2. Remove employer and client branding unless permission is confirmed.
3. Verify that screenshots contain no names, IDs, contact details, or confidential metrics.
4. Document the KPI definitions, data model, Power Query steps, and key DAX measures.
5. Publish the safe PBIX, screenshots, data dictionary, and synthetic dataset.

## Data safety

Do not commit original PBIX files, monthly exports, operational-impact documents, or raw screenshots. A private GitHub repository is not a substitute for employer or client approval.

## Status

Portfolio preparation is in progress. The local source projects have been inventoried; sanitised case studies have not yet been generated.
