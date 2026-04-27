# Session Memory and Follow-Up Workflow

Use this reference to make the skill longitudinal across sessions.

## Core Rule

The first assessment is the baseline. Every later session must begin by retrieving that baseline and the most recent follow-up memory before offering new guidance.

Do not make the user repeat their developmental history if persistent memory is available.

## Report Display Rule

The assessment report should be shown directly in the conversation by default.

Do not default to file-only delivery.

After showing the report, ask:

`Do you want me to export this assessment to a Feishu document?`

If the user says yes and a Feishu-capable workflow or tool is available in the environment, export it. If Feishu export is unavailable, say so plainly and offer the report in a copyable structured format instead.

## Persistent Storage Location

Store longitudinal memory in:

`~/.codex/skills/human-3-development-assessor/memory/`

Use one Markdown file per person:

`<stable-identifier>.md`

Normalize the identifier into lowercase hyphen-case when practical.

Examples:

- `alice-chen.md`
- `jay-growth-log.md`
- `client-014.md`

## If No Identifier Exists

Ask once:

`Before we continue, what short name or identifier should I use so I can keep your HUMAN 3.0 assessment history consistent across sessions?`

Use that identifier for all future memory retrieval and updates.

## Consultation Startup Sequence

At the start of any session involving this skill:

1. Decide whether this looks like a first assessment or follow-up.
2. If the user provides an identifier, search memory for that identifier first.
3. If no identifier is provided but prior memory is strongly implied and recoverable from context or existing files, use the best match carefully.
4. If a matching memory file exists, read:
   - the baseline summary
   - the current active summary
   - the last 1-3 follow-up entries, depending on relevance
5. Open the conversation by briefly grounding in that memory before asking the next question.

Example grounding:

- `I reviewed your baseline assessment and your recent follow-up notes. Your recurring bottleneck has been Vocation draining Body and Spirit, and the last commitment was rebuilding sleep consistency before making bigger career moves. I'll start from there.`

## Memory File Structure

Use this structure:

```md
# HUMAN 3.0 Memory: <identifier>

## Profile
- Identifier:
- First assessment date:
- Last updated:

## Baseline Assessment
- Metatype:
- Lifestyle Archetype:
- Mind:
- Body:
- Spirit:
- Vocation:
- Core problem:
- Primary block:
- Unlock opportunity:
- Glitch stance:

## Active Summary
- Current trajectory:
- Current top problem:
- Current commitments:
- Current risks:
- Current recommended next action:

## Follow-Up Log

### <YYYY-MM-DD>
- Session type:
- What changed:
- Progress made:
- Regressions or avoidance:
- Glitch exposure or AI dependency notes:
- Updated advice:
```

Keep entries concise and retrieval-friendly. Optimize for future continuity, not literary style.

## What to Save After the First Assessment

Always save:

- identifier
- date
- Metatype
- Lifestyle Archetype
- quadrant snapshot
- core problem
- primary block
- unlock opportunity
- major false transformation flags
- active regression triggers
- Glitch guidance stance
- immediate next action
- 30-day focus

## What to Save After Follow-Ups

Always append:

- date
- whether the session was progress review, crisis, recalibration, or new assessment
- what the user actually did
- what they avoided
- what improved
- what regressed
- any change in dominant archetype or core problem
- updated immediate next action

## Proactive Memory Use

On follow-up sessions, actively weave memory into the dialogue:

- reference the original core problem
- compare claimed progress against prior commitments
- note repeated patterns without shaming
- distinguish real change from narrative inflation
- update risk if the user is moving closer to or farther from safe Glitch use

Do not merely store memory. Use it.

## Feishu Export Rule

After showing the report in chat, ask whether the user wants Feishu export.

If yes:

1. Preserve the on-screen report as the primary delivery.
2. Export the same structure, not a watered-down summary, unless the user asks for a shorter version.
3. If follow-up memory exists, optionally offer a second Feishu document mode:
   - latest assessment only
   - full longitudinal record with baseline plus follow-up timeline

## Safety and Privacy

Persistent memory may contain sensitive developmental, psychological, health, and work information.

- Keep summaries compact and relevant.
- Do not invent memory when retrieval fails.
- If uncertain about identity matching, ask before merging histories.
- If the user asks to stop memory retention, stop updating the file and say so clearly.
