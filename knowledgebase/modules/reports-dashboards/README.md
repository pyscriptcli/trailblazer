# Salesforce Trailhead Study Notes: Reports & Dashboards for Lightning Experience

**Badge:** [Reports & Dashboards for Lightning Experience](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_reports_dashboards?trail_id=force_com_admin_beginner)  
**Level:** Foundational · Administrator  
**Trailhead estimate:** About 1 hour 50 minutes · 5 units

Reports answer a defined question with selected Salesforce records. Dashboards arrange report-based components to make important measures and trends visible at a glance.

## Units and outcomes

1. [Get to Know Lightning Reports and Dashboards](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_overview) — translate a business question into criteria; distinguish reports, report types, folders, and dashboards.
2. [Create Reports with the Report Builder](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_using_report_builder) — select a report type, add fields, configure Outline and Filters, save, and run the report.
3. [Filter Your Report](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_filter_your_report) — use standard and field filters, filter logic, cross filters, and row limits.
4. [Format Your Report](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats) — choose tabular, summary, or matrix based on how the audience needs to scan and compare data.
5. [Visualize Your Data with the Lightning Dashboard Builder](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data) — use source reports to build dashboard charts, tables, metrics, or gauges; consider dynamic dashboard viewing context.

## Translate a question into a report

Before building, clarify terms such as “top,” “recent,” or “successful.” Ask which records count, what date range applies, whether inactive records belong, how results should be grouped, and what calculation answers the question. Then choose the report type and define columns, filters, groupings, summary calculations, and (when useful) a chart.

| Concept | What it means |
|---|---|
| Report | A saved view of records that match criteria; it can filter, group, summarize, and chart data. |
| Report type | The template that determines which primary and related records and fields are available. |
| Report folder | Controls who can view, edit, or manage reports stored there. |
| Dashboard | A page of components that visualize data from source reports; each data component uses one source report. |

## Filters and formats

- **Standard filters** include common scoping such as records the user sees and date ranges.
- **Field filters** specify a field, operator, and value.
- **Filter logic** combines field filters with AND/OR logic; it does not combine standard filters.
- **Cross filters** include or exclude records based on related child records, such as Accounts with Opportunities.
- **Row limits** restrict tabular report output and can support a dashboard component.

| Format | Best for |
|---|---|
| Tabular | A flat list of records. |
| Summary | Records grouped and summarized by row fields. |
| Matrix | Grouping and comparing by both rows and columns. |

Choose a format only after deciding what comparison the question needs. Dashboard widgets should make the result easier to act on; charts show patterns, metrics highlight one value, gauges place one value in a range, and tables preserve row-level detail.

## Build and check

1. From the Reports tab, start a report and select the report type that exposes the needed records and fields.
2. Add fields and apply the smallest useful date range and filters.
3. Group and summarize if the question requires comparison, then save with a clear name and description in the appropriate folder.
4. Run the report and verify the returned records against the question. No rows may indicate filters or source data that do not match.
5. For an overview, create a dashboard and add widgets backed by suitable saved reports. Verify dashboard filters and running/view context.

Dynamic dashboards let the same dashboard show each viewer the records they are allowed to see under their Salesforce sharing and security settings. Confirm the running-user configuration and test with representative users; a dashboard does not grant access to underlying records.

## Review questions

1. What does the report type determine?
2. When would you use a cross filter?
3. Which report format compares groupings across both rows and columns?
4. What does a dashboard data widget use as its source?

<details><summary>Suggested answers</summary>

1. The primary/related records and fields that are available to the report.
2. To include or exclude parent records based on whether related child records match conditions.
3. Matrix.
4. One source report.

</details>

## Sources

- [Reports & Dashboards for Lightning Experience badge](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_reports_dashboards?trail_id=force_com_admin_beginner)
- The linked Trailhead units above.

Compiled 2026-09-28. Report builder capabilities, folder access, dashboard viewing behavior, and UI labels can change; confirm current Salesforce Help and org permissions.
