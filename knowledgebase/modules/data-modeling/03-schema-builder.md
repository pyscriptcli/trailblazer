# Unit 3 — Work with Schema Builder

**Estimated time:** 15 minutes  
**Official unit:** [Trailhead](https://trailhead.salesforce.com/content/learn/modules/data_modeling/schema_builder)

## Learning goals

- Explain how Schema Builder helps with data modeling.
- View an object model and create objects and fields in the visual tool.

## Core ideas

Schema Builder is a visual workspace for seeing and editing objects, fields, and relationships. It helps people understand a model and discuss how information flows. Moving objects around the canvas changes their layout for viewing; it does not change the underlying data model.

## View a schema

1. In Setup, use Quick Find to open **Schema Builder**.
2. In the left panel, choose **Clear All**.
3. Select the objects to inspect, such as Contact, Favorite, Offer, and Property.
4. Choose **Auto-Layout** to arrange them on the canvas.
5. Drag cards to make the diagram easier to read or explain.

## Create an object visually

1. In the left sidebar, open **Elements**.
2. Drag **Object** onto the canvas.
3. Enter the object's settings and save.

## Create a field visually

1. From **Elements**, choose a field type and drag it onto the target object.
2. Complete the field settings, such as label, name, and required behavior.
3. Save. Relationship, formula, and ordinary fields can be added this way.
4. Confirm the object or field also appears in Object Manager.

## Hands-on challenge reminder

The Trailhead challenge asks you to add a required Street Address field to Property using Schema Builder. Follow the current challenge's exact field-type and naming requirements in Trailhead, because challenge validators can be sensitive to the chosen type and API name.

## Check your understanding

1. What problem does Schema Builder help solve?
2. Does rearranging object cards change the actual schema?
3. Where do you drag an object from when creating one visually?
4. After creating a field in Schema Builder, where can you verify it?

<details><summary>Suggested answers</summary>

1. It provides a visual way to inspect, explain, and edit the data model.
2. No, canvas positioning is only a visualization change.
3. The Elements tab in the left sidebar.
4. In Object Manager, under the object’s fields.

</details>
