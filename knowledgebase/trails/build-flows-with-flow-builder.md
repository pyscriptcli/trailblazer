# Build Flows with Flow Builder

**Type:** Trailhead trail study guide
**Checked:** 2026-09-28
**Audience:** Salesforce admins, intermediate

## What this trail covers

The trail is an approximately 12-hour, eight-badge progression through declarative automation. Flow Builder lets an administrator define a sequence of steps and decisions that runs when a user interacts with it, a record changes, or a schedule is reached. The trail progresses from the builder and variables to record access, actions, branching, triggered and scheduled automation, screens, collection transforms, and loops.

## Learning map

1. [Flow Builder Basics](https://trailhead.salesforce.com/content/learn/modules/flow-basics) introduces business process automation, the builder canvas, and flow variables.
2. [Data and Actions in Flows](https://trailhead.salesforce.com/content/learn/modules/data-and-actions-in-flows) covers working with Salesforce records, variables, action elements, and global values.
3. [Flow Builder Logic](https://trailhead.salesforce.com/content/learn/modules/flow-build-logic) develops branching, assignments, formulas, subflows, and element ordering.
4. [Record-Triggered Flows](https://trailhead.salesforce.com/content/learn/modules/record-triggered-flows) covers record-change entry conditions, actions, scheduled paths, and trigger ordering.
5. [Autolaunched and Scheduled Flows](https://trailhead.salesforce.com/content/learn/modules/autolaunched-scheduled-flows) covers flows without screens, invocation from automation or buttons, and time-based starts.
6. [Screen Flows](https://trailhead.salesforce.com/content/learn/modules/screen-flows) introduces user-facing flow screens and interactions.
7. [Multirecord Elements and Transforms in Flows](https://trailhead.salesforce.com/content/learn/modules/multirecord-elements-and-transforms-in-flows) organizes and transforms collections of records.
8. [Loops in Flow Builder](https://trailhead.salesforce.com/content/learn/modules/loops-in-flow-builder) iterates through collection items to perform repeated logic.

Trailhead can revise badge names, ordering, and durations. The [trail overview](https://trailhead.salesforce.com/content/learn/trails/build-flows-with-flow-builder) is the canonical current curriculum.

## Practical way to design a flow

1. State the business outcome and identify what starts the automation: a user opening a screen, a record event, an explicit invocation, or a schedule.
2. Define entry conditions narrowly and decide which records and fields the flow needs.
3. Sketch the paths and outcomes before adding elements. Use decisions for branching, assignments/formulas for values, and actions for operations.
4. Choose a screen flow when the process needs user input or display; use a background flow when it should run without an interactive session.
5. For multiple records, work with collections and transforms; add a loop only when each item needs individual logic.
6. Test representative paths, including boundary conditions and failure outcomes, then activate only after reviewing the flow and its effects.

## Terms to know

- **Element:** A step on the flow canvas, such as a decision, assignment, screen, or action.
- **Resource:** A variable, formula, constant, or other value a flow can reference.
- **Collection:** A variable holding multiple values or records.
- **Record-triggered flow:** Automation that starts in response to a record event.
- **Autolaunched flow:** A background flow with no screen interaction, started by another process or invocation.
- **Subflow:** A reusable flow called by another flow.

## Review prompts

1. Which start type best fits the process, and what should its entry criteria be?
2. What state belongs in a variable, and what data can be obtained directly from the triggering context?
3. Where should the flow branch, and what should happen when no branch matches?
4. Is the data one record or a collection? Does the collection require a transform or per-item loop?
5. Which success and failure cases must be tested before activation?

## Sources

- [Build Flows with Flow Builder — Trailhead](https://trailhead.salesforce.com/content/learn/trails/build-flows-with-flow-builder)
- [Flow Builder Basics](https://trailhead.salesforce.com/content/learn/modules/flow-basics)
- [Data and Actions in Flows](https://trailhead.salesforce.com/content/learn/modules/data-and-actions-in-flows)
- [Flow Builder Logic](https://trailhead.salesforce.com/content/learn/modules/flow-build-logic)
- [Record-Triggered Flows](https://trailhead.salesforce.com/content/learn/modules/record-triggered-flows)
- [Autolaunched and Scheduled Flows](https://trailhead.salesforce.com/content/learn/modules/autolaunched-scheduled-flows)
- [Screen Flows](https://trailhead.salesforce.com/content/learn/modules/screen-flows)
- [Multirecord Elements and Transforms in Flows](https://trailhead.salesforce.com/content/learn/modules/multirecord-elements-and-transforms-in-flows)
- [Loops in Flow Builder](https://trailhead.salesforce.com/content/learn/modules/loops-in-flow-builder)
