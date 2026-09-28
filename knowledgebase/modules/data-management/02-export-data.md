# Unit 2 — Export Data

**Estimated time:** About 5 minutes  
**Official unit:** [Trailhead: Export Data](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_data_management/lex_implementation_data_export?trail_id=force_com_admin_beginner)

## Learning goals

- Compare the Data Export Service with Data Loader.
- Start an export now or schedule one when the org supports it.
- Recognize what the export archive contains and when it is available.

## Choose an export method

| Method | Typical fit |
|---|---|
| Data Export Service | A broad Salesforce data backup, manually requested or scheduled. Produces a ZIP archive of CSV files, with options for including files and attachments. |
| Data Loader | More targeted exports and workflows that need a client app, command-line operation, or integration. |

Trailhead documents edition-dependent frequency rules: for example, weekly exports are available in Enterprise, Performance, and Unlimited, while some other editions have monthly-only options. Manual request intervals and schedule options can also vary. Check the current Data Export page in Setup and current Help for your org's exact availability.

## Data Export Service workflow

1. In Setup, search for **Data Export**.
2. Choose **Export Now** or **Schedule Export**, if available.
3. Select encoding, the data types to include, and whether files such as images, documents, and attachments should be included.
4. For integration-friendly files, consider the option to replace carriage returns with spaces.
5. For a scheduled export, set the frequency and date/time options that your org allows.
6. Start the export or save the schedule. Salesforce prepares a ZIP of CSV files and notifies the user when it is ready. Large exports may be split across files; Trailhead says download links expire after 48 hours.

## Backup practice

An export is a copy of data, not proof that the org can be recovered from it. Store the downloaded archive in an approved secure location, protect it as sensitive data, and periodically verify that the files are usable and meet retention requirements. Plan how related files and attachments are handled if they matter to recovery.

## Review questions

1. Which method is designed for a broad archive that can include files and attachments?
2. What should you do when the export notification arrives?
3. Why is downloading an export not enough to prove recoverability?

<details><summary>Suggested answers</summary>

1. Data Export Service.
2. Download the ZIP before its link expires and store it securely.
3. Recovery also depends on complete, usable files and a tested process for restoring them.

</details>

## Sources

- [Trailhead: Export Data](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_data_management/lex_implementation_data_export?trail_id=force_com_admin_beginner)
- [Salesforce Developers: Data Loader Guide](https://developer.salesforce.com/docs/platform/data-loader-impl/guide/data-loader-intro.html)
- [Salesforce Help: Export Backup Data from Salesforce](https://help.salesforce.com/s/articleView?id=sf.admin_exportdata.htm&language=en_US&type=5)

Compiled 2026-09-28. Export timing, edition support, downloadable-file retention, and available selections may change; verify current behavior in Salesforce Setup and Help.
