---
name: forecasting-blockers
description: Find project blockers and upcoming dependencies, batch ready human actions, and save or resume a simple Markdown project tracker when requested.
---

# Forecasting Blockers

Find what could stop the next milestone before it stops the work. Use the existing plan and tracker; do not create a competing system.

## Find the dependencies

- State the next milestone and the observable evidence that would prove it complete.
- Read the current plan, latest owner updates, and available evidence. State the evidence cutoff. Label missing or conflicting information unverified.
- Work backward through dependencies relevant to this project: access, owners, data, costs, credentials, devices, deployment, acceptance, and rollback. Omit unrelated categories.
- Classify each finding as a confirmed blocker, future risk, unverified dependency, or closed item. Include evidence, the affected milestone, an owner if known, the trigger or due date if known, and the smallest useful next action.
- Identify independent work that can continue within the user's existing authorization. A plan or assigned owner does not by itself authorize new external actions.

## Make human actions easy

Route technical gaps to the existing responsible owner when authorized. Reserve the human batch for things only the human can supply or decide.

For each ready action, provide:

- Exact account, device, or page and the action to take; never request secrets in chat.
- Prerequisites and whether they are ready.
- Time estimate, or unknown; aim for a 2–5 minute batch when feasible.
- What this unlocks, any expiry, and how completion will be checked.

Reuse existing item IDs. Link one answer to all dependencies it unlocks instead of counting it multiple times. Keep not-yet-ready requests separate. Time authentication close to when it can actually be used.

For a decision, state the recommended option and meaningful alternatives with their tradeoffs. Do not invent a decision when the evidence already resolves it.

## Save and resume a project

When the user requests tracking or saving, use their existing tracker. If none exists, create PROJECT.md in their chosen project folder using [the empty template](assets/PROJECT.template.md). Do not create files merely because this skill was loaded.

Keep stable task, blocker, and decision IDs. Link each blocker and decision to the task IDs it affects. Record the goal, next milestone, completion checks, evidence cutoff, owners where known, and next session actions. Leave unknown owners or dates unknown. Save only necessary project information; never store credentials or secrets.

On resume, read the latest tracker first. Distinguish saved observations from facts checked now; old notes do not establish fresh evidence. Update only relevant rows and append a short dated change note. Preserve unrelated edits. Before writing, check that the file has not changed since it was read; if it has, reread and merge rather than overwriting. Verify the saved result. If saving is unavailable, return a clearly labeled unsaved Markdown update.

Use task states todo, doing, blocked, done; blocker states confirmed, risk, unverified, closed; decision states pending, decided, applied, verified. Mark tasks done and blockers closed only when their completion evidence exists. Do not invent a percentage without an agreed baseline and counting rule.

Project files remain separate from the reusable skill. Do not commit, upload, or send them anywhere unless the user authorizes that destination. Local files may still be read by the host AI, so local storage is not a promise of offline processing or provider privacy.

## Report and recheck

Keep the report brief:

1. Milestone and evidence cutoff.
2. What blocks work now, what could block it next, and what remains unverified.
3. The ready human-action batch.
4. Authorized independent work and the next verification step.

Distinguish requested, answered, applied, and verified. Likewise, distinguish implemented, reviewed, deployed, and verified in real use. Mark an item closed only when its completion evidence exists.

Use the project's existing progress baseline. If none exists, report not baselined instead of inventing a percentage. Recheck when evidence or the plan changes. This skill does not authorize recurring monitoring, spending, messaging, or deployment.
