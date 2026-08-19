# Synthetic Operations Dashboard Blueprint

This is an original, generic dashboard concept for a public portfolio. It is not a reproduction of any client or employer report.

## Audience and question

An operations lead needs to understand whether a fictional case-handling service is keeping up with demand, meeting its service target, and reducing outstanding work.

## Page 1 — Operations overview

- KPI cards: new cases, completed cases, open backlog, and on-time rate
- Line chart: new cases versus completed cases by month
- Column chart: open backlog by region
- Donut chart: completed cases by service line
- Slicers: month, region, and service line

## Page 2 — Delivery detail

- Matrix: month by service line with new cases, completed cases, and on-time rate
- Bar chart: median review time by region
- Table: monthly operational summary with no individual-level records
- Narrative box: assumptions, refresh date, and limitations

## Example measures

Use measures that operate only on the fictional dataset:

```DAX
Completion Rate =
DIVIDE(SUM(Workflow[CompletedCases]), SUM(Workflow[NewCases]))

On-Time Rate =
AVERAGE(Workflow[OnTimeRate])

Backlog Change =
SUM(Workflow[OpenBacklog])
    - CALCULATE(SUM(Workflow[OpenBacklog]), DATEADD(Workflow[Month], -1, MONTH))
```

## Design rules

- Use a neutral palette and generic labels.
- Keep values rounded and clearly label them as synthetic.
- Avoid row-level detail, personal names, email addresses, case references, and external source URLs.
- Add alt text to every non-decorative visual before publishing screenshots.
