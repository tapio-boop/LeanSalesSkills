---
name: show-play
description: Display a complete GTM Play with all linked entities — ICP, Buyer Personas, JTBDs, and Value Propositions. Use when the user wants to see the full details of a specific play.
argument-hint: [play-id]
allowed-tools: Read, Glob, Bash(ls:*)
---

# Show GTM Play

## Context

Available plays:
!`ls data/gtm-plays/*/play.json 2>/dev/null || echo "No plays defined yet."`

## Instructions

1. If `$ARGUMENTS` is provided, use it to find the play. Otherwise list available plays and ask.
2. Read `data/gtm-plays/{play-id}/play.json`
3. Read the linked ICP from `data/icps/{icp_id}.json`
4. For each persona ID in the ICP's `persona_ids`, read:
   - The persona from `data/personas/{persona-id}.json`
   - The linked JTBD from `data/jtbd/{jtbd-id}.json`
   - The linked Value Proposition from `data/value-propositions/{vp-id}.json`

5. Display the complete play in this format:

```
═══════════════════════════════════════════════════
GTM PLAY: {name}
Strategy: {strategy} | Status: {status}
Created: {created_at} | Updated: {updated_at}
═══════════════════════════════════════════════════

MARKET CONTEXT
  Geography: {geography}
  Industry: {industry_vertical}
  Maturity: {market_maturity}
  Competitive: {competitive_landscape_summary}

SUCCESS METRICS
  Opportunities/quarter: {target}
  Win rate: {target}%
  Avg deal size: €{target}
  Cycle length: {target} days

───────────────────────────────────────────────────
ICP: {icp name}
───────────────────────────────────────────────────
  Firmographics: {summary}
  Technographics: {summary}
  Buying triggers: {list}
  Disqualifiers: {list}
  Priority: {segment_priority}

  PERSONA 1: {persona name}
  ─────────────────────────────
  Role: {role_title} | {department} | {seniority_level}
  DMU Role: {dmu_role}
  Pain Points: {list}
  Motivations: {list}
  Objections: {list}

    JTBD: {job_statement}
    Functional: {functional_job}
    Emotional: {emotional_job}
    Social: {social_job}
    Underserved outcomes: {list with importance/satisfaction}

    VALUE PROPOSITION: {headline}
    {core_message}
    Benefits: {list with proof points}
    Differentiation: {summary}
    30s pitch: {elevator_pitch_30s}

  PERSONA 2: {persona name}
  ─────────────────────────────
  ... (same structure)
```

6. At the end, suggest relevant next actions:
   - `/validate-play {play-id}` to check completeness
   - `/expand-play`, `/acquire-play`, or `/enter-play` (based on strategy) for workflow guidance
