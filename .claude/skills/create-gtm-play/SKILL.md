---
name: create-gtm-play
description: Create a complete GTM Play — the foundational construct combining Strategy (expand/acquire/enter), ICP, Buyer Personas, JTBD, and Value Propositions. This is the orchestrator skill that walks through the full play creation flow.
argument-hint: [play-name]
allowed-tools: Read, Write, Glob, Bash(date:*)
---

# Create GTM Play

## Context

Existing GTM Plays:
!`ls data/gtm-plays/ 2>/dev/null || echo "No plays defined yet."`

Existing ICPs:
!`ls data/icps/ 2>/dev/null || echo "No ICPs defined yet."`

## Schema Reference

Read schemas from `schemas/` directory for complete field definitions:
- `schemas/gtm-play.schema.json`
- `schemas/icp.schema.json`
- `schemas/persona.schema.json`
- `schemas/jtbd.schema.json`
- `schemas/value-proposition.schema.json`

## Instructions

Create a complete GTM Play by walking the user through each layer. If `$ARGUMENTS` is provided, use it as the play name.

A GTM Play is the foundational construct of the Lean Sales method — it binds together WHO you sell to, WHAT job they need done, and WHY they should buy from you, within a specific strategic motion.

### Step 1: Strategy Selection

Ask the user to choose the GTM motion:

| Strategy | When to Use | Key Characteristics |
|----------|-------------|---------------------|
| **Expand** | Growing existing customer accounts | Known relationships, proven value, lower risk. Focus: whitespace analysis, upsell/cross-sell, account planning |
| **Acquire** | Winning new customers in known markets | Brand awareness exists, references available, validated ICP. Focus: competitive displacement, outreach sequences |
| **Enter** | Penetrating new markets | Limited brand awareness, hypothesis ICP, longer cycles. Focus: beachhead strategy, lighthouse accounts, validation |

### Step 2: Market Context

Gather:
- **Geography**: Target regions
- **Industry vertical**: Primary industry
- **Market maturity**: Emerging, growing, mature, or declining
- **Competitive landscape**: Brief overview of key competitors and positioning

### Step 3: Success Metrics

Define targets:
- **Opportunities per quarter**: How many qualified opportunities?
- **Win rate**: Target conversion rate
- **Deal size (EUR)**: Average expected deal value
- **Cycle length (days)**: Expected sales cycle duration

### Step 4: ICP

Either **link to an existing ICP** or **create a new one**:

If creating new, walk through the full ICP definition (firmographics, technographics, behavioral signals) following the same flow as `/create-icp`. Write to `data/icps/{icp-id}.json`.

### Step 5: Buyer Personas (1 or more)

For each persona within this ICP, walk through:
- Role identity (title, department, seniority, DMU role)
- Psychology (pain points, motivations, success metrics, objections)
- Communication preferences

Write each to `data/personas/{persona-id}.json`. Update the ICP's `persona_ids`.

Ask if they want to add another persona. Most plays have 2-4 personas.

### Step 6: JTBD (one per persona)

For each persona, define their Job-To-Be-Done:
- Core job statement: "When [situation], I want to [motivation], so I can [outcome]"
- Functional, emotional, and social dimensions
- Current solution and constraints
- Underserved outcomes (the opportunity)

Write each to `data/jtbd/{jtbd-id}.json`. Update each persona's `jtbd_id`.

### Step 7: Value Propositions (one per persona)

For each persona + JTBD pair, craft:
- Headline and core message
- Key benefits with proof points (mapped to underserved outcomes)
- Differentiation (vs. status quo, vs. competitors, unique mechanism)
- Objection responses
- Elevator pitches (30s and 60s)
- Email hook

Write each to `data/value-propositions/{vp-id}.json`. Update each persona's `value_proposition_id`.

### Step 8: Assemble Play

Create the play directory and play.json:

```
data/gtm-plays/{play-id}/play.json
```

The play JSON links all entities by ID. Set `status` to "draft" and `created_at` to today.

### Step 9: Summary

Display the complete play as a structured overview:

```
GTM Play: {name}
Strategy: {strategy}
Status: draft

ICP: {icp name}
  Industry: {industries}
  Company size: {employee range}
  Revenue: {revenue range}

Personas:
  1. {persona name} ({role_title}, {dmu_role})
     JTBD: {job_statement}
     VP: {headline}

  2. {persona name} ({role_title}, {dmu_role})
     JTBD: {job_statement}
     VP: {headline}

Success Metrics:
  Opportunities/quarter: {target}
  Win rate: {target}
  Avg deal size: €{target}
  Cycle length: {target} days
```

Suggest the user run `/validate-play` to check completeness, or the appropriate workflow skill (`/expand-play`, `/acquire-play`, `/enter-play`) to generate execution guidance.

## Lean Sales Context

The GTM Play is the unit of strategic execution in the Lean Sales method. It connects the Strategy Layer (what the Segment Strategy Agent and Value Proposition Optimization Agent define) to the Execution Layer (what Outreach, Discovery, Qualification, and other agents execute). A complete play ensures every agent in the system has the context it needs to operate effectively, eliminating the waste of generic, untargeted sales activity.
