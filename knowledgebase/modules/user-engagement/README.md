# Salesforce Trailhead Study Notes: User Engagement

**Badge:** [User Engagement](https://trailhead.salesforce.com/content/learn/modules/user-engagement?trail_id=force_com_admin_beginner)  
**Level:** Foundational · Administrator  
**Trailhead estimate:** About 1 hour 10 minutes · 4 units

User engagement is the work of onboarding, assisting, and teaching people inside the app. The goal is useful guidance that helps someone reach value with little interruption—not messages for their own sake.

## Units and outcomes

1. [Get Started with User Engagement](https://trailhead.salesforce.com/content/learn/modules/user-engagement/get-started-with-user-engagement) — recognize four scenarios: onboarding, feature discovery/adoption, troubleshooting help, and deeper learning; choose suitable components and push/pull delivery.
2. [Promote Feature Adoption and Discovery](https://trailhead.salesforce.com/content/learn/modules/user-engagement/promote-feature-adoption-and-discovery) — decide when a single prompt or multi-step walkthrough fits and compare floating, targeted, and docked prompts.
3. [Create Prompts in Agentforce 360 Platform](https://trailhead.salesforce.com/content/learn/modules/user-engagement/create-in-app-prompts) — use In-App Guidance to preview and configure prompts, including placement, audience, schedule, action, and trusted image URLs. The Trailhead exercise requires its sample playground packages.
4. [Design a User Engagement Journey](https://trailhead.salesforce.com/content/learn/modules/user-engagement/design-a-user-engagement-journey) — plan around an “aha” moment and use MAP (Message, Audience, Purpose) and FACE (Friendly, Accurate, Concise, Educational) to write guidance.

## Choose guidance with intent

- A **prompt** is a short, single message that points out a feature or asks for a small action.
- A **walkthrough** connects multiple prompts into a guided sequence for a procedure or related features.
- **Push** guidance appears proactively when it may help (for example, prompts, walkthroughs, empty states, or field help). **Pull** guidance is available when the user asks for it (for example, a help tooltip). A useful strategy supports both.
- Use a brief prompt for a clear, easy-to-try feature. Use a walkthrough for a sequence. Use other training or documentation when a topic needs extensive context, has many prerequisites, or is too complex for in-context help.
- Prompts can be floating, anchored to a page element (targeted), or docked. Choose placement based on the task and avoid obscuring users' work.
- Guidance settings can control where, when, how often, and for whom it appears. Keep the audience and end date/repetition rules intentional, then review whether it helped.
- Trailhead describes built-in engagement metrics such as unique viewers and completion/action rates; use them to refine content, placement, and frequency rather than assuming views alone mean the guidance worked.

## Plan a small engagement journey

1. Name the user need and the point in the workflow where help is most useful.
2. Define the **Message** (what users should learn), **Audience** (who needs it), and **Purpose** (why it helps them).
3. Choose a prompt, walkthrough, or a richer learning resource.
4. Write in FACE style and make the call to action clear.
5. Test placement and frequency with the target audience; revise or retire guidance that is no longer relevant.

Trailhead notes specific prerequisites and permissions for some prompt setup scenarios. Verify current org capabilities, licensing, package requirements, permissions, and Experience Cloud site support before applying those steps outside a Trailhead Playground.

## Review questions

1. Name the four engagement scenarios.
2. When is a walkthrough a better fit than a single prompt?
3. What do MAP and FACE stand for?
4. What is the difference between push and pull guidance?

<details><summary>Suggested answers</summary>

1. Onboarding; feature discovery/adoption; troubleshooting help; deeper learning.
2. When the user needs a multi-step guided experience or a sequence of related features.
3. Message, Audience, Purpose; Friendly, Accurate, Concise, Educational.
4. Push appears proactively; pull is opened by a user seeking help. Use both to support different needs.

</details>

## Sources

- [User Engagement badge](https://trailhead.salesforce.com/content/learn/modules/user-engagement?trail_id=force_com_admin_beginner)
- The linked Trailhead units above.

Compiled 2026-09-28. In-App Guidance labels, permissions, limits, licensing, and supported surfaces may change; verify current Salesforce documentation and org settings.
