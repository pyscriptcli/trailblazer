# Salesforce Trailhead Study Notes: Lightning Experience Customization

**Badge:** [Lightning Experience Customization](https://trailhead.salesforce.com/content/learn/modules/lex_customization?trail_id=force_com_admin_beginner)  
**Level:** Foundational · Administrator  
**Trailhead estimate:** About 3 hours · 7 units

These notes summarize how an admin can make Salesforce fit users' roles and recurring work using declarative setup. A good customization reduces steps and highlights relevant information while preserving clear access and data rules.

## Units and outcomes

1. [Set Up Your Org](https://trailhead.salesforce.com/content/learn/modules/lex_customization/lex_customization_custom_objects) — build the Energy Audit example with a custom object, tab, typed fields, sample records, and feed tracking.
2. [Create and Customize Lightning Apps](https://trailhead.salesforce.com/content/learn/modules/lex_customization/lex_customization_apps) — bundle navigation items and supported tabs into a role-oriented app; configure branding and app availability.
3. [Create and Customize List Views](https://trailhead.salesforce.com/content/learn/modules/lex_customization/lex_customization_list) — create a reusable object-record list, set filters and visible columns, sort it, and optionally add a chart.
4. [Customize Record Highlights with Compact Layouts](https://trailhead.salesforce.com/content/learn/modules/lex_customization/lex_customization_compact_layouts) — select the fields users need at a glance in highlights, lookup cards, and mobile views; assign the compact layout as primary.
5. [Customize Record Page Components and Fields](https://trailhead.salesforce.com/content/learn/modules/lex_customization/lex_customization_page_layouts) — use Lightning App Builder for page structure/components and page layouts for fields/actions/related lists; activate the page for the intended audience.
6. [Create Custom Buttons and Links](https://trailhead.salesforce.com/content/learn/modules/lex_customization/lex_customization_buttons_links) — add list buttons, detail buttons, or detail links where users need them.
7. [Empower Users with Quick Actions](https://trailhead.salesforce.com/content/learn/modules/lex_customization/lex_customization_actions) — create actions tied to a record or actions available globally, and place them on the relevant layout.

## The main distinctions

| Tool or feature | What it controls |
|---|---|
| Lightning app | Navigation bundle: objects, tabs, utilities, and other supported items for a work context. |
| List view | Which records appear in a list, with filters, columns, and sorting. |
| Compact layout | The key fields shown in a record's highlights and related compact displays. |
| Lightning record page | Page structure and components, configured in Lightning App Builder. |
| Page layout | Record detail fields, related lists, buttons, links, and actions. |
| Quick action | A shortcut to create/update records or complete a task from a contextual or global surface. |

Lightning pages and page layouts work together but solve different layout problems. A page may also need activation and assignment for the correct app, record type, and audience before users see it.

## Useful design sequence

1. Ask each user group which records and tasks they use most.
2. Make the required objects/fields available, using appropriate types and required settings.
3. Organize navigation in an app and use filtered list views for repeated record subsets.
4. Put the most useful fields in highlights; use record pages and page layouts to arrange details, related records, and actions.
5. Test with the intended profile/permission context and verify that links, actions, and records are accessible to the audience.

Use public file links only when public access is intended and approved. A button or link can expose information outside the normal Salesforce access context if its target is public.

## Review questions

1. Where do you configure Lightning page components, and where do you configure related lists and page actions?
2. Which feature makes a user's repeated subset of records easy to revisit?
3. What is the difference between object-specific and global actions?
4. After creating a Lightning record page, what determines which users/app context receives it?

<details><summary>Suggested answers</summary>

1. Lightning App Builder; page layout editor.
2. A list view.
3. Object-specific actions run in a record context and can relate created records to it; global actions are available independently of a particular record.
4. Page activation and assignment, including app, record type, and profile context as applicable.

</details>

## Sources

- [Lightning Experience Customization badge](https://trailhead.salesforce.com/content/learn/modules/lex_customization?trail_id=force_com_admin_beginner)
- The linked Trailhead units above.

Compiled 2026-09-28. Setup labels and feature availability can change; check current Salesforce Help and org permissions before configuration.
