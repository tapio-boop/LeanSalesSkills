---
name: acquire-play
description: Generate Acquire workflow guidance for a GTM Play targeting new customer acquisition in known markets. Produces outreach sequences, competitive displacement messaging, qualification criteria, and closing strategies. Use when the play strategy is "acquire".
argument-hint: [play-id]
allowed-tools: Read, Glob, Bash(ls:*)
---

# Acquire Workflow Guidance

## Context

Available plays:
!`ls data/gtm-plays/*/play.json 2>/dev/null || echo "No plays defined yet."`

## Reference

Read the Acquire workflow details from `Agentic_Sales_Systems_Simplified_Illustrations_v3.md` for the full workflow architecture.

## Instructions

1. If `$ARGUMENTS` is provided, use it to find the play. Otherwise list available plays and ask.
2. Read the play and all linked entities (ICP, personas, JTBDs, VPs).
3. Verify the play strategy is "acquire". If not, suggest the appropriate workflow skill.

### Generate Acquire Workflow Guidance

Based on the play data, generate execution-ready guidance for each phase:

#### Phase 1: Target Identification (Segment Strategy Agent + Prospect Intelligence Agent)

Using the ICP definition:
- **Target account criteria**: Translate ICP firmographics into actionable search criteria for prospecting tools
- **Buying signal detection**: Specific signals to monitor based on ICP behavioral triggers
- **Account prioritization framework**: Score potential targets on ICP fit + buying signal strength
- **Competitive intelligence needs**: What to research about incumbent vendors at target accounts

#### Phase 2: Outreach Strategy (Outreach Automation Agent)

For each persona in the play:
- **Personalized outreach sequence**: Multi-touch sequence (email, LinkedIn, phone) with timing
- **First-touch messaging**: Using the VP email hook, craft opening messages per persona
- **Follow-up cadence**: Sequence of 5-7 touches with escalating value delivery
- **Channel strategy**: Which channels to use for each persona based on communication preferences
- **A/B test suggestions**: Message variations to test

#### Phase 3: Discovery & Qualification (Discovery Agent + Qualification Agent)

Using personas and JTBDs:
- **Discovery question framework**: 8-10 questions per persona that uncover JTBD fit, organized by:
  - Situation questions (current state)
  - Problem questions (pain and impact)
  - Implication questions (cost of inaction)
  - Need-payoff questions (desired outcome)
- **DMU mapping checklist**: Identify which personas are present, their relationships, and the buying process
- **Qualification scorecard**: Go/no-go criteria specific to this play's ICP and success metrics
- **Competitive assessment**: Key questions to understand incumbent satisfaction and switching barriers

#### Phase 4: Value Delivery & Closing (Value Selling + Sales Argumentation + Proposal Generation + Deal Acceleration)

Using value propositions:
- **Stakeholder-specific value arguments**: Per persona, mapped to their JTBD underserved outcomes
- **Competitive displacement messaging**: Why switch from current solution, addressing switching costs and risks
- **Business case framework**: ROI calculation template using VP quantifications
- **Proposal structure**: Recommended sections based on personas and their priorities
- **Closing strategy**: Decision criteria, timeline management, urgency creation tied to buying triggers

### Output Format

Present the guidance as a complete acquisition playbook with:
- Target account scoring template
- Per-persona outreach sequences with actual message drafts
- Discovery question sets organized by persona
- Value argument matrix (persona x benefit x proof)
- Competitive battle card structure
- Qualification scorecard

## Lean Sales Context

The Acquire workflow in the Lean Sales method involves 12 agents working together to systematically win new customers. It follows the Opportunity Generation Engine flow: Market Intelligence → Segment Strategy → Prospect Intelligence → Outreach → Discovery → Qualification → Value Selling → Argumentation → Proposal → Deal Acceleration. The constraint-based flow control ensures the pipeline doesn't get overloaded — the Qualification Agent adjusts thresholds based on capacity, and the Lead Nurturing Agent serves as a buffer for not-yet-ready prospects.
