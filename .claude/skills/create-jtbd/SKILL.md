---
name: create-jtbd
description: Define a Jobs-To-Be-Done for a Buyer Persona. Captures the functional, emotional, and social jobs the buyer hires a solution to do, plus underserved outcomes. Use when defining what job a persona needs done.
argument-hint: [persona-name-or-id]
allowed-tools: Read, Write, Glob, Bash(date:*)
---

# Create Jobs-To-Be-Done

## Context

Existing Personas:
!`ls data/personas/ 2>/dev/null || echo "No personas defined yet — create a persona first with /create-persona"`

Existing JTBDs:
!`ls data/jtbd/ 2>/dev/null || echo "No JTBDs defined yet."`

## Schema Reference

Read the JTBD schema from `schemas/jtbd.schema.json` for the complete field definitions.

## Instructions

Create a JTBD by gathering information through a structured conversation. If `$ARGUMENTS` is provided, use it to identify the target persona.

### Step 0: Link to Persona
- If `$ARGUMENTS` matches a persona name or ID, use it
- Otherwise list available personas and ask the user to choose
- If no personas exist, inform the user to create one first with `/create-persona`

### Step 1: Core Job Statement
Guide the user to articulate the job using this formula:

> **"When** [situation/trigger], **I want to** [motivation/action], **so I can** [expected outcome/benefit]"

Example: "When I'm planning next quarter's digital transformation roadmap, I want to quickly assess vendor capabilities against our requirements, so I can present a credible recommendation to the board with confidence."

### Step 2: Job Dimensions
- **Functional job**: The practical task they need to accomplish (the "what")
- **Emotional job**: How they want to feel — confident, in control, innovative, secure (the "feel")
- **Social job**: How they want to be perceived — as a leader, innovator, pragmatist, trusted advisor (the "appear")

### Step 3: Current State
- **Current solution**: How they get this job done today (competitor, manual process, workaround, or nothing)
- **Constraints**: Limitations on how they can get the job done (budget, time, org politics, technical debt)

### Step 4: Desired Outcomes
- **Desired outcome**: The ideal end state in their own language
- **Success criteria**: How they measure whether the job is done well (3-5 measurable criteria)

### Step 5: Underserved Outcomes
This is where the opportunity lives. For each outcome, capture:
- **Outcome**: What they want to achieve
- **Importance**: Critical, high, medium, or low
- **Current satisfaction**: Unmet, underserved, adequately-served, or overserved

Focus on outcomes rated **critical/high importance** AND **unmet/underserved** — these are the strongest opportunities to build value propositions around.

### Step 6: Generate & Save

Generate a slugified ID: `jtbd-{slug}` (e.g., `jtbd-assess-vendor-capabilities`).

Write the complete JTBD JSON to `data/jtbd/{jtbd-id}.json`.

Set `created_at` to today's date.

Also update the parent persona's `jtbd_id` field to reference this JTBD.

### Output

After saving, display the JTBD summary with special emphasis on underserved outcomes. Ask if the user wants to create a Value Proposition that addresses these underserved outcomes.

## Lean Sales Context

JTBD is the missing link between understanding WHO you sell to (ICP + Persona) and WHY they buy. In the Lean Sales method, JTBD informs the **Value Proposition Optimization Agent** (what resonates), **Discovery Agent** (what to explore in meetings), **Sales Argumentation Agent** (which outcomes to emphasize per stakeholder), and **Qualification Agent** (does the prospect actually have this job?). Without JTBD, value propositions become generic feature lists rather than outcome-oriented messages.
