# Unit 2 — Create Object Relationships

**Estimated time:** 15 minutes  
**Official unit:** [Trailhead](https://trailhead.salesforce.com/content/learn/modules/data_modeling/object_relationships)

## Learning goals

- Describe lookup, master-detail, and hierarchical relationships.
- Create a lookup and master-detail field.

## Core ideas

A relationship is a special field that connects records across objects. Standard relationships already connect common Salesforce records; for example, an Account can show its related Contacts. Admins can also define custom relationships for their own objects.

| Relationship | How it behaves | Typical fit |
|---|---|---|
| Lookup | Links records while the related records generally remain independent. Can represent one-to-one or one-to-many patterns. | Optional or looser association, such as a contact that may or may not be tied to an account. |
| Master-detail | The detail depends on its master; the master controls important behavior such as access and deletion. Deleting a master can delete related detail records. The relationship field is created on the detail object. | A child record that has no useful life without its parent, such as Favorite records belonging to a Property. |
| Hierarchical | A special lookup available only on User. | User reporting/management chains. |

Choose deliberately: relationships make data more useful, but they also add dependencies. Consider what happens to access and related records if a record or field changes or is deleted.

## Hands-on walkthrough: Favorite, Contact, and Property

### Create Favorite

1. In Object Manager, choose **Create → Custom Object**.
2. Set label **Favorite**, plural label **Favorites**, enable the custom tab wizard, and save.
3. Choose a tab style and finish the wizard.

### Link Favorite to Contact with a lookup

1. Open Favorite → **Fields & Relationships** → **New**.
2. Choose **Lookup Relationship** and continue.
3. Set **Related To** to **Contact**. Use **Contact** as the field name and save through the wizard.

### Link Favorite to Property with master-detail

1. On Favorite → **Fields & Relationships**, choose **New**.
2. Select **Master-Detail Relationship** and continue.
3. Set **Related To** to **Property**; use **Property** as the field name and save.
4. Open a Property record and inspect its Related tab. Favorites should appear as related records.

### Add a Favorite record

Open the Sales app, select a Property, use its Related tab to create a Favorite, give it a name, and save.

## Check your understanding

1. Which relationship should you consider when the child cannot stand alone and should be deleted with the parent?
2. On which object is a master-detail relationship field created?
3. Can a hierarchical relationship be added to any custom object?
4. What design question should you ask before deleting a master record?

<details><summary>Suggested answers</summary>

1. Master-detail.
2. The detail (child) object.
3. No. It is a special lookup available only on User.
4. Whether its dependent detail records should also be removed, along with the effect on users/access.

</details>
