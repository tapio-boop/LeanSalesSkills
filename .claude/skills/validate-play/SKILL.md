---
name: validate-play
description: Validate a GTM Play for completeness and consistency. Checks that all entities are linked, required fields are populated, and identifies quality issues. Use after creating or updating a play.
argument-hint: [play-id]
allowed-tools: Read, Glob, Bash(ls:*)
---

# Validate GTM Play

## Context

Available plays:
!`ls data/gtm-plays/*/play.json 2>/dev/null || echo "No plays defined yet."`

## Instructions

1. If `$ARGUMENTS` is provided, use it to find the play. Otherwise list available plays and ask.
2. Read the play JSON and all linked entities.

### Structural Checks

Run these checks and report pass/fail:

| Check | Rule |
|-------|------|
| Play has ICP | `icp_id` references an existing ICP file |
| ICP has personas | `persona_ids` is non-empty and all IDs resolve |
| Each persona has JTBD | `jtbd_id` is set and file exists |
| Each persona has VP | `value_proposition_id` is set and file exists |
| VP references correct persona | `persona_id` matches |
| VP references correct JTBD | `jtbd_id` matches |
| JTBD references correct persona | `persona_id` matches |
| No orphaned entities | All referenced IDs exist as files |

### Completeness Checks

For each entity, check key fields are populated (not null, empty string, or empty array):

**ICP**: industry, at least one firmographic dimension, buying_triggers
**Persona**: role_title, pain_points (min 2), motivations (min 1), dmu_role
**JTBD**: job_statement, functional_job, at least 1 underserved outcome
**VP**: headline, core_message, at least 2 key_benefits, elevator_pitch_30s

### Quality Checks

| Check | What to Look For |
|-------|------------------|
| JTBD-VP alignment | Do VP benefits address JTBD underserved outcomes? |
| Persona coverage | Does the play cover at least economic-buyer and one other DMU role? |
| Objection coverage | Does the VP have responses for each persona objection? |
| Strategy consistency | Do success metrics align with the strategy type? (Enter = longer cycles, Expand = higher win rates) |

### Output

Display results as a scorecard:

```
PLAY VALIDATION: {play name}
═══════════════════════════════════════

STRUCTURAL INTEGRITY     [X/Y passed]
  ✓ Play has ICP
  ✓ ICP has 3 personas
  ✗ Persona "CTO" missing JTBD
  ...

COMPLETENESS            [X/Y passed]
  ✓ ICP firmographics complete
  ✗ Persona "CFO" has only 1 pain point (recommend 3+)
  ...

QUALITY                 [X/Y passed]
  ✓ VP benefits align with JTBD underserved outcomes
  ✗ No economic-buyer persona defined
  ...

OVERALL SCORE: X/Y (percentage%)
```

Provide specific recommendations for fixing any failures.
