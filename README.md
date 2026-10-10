# Forecasting Blockers

Spot project blockers early. Get a short action list. Pick up where you left off.

An AI agent skill for finding missing access, decisions, and dependencies before they stop your project. When requested, it keeps a simple local Markdown tracker for tasks, blockers, decisions, and next steps.

## What it does

- Works backward from your next milestone.
- Separates confirmed blockers, possible risks, and missing evidence.
- Batches ready human actions into practical 2–5 minute sessions when feasible.
- Gives each action prerequisites, an owner where known, what it unlocks, and a completion check.
- Saves and resumes a PROJECT.md file when you ask it to track a project.
- Keeps old notes separate from newly checked evidence.

## Install in Codex

Copy the `forecasting-blockers` folder into `~/.codex/skills/`. It should contain `SKILL.md` and `assets/PROJECT.template.md`. Compare before replacing any existing skill. The skill becomes discoverable on the next turn.

Other tools that support Markdown agent skills may use the same instructions, but their install locations and compatibility need checking. This release has not been tested across every AI tool.

## Try it

- “Use forecasting-blockers to check what could stop this project next.”
- “Give me the ready human actions I can finish in five minutes.”
- “Track this project in PROJECT.md in this folder.”
- “Resume from PROJECT.md. Check what changed before updating it.”

## Fictional example

You want a reviewer to test a new app tomorrow. Their test-account invite is missing.

The skill records the blocker, links it to the login test, and gives the administrator a ready action: invite the reviewer, then verify that sign-in works. Meanwhile, other authorized work can continue. If rollback instructions are unavailable, it labels them unverified instead of assuming they do not exist.

## The tracker

`Goal → Tasks → Blockers → Decisions → Ready actions → Next session`

The empty template is in `forecasting-blockers/assets/PROJECT.template.md`. Keep your actual PROJECT.md in your project workspace, outside this reusable skill repository. Use an existing tracker when one already exists.

## Privacy and limitations

This repository contains generic instructions and an empty template, not personal project data. It has no telemetry, server, or API key requirement. The host AI may read the files you provide; its privacy settings and model/tool costs still apply. Local storage does not mean offline AI processing.

The skill does not automatically upload project notes, monitor in the background, authorize external actions, or predict failure statistically. It does not prove receipt authenticity. Completion claims require evidence; percentages require a clear baseline. AI output can be wrong.

## Release status

Initial release. Skill structure and local file references validated; broad behavioral reliability and cross-tool compatibility are not established. Feedback with fictional or redacted examples is welcome. Never attach credentials or private project records to issues.

## License

MIT — see LICENSE.
