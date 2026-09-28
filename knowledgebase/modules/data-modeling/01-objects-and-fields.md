# Unit 1 — Optimize Customer Data with Standard and Custom Objects

**Estimated time:** 15 minutes  
**Official unit:** [Trailhead](https://trailhead.salesforce.com/content/learn/modules/data_modeling/objects_intro)

## Learning goals

- Explain why Salesforce objects are useful.
- Distinguish standard objects from custom objects.
- Recognize common field categories and data types.

## Core ideas

Salesforce presents database structure in terms that are easier to work with: an object holds a kind of information, its fields describe the information, and each record is one instance. For example, a Property object could have Address and Price fields, with one record for each home. Together, objects and fields form an app's data model.

Salesforce includes standard objects for common business concepts, such as Account, Contact, Lead, and Opportunity. When a business needs a concept that does not fit a standard object, an admin can create a custom object. The DreamHouse example uses a custom Property object to track homes for sale. Creating an object also gives Salesforce metadata and user-interface structure, such as a record page layout.

### Field categories

| Category | Purpose | Example |
|---|---|---|
| Identity | System-generated record identifier | Record ID |
| System | Read-only record history/metadata | CreatedDate, LastModifiedDate |
| Name | Human-readable or automatically numbered record name | Julie Bean; CA-1024 |
| Custom | A field added to fit a business need | Birthday, Price |

Every field has a data type. Choose one that matches the value: Checkbox for yes/no, Date or DateTime for time values, Currency for money, and Formula for a calculated result. A custom field's API name commonly ends in `__c` (for example, `Price__c`).

## Hands-on walkthrough: Property and Price

1. Create a fresh Trailhead Playground for the module and launch it.
2. Open Setup, then Object Manager, then choose **Create → Custom Object**.
3. Set the label to **Property** and plural label to **Properties**. Keep the other defaults.
4. Select **Launch New Custom Tab Wizard after saving**, save, choose a tab style, then finish the wizard.
5. In Object Manager, open Property → **Fields & Relationships** → **New**.
6. Choose **Currency**. Set the field label to **Price**, add a helpful description, and mark it required if every property must have a price.
7. Save the field. Confirm the API name is `Price__c`.
8. In the Sales app, open the Properties tab, create a record, enter its name and price, and save.

## Design reminders

- Use specific, unique names for objects and fields so users can tell them apart.
- Add descriptions; use help text for fields whose purpose may not be obvious.
- Require a value only when records are genuinely incomplete without it.
- Think through what you need to store before choosing a field type.

## Check your understanding

1. In the spreadsheet analogy, what do an object, field, and record correspond to?
2. Why might a business create a custom object instead of reusing a standard one?
3. Which field type fits a yes/no value? Which fits a calculated commission?
4. What does the `__c` suffix indicate?

<details><summary>Suggested answers</summary>

1. Table, column, and row.
2. To represent a business-specific concept not covered by a suitable standard object.
3. Checkbox; Formula.
4. It identifies a custom field's API name.

</details>
