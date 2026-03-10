---
name: create-icp
description: Define an Ideal Customer Profile (ICP) with firmographic, technographic, and behavioral attributes. Use when the user wants to create or define a new ICP for targeting.
argument-hint: [icp-name]
allowed-tools: Read, Write, Glob, Bash(date:*)
---

# Create Ideal Customer Profile

## Context

Existing ICPs:
!`ls data/icps/ 2>/dev/null || echo "No ICPs defined yet."`

Existing Personas:
!`ls data/personas/ 2>/dev/null || echo "No personas defined yet."`

## Schema Reference

Read the ICP schema from `schemas/icp.schema.json` for the complete field definitions.

## Instructions

Create an ICP by gathering the following information from the user through a structured conversation. If `$ARGUMENTS` is provided, use it as the ICP name.

### Step 1: Identity
- **Name**: Descriptive name for this ICP (e.g., "Mid-market Nordic Manufacturers")
- **Description**: 1-2 sentence summary of who this ICP represents
- **Segment Priority**: primary, secondary, or experimental

### Step 2: Firmographics
- **Industry**: Target industries (can be multiple)
- **Employee count**: Min and max range
- **Revenue (EUR)**: Min and max range
- **Geography**: Target regions/countries
- **Company type**: Private, public, PE-backed, family-owned, etc.

### Step 3: Technographics
- **Tech stack**: Relevant technologies (what they currently use)
- **Digital maturity**: Low, medium, or high
- **Key systems**: ERP, CRM, or other critical systems

### Step 4: Behavioral Signals
- **Buying triggers**: Events that signal buying intent (e.g., new CTO hired, funding round, contract renewal)
- **Disqualifiers**: Red flags that disqualify a prospect
- **Typical buying cycle**: Length in days

### Step 5: Generate & Save

Generate a slugified ID: `icp-{slug}` (e.g., `icp-midmarket-nordic-manufacturers`).

Write the complete ICP JSON to `data/icps/{icp-id}.json`.

Set `created_at` to today's date. Leave `persona_ids` as an empty array — personas will be linked later.

### Output

After saving, display a summary table of the ICP and confirm the file location. Ask if the user wants to create Buyer Personas for this ICP.

## Lean Sales Context

In the Lean Sales method, ICPs are defined by the **Segment Strategy Agent** in the Strategy Layer. They serve as the foundation for all downstream targeting — every Buyer Persona, JTBD, and Value Proposition connects back to an ICP. A well-defined ICP eliminates waste by ensuring the sales system only pursues prospects with genuine fit.
