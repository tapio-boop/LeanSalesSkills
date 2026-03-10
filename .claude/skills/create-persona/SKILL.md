---
name: create-persona
description: Create a Buyer Persona linked to an ICP, including role, pain points, motivations, DMU role, and communication preferences. Use when the user wants to define who they sell to within an ICP.
argument-hint: [persona-name]
allowed-tools: Read, Write, Glob, Bash(date:*)
---

# Create Buyer Persona

## Context

Existing ICPs:
!`ls data/icps/ 2>/dev/null || echo "No ICPs defined yet — create an ICP first with /create-icp"`

Existing Personas:
!`ls data/personas/ 2>/dev/null || echo "No personas defined yet."`

## Schema Reference

Read the persona schema from `schemas/persona.schema.json` for the complete field definitions.

## Instructions

Create a Buyer Persona by gathering information through a structured conversation. If `$ARGUMENTS` is provided, use it as the persona name.

### Step 0: Link to ICP
- If only one ICP exists, confirm using it
- If multiple ICPs exist, ask the user to choose
- If no ICPs exist, inform the user to create one first with `/create-icp`

### Step 1: Role Identity
- **Name**: Descriptive persona name (e.g., "The Digital Transformation CTO")
- **Role title**: Typical job title
- **Department**: Function area
- **Seniority level**: c-level, vp, director, manager, or individual-contributor
- **DMU role**: Their role in the Decision Making Unit:
  - **Economic buyer**: Controls the budget, makes final purchase decision
  - **Technical evaluator**: Assesses technical fit and feasibility
  - **User buyer**: Will use the solution day-to-day
  - **Coach**: Internal champion who guides you through the organization
  - **Blocker**: May resist or obstruct the purchase
  - **Influencer**: Shapes opinions but doesn't decide

### Step 2: Psychology
- **Pain points**: Top 3-5 problems and frustrations they face
- **Motivations**: What drives their decisions (career, efficiency, innovation, risk reduction)
- **Success metrics**: KPIs they are measured on
- **Objections**: Common concerns they raise during sales process

### Step 3: Communication Preferences
- **Preferred channels**: Email, LinkedIn, phone, in-person, etc.
- **Content format**: Executive-summary, detailed-analysis, visual, or data-driven
- **Tone**: Strategic, technical, practical, or financial
- **Meeting preference**: Brief (15-20 min), standard (30-45 min), or deep-dive (60+ min)
- **Information sources**: Where they get industry information (publications, events, peers)

### Step 4: Generate & Save

Generate a slugified ID: `persona-{slug}` (e.g., `persona-digital-transformation-cto`).

Write the complete persona JSON to `data/personas/{persona-id}.json`.

Set `created_at` to today's date. Leave `jtbd_id` and `value_proposition_id` empty — they will be linked when created.

Also update the parent ICP's `persona_ids` array to include this new persona ID.

### Output

After saving, display a summary of the persona and confirm the file location. Ask if the user wants to create a Jobs-To-Be-Done for this persona.

## Lean Sales Context

Buyer Personas bridge the gap between company-level targeting (ICP) and individual-level engagement. In the Lean Sales method, personas inform the **Outreach Automation Agent** (channel preferences), **Discovery Agent** (pain points, motivations), **Sales Argumentation Agent** (stakeholder-specific messaging), and **Value Selling Agent** (success metrics for ROI). Each persona within an ICP may have completely different pain points and communication needs.
