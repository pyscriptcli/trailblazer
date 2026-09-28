# Lightning Email Templates in Salesforce CRM

**Type:** Article study guide with official-documentation cross-check
**Checked:** 2026-09-28
**Article updated:** SalesforceBen page reports May 11, 2026

## Summary

Lightning email templates are reusable messages for Salesforce CRM workflows. Depending on the selected template type and related record, they can include merge fields so a message is populated with record context. Salesforce supports template use in the Lightning email composer and automation scenarios such as alerts and flows, subject to the feature and configuration involved.

The SalesforceBen article is a useful walkthrough, but interface steps and feature limits can change. Use Salesforce Help as the source of truth for current behavior, permissions, and supported merge fields.

## Create and validate a template

1. Confirm that the user has the required Lightning email template and builder permissions. Current Salesforce Help lists **Access Drag-and-Drop Content Builder** for the drag-and-drop builder; availability can depend on the feature and license.
2. Open the email templates area, create a template, and choose its folder and related entity type where applicable. The related entity controls which record context and merge fields can be used.
3. Compose content, insert merge fields using Salesforce's picker, and use the builder's supported content blocks and formatting.
4. Preview with relevant record context. Send a test where available and verify that merge values resolve as expected.
5. Set folder access intentionally. Private, public, and shared-folder access have different visibility; enhanced folder sharing is an administrative option, not a blanket prerequisite.

Always use current Setup/search labels because Salesforce updates navigation. Avoid assuming every merge field works in every template type or sending context; consult the merge-field reference for that combination.

## Terms to know

- **Merge field:** A placeholder resolved from a Salesforce record or supported global value.
- **Related entity type:** The record type that supplies context for template merge fields.
- **Email Template Builder:** Salesforce's drag-and-drop template editing experience.
- **Folder sharing:** Controls which users can access templates stored in a folder.

## Review prompts

1. What record context should the template use, and does that context expose the needed fields?
2. What permission is needed for the selected editing experience?
3. How will you test both the message layout and merge-field values?
4. Who should be able to view or edit the template folder?

## Sources

- [Your Guide to Salesforce Lightning Email Templates — SalesforceBen](https://www.salesforceben.com/your-guide-to-salesforce-lightning-email-templates/)
- [Email Templates in Lightning Experience](https://help.salesforce.com/s/articleView?id=sales.email_templates_lightning_parent.htm&language=en_US&type=5)
- [Create Email Templates](https://help.salesforce.com/s/articleView?id=email_create_a_template.htm&language=en_US&type=5)
- [Merge Fields and Templates in Emails](https://help.salesforce.com/s/articleView?id=sf.access_sharing_merge_fields.htm&language=en_US&type=5)
- [Lightning Email Template Builder Guidelines](https://help.salesforce.com/s/articleView?id=sf.email_template_builder_guidelines.htm&type=5)
- [Email Template Permissions](https://help.salesforce.com/s/articleView?id=sales.email_templates_perms.htm&language=en_US&type=5)
- [HML and SML Merge Language](https://help.salesforce.com/s/articleView?id=sf.merge_fields_email_templates_lex.htm&language=en_US&type=5)

Salesforce permissions, template types, merge-field availability, and UI labels can change by release and org configuration; validate them in current Help before deployment.
