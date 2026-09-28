# Unit 1 — Import Data

**Estimated time:** About 30 minutes  
**Official unit:** [Trailhead: Import Data](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_data_management/lex_implementation_data_import?trail_id=force_com_admin_beginner)

## Learning goals

- Compare the Data Import Wizard and Data Loader.
- Prepare a CSV and map its columns to Salesforce fields.
- Run an import and inspect its results.

## Choose an import tool

| Tool | Typical fit | Notes from the current Trailhead unit |
|---|---|---|
| Data Import Wizard | Guided, non-automated imports to supported standard or custom objects | Trailhead describes up to 50,000 records per import. |
| Data Loader | Larger loads, objects the Wizard does not support, or repeatable/automated jobs | Trailhead describes 50,000 to 150 million records, with UI and command-line use. It can use SOAP API and can be configured for Bulk API processing. |

Limits and supported objects can depend on edition, permissions, object type, and org storage. Confirm current availability in your org before choosing a tool; for volumes beyond the documented range, consult Salesforce guidance or an experienced implementation partner.

## Prepare data first

1. Export the source data as a CSV.
2. Remove duplicates and unnecessary columns; correct inconsistent spelling and naming.
3. Compare source columns with Salesforce fields. Create fields or picklist values where required, and consider validation rules and other automation that may affect the load.
4. Test with a small sample file before loading the full dataset.

## Data Import Wizard workflow

1. In Setup, search for **Data Import Wizard** and launch it.
2. Select the standard or custom object category, then choose to add new records, update existing records, or add and update.
3. Set any matching criteria, select the CSV, and confirm its character encoding.
4. Review field mappings. The Wizard may map fields automatically; manually map required columns. **Unmapped fields are not imported.**
5. Review the import configuration and start the job.
6. Check **Bulk Data Load Jobs** in Setup and review the completion email and result files for successes and errors.

## Data behavior to remember

- Multi-select picklist values are separated by semicolons in the import file.
- Checkbox values use `1` for selected and `0` for unselected.
- Date/time values must match the expected locale-aware format.
- Formula fields are read-only and cannot receive imported values.
- Validation rules run during import; records that fail validation do not load.
- Restricted picklists can reject or default an unrecognized value; verify the target field's configuration.

## Review questions

1. Which tool is suited to a guided import of fewer than 50,000 rows into a supported object?
2. What happens to an unmapped source column in the Wizard?
3. Why run a small test import first?
4. Which separator represents multiple selected values for a multi-select picklist?

<details><summary>Suggested answers</summary>

1. Data Import Wizard, assuming the object's supported and other org limits allow the import.
2. It is not imported.
3. To validate cleanup, mapping, and configuration before processing the full dataset.
4. A semicolon.

</details>

## Sources

- [Trailhead: Import Data](https://trailhead.salesforce.com/content/learn/modules/lex_implementation_data_management/lex_implementation_data_import?trail_id=force_com_admin_beginner)
- [Salesforce Help: Salesforce Data Import](https://help.salesforce.com/s/articleView?id=xcloud.importing.htm&language=en_US&type=5)
- [Salesforce Developers: Data Loader Guide](https://developer.salesforce.com/docs/platform/data-loader-impl/guide/data-loader-intro.html)

Compiled 2026-09-28. Interface steps, import limits, edition support, and object availability may change; verify them in current Salesforce documentation and in the target org.
