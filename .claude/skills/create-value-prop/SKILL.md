---
name: create-value-prop
description: Craft a Value Proposition tailored to a specific Buyer Persona and their JTBD. Generates headline, core message, benefits with proof points, differentiation, objection responses, and elevator pitches. Use when building messaging for a persona.
argument-hint: [persona-name-or-id]
allowed-tools: Read, Write, Glob, Bash(date:*)
---

# Create Value Proposition

## Context

Existing Personas:
!`ls data/personas/ 2>/dev/null || echo "No personas defined yet."`

Existing JTBDs:
!`ls data/jtbd/ 2>/dev/null || echo "No JTBDs defined yet — create a JTBD first with /create-jtbd"`

Existing Value Propositions:
!`ls data/value-propositions/ 2>/dev/null || echo "No value propositions defined yet."`

## Schema Reference

Read the value proposition schema from `schemas/value-proposition.schema.json` for the complete field definitions.

## Instructions

Create a Value Proposition by gathering information and then generating tailored messaging. If `$ARGUMENTS` is provided, use it to identify the target persona.

### Step 0: Link to Persona + JTBD
- Identify the target persona (from `$ARGUMENTS` or by listing available personas)
- Read the persona's JSON to understand their pain points, motivations, and communication preferences
- Read the linked JTBD to understand the job, desired outcomes, and underserved outcomes
- Also read the parent ICP for firmographic context
- If no persona or JTBD exists, inform the user to create them first

### Step 1: Value Proposition Core
Work with the user to define:
- **Headline**: One powerful line that captures the core value (speak to the persona's language and JTBD)
- **Subheadline**: Supporting statement that elaborates
- **Core message**: 2-3 sentences connecting the persona's pain to the solution's outcome

The core message should follow this structure:
> [Persona's situation/pain] → [How we uniquely solve it] → [Outcome they care about]

### Step 2: Key Benefits (3-5)
For each benefit, capture:
- **Benefit**: What the persona gains (tied to JTBD underserved outcomes)
- **Proof point**: Evidence — customer example, case study, data point
- **Quantification**: Measurable impact (%, time saved, revenue gained)

Prioritize benefits that map to **underserved outcomes** from the JTBD.

### Step 3: Differentiation
- **vs. Status Quo**: Why change from what they're doing now? (addresses inertia)
- **vs. Competitors**: Why choose us over alternatives? (addresses comparison)
- **Unique mechanism**: What makes our approach uniquely effective? (the "how" that's different)

### Step 4: Objection Responses
Based on the persona's known objections, craft concise responses:
- Each response should acknowledge the concern, reframe, and provide evidence

### Step 5: Elevator Pitches
Generate two versions:
- **30-second**: For brief introductions — problem, solution, outcome in 3 sentences
- **60-second**: For more detailed conversations — adds proof point and call to action

### Step 6: Email Hook
A compelling opening line for outreach emails that:
- References the persona's world (not yours)
- Hints at the underserved outcome
- Creates curiosity without being clickbait

### Step 7: Generate & Save

Generate a slugified ID: `vp-{slug}` (e.g., `vp-cto-vendor-assessment`).

Write the complete Value Proposition JSON to `data/value-propositions/{vp-id}.json`.

Set `created_at` to today's date. Set `status` to "draft".

Also update the parent persona's `value_proposition_id` field to reference this VP.

### Output

After saving, display the complete value proposition in a readable format, organized by section. Highlight how each benefit maps to JTBD underserved outcomes.

## Lean Sales Context

In the Lean Sales method, Value Propositions are managed by the **Value Proposition Optimization Agent** and consumed by nearly every execution agent: **Outreach Automation** (email hooks, messaging), **Sales Argumentation** (stakeholder-specific arguments), **Value Selling** (ROI and business case), **Proposal Generation** (proposal messaging), and **Sales Content** (collateral). A well-crafted VP tied to persona + JTBD eliminates waste by ensuring every customer touchpoint delivers relevant, outcome-oriented messaging rather than generic feature talk.
