---
name: expand-play
description: Generate Expand workflow guidance for a GTM Play targeting existing customer growth. Produces account planning priorities, discovery questions, expansion opportunity identification, and upsell/cross-sell value arguments. Use when the play strategy is "expand".
argument-hint: [play-id]
allowed-tools: Read, Glob, Bash(ls:*)
---

# Expand Workflow Guidance

## Context

Available plays:
!`ls data/gtm-plays/*/play.json 2>/dev/null || echo "No plays defined yet."`

## Reference

Read the Expand workflow details from `Agentic_Sales_Systems_Simplified_Illustrations_v3.md` for the full workflow architecture.

## Instructions

1. If `$ARGUMENTS` is provided, use it to find the play. Otherwise list available plays and ask.
2. Read the play and all linked entities (ICP, personas, JTBDs, VPs).
3. Verify the play strategy is "expand". If not, suggest the appropriate workflow skill.

### Generate Expand Workflow Guidance

Based on the play data, generate execution-ready guidance for each phase:

#### Phase 1: Account Analysis (Account Planning Agent)

Using the ICP and current customer base context:
- **Whitespace analysis framework**: Map which offerings/solutions the customer uses vs. what else from the portfolio could apply
- **Growth signal indicators**: Based on ICP behavioral signals, what triggers indicate expansion readiness in existing accounts
- **Account health criteria**: Red/yellow/green indicators for account expansion readiness

#### Phase 2: Stakeholder Expansion (Prospect Intelligence Agent + Discovery Agent)

Using the personas defined in the play:
- **New stakeholder targets**: Which personas in the ICP are not yet engaged? Generate a stakeholder mapping plan
- **Discovery questions**: For each persona, generate 5-7 discovery questions tailored to their JTBD and pain points
- **Cross-department entry strategy**: How to expand from current department to new departments

#### Phase 3: Value Expansion (Value Selling Agent + Sales Argumentation Agent)

Using the value propositions and JTBDs:
- **Upsell arguments**: For each persona, craft arguments for deeper adoption tied to their underserved outcomes
- **Cross-sell arguments**: How adjacent offerings solve related jobs for different personas
- **ROI reinforcement**: Use existing success metrics to build expansion business case
- **Reference leverage**: How to use the existing relationship as proof for new stakeholders

#### Phase 4: Opportunity Qualification (Qualification Agent)

- **Expansion qualification criteria**: Specific go/no-go factors for expansion opportunities
- **Priority scoring**: How to rank expansion opportunities across the account portfolio
- **Resource allocation guidance**: How much effort to invest based on expansion potential

### Output Format

Present the guidance organized by phase with specific, actionable items. Include:
- Per-persona discovery question sets
- Stakeholder-specific value arguments
- A suggested expansion sequence (which persona to approach first, second, etc.)
- Key metrics to track

## Lean Sales Context

The Expand workflow is the highest-ROI motion in the Lean Sales method — existing customers have proven need, established trust, and shorter cycles. The workflow leverages the Account Planning Agent, Discovery Agent, Value Selling Agent, and Sales Argumentation Agent working together. The Expand workflow from the Agentic Sales System shows how 12 agents collaborate to systematically identify and capture growth opportunities within the existing customer base.
