# Salesforce Trailhead Study Notes: Data Management

**Badge:** [Data Management](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_data_management?trail_id=force_com_admin_beginner)  
**Level:** Foundational · Administrator  
**Estimated time:** About 35 minutes (Import Data: 30 minutes; Export Data: 5 minutes)

These notes cover the two units on moving data into and out of Salesforce. They summarize the workflow and decision points; use Trailhead for the official hands-on challenges and the latest UI wording.

## Units

1. [Import Data](01-import-data.md)
2. [Export Data](02-export-data.md)

## Quick tool guide

| Need | Starting point |
|---|---|
| Import a smaller file into supported objects with a guided interface | Data Import Wizard |
| Import a larger volume, use an unsupported object, or automate a load | Data Loader |
| Create an org data backup archive on demand or a schedule | Data Export Service |
| Export selected data or automate the extract | Data Loader |

Treat these as starting points rather than hard guarantees: object support, row limits, features, permissions, and availability depend on the Salesforce edition and org configuration.

## Study checklist

- [ ] Choose between Data Import Wizard and Data Loader for a scenario.
- [ ] Prepare and map a CSV before importing.
- [ ] Explain add, update, and add-and-update import operations.
- [ ] Check import results and investigate failed rows.
- [ ] Compare Data Export Service and Data Loader.
- [ ] Explain why an export archive is not by itself a tested recovery plan.

Compiled 2026-09-28. Confirm edition-, permission-, and release-dependent details in the linked Salesforce sources before acting.
