---
name: enter-play
description: Generate Enter workflow guidance for a GTM Play targeting new market penetration. Produces beachhead strategy, lighthouse account targeting, hypothesis validation plan, and pilot program structure. Use when the play strategy is "enter".
argument-hint: [play-id]
allowed-tools: Read, Glob, Bash(ls:*)
---

# Enter Workflow Guidance

## Context

Available plays:
!`ls data/gtm-plays/*/play.json 2>/dev/null || echo "No plays defined yet."`

## Reference

Read the Enter workflow details from `Agentic_Sales_Systems_Simplified_Illustrations_v3.md` for the full workflow architecture including the healthcare market entry example.

## Instructions

1. If `$ARGUMENTS` is provided, use it to find the play. Otherwise list available plays and ask.
2. Read the play and all linked entities (ICP, personas, JTBDs, VPs).
3. Verify the play strategy is "enter". If not, suggest the appropriate workflow skill.

### Key Differences: Enter vs. Acquire

| Aspect | Acquire | Enter |
|--------|---------|-------|
| Brand awareness | Known in market | Unknown or limited |
| References | Have relevant case studies | May lack segment-specific proof |
| ICP confidence | Validated | Hypothesis to test |
| Sales cycle | Predictable | Longer, more uncertain |
| Competitive position | Understood | Learning |

The Enter play must account for these differences with hypothesis-driven approaches and validation loops.

### Generate Enter Workflow Guidance

Based on the play data, generate execution-ready guidance for each phase:

#### Phase 1: Market Analysis & Beachhead Strategy (Strategic Market Intelligence + Segment Strategy)

Using the play's market context and ICP (treated as hypothesis):
- **Market sizing**: Framework to validate the addressable opportunity
- **Competitive landscape map**: Who are the incumbents? What are their strengths/weaknesses?
- **Entry barrier assessment**: Technical, regulatory, relationship, and brand barriers
- **Beachhead segment definition**: The specific narrow sub-segment to start with and why
- **ICP hypothesis validation plan**: What evidence would confirm or refute the hypothesis ICP? Define specific experiments

#### Phase 2: Value Proposition Adaptation (Value Proposition Optimization + Offering Configuration)

Using the VPs (treated as hypothesis messaging):
- **Message adaptation**: How existing value props need to change for the new market
- **Proof point substitutes**: Adjacent references and analogies when direct case studies don't exist
- **Hypothesis messaging to test**: 3-4 message variations to validate with early prospects
- **Entry offering structure**: Pilot/POC program that reduces buyer risk:
  - Scope and duration
  - Pricing (penetration vs. premium)
  - Success metrics defined upfront
  - Reference commitment (lighthouse customers agree to be references if successful)

#### Phase 3: Lighthouse Account Targeting (Prospect Intelligence + Outreach Automation)

Using the hypothesis ICP and personas:
- **Lighthouse account criteria**: What makes an ideal first customer in the new market (beyond ICP fit — includes reference potential, visibility, risk tolerance)
- **Target list**: 5-10 lighthouse account targets with specific rationale
- **Credibility-building outreach**: Messaging that acknowledges being new to the market while establishing credibility through adjacent expertise
- **Network-based entry**: How to leverage existing relationships, advisors, or partners for warm introductions
- **Content strategy**: Thought leadership and educational content to build awareness

#### Phase 4: Discovery & Validation (Discovery Agent + Qualification Agent)

Using personas and JTBDs (all treated as hypotheses):
- **Validation-focused discovery**: Questions designed to validate or refute ICP and JTBD hypotheses, not just qualify opportunities
- **Learning objectives per conversation**: What you need to learn from each early interaction
- **Pivot triggers**: What signals would indicate you need to change the ICP, persona, or JTBD definition
- **Modified qualification criteria**: Lighter qualification for early market entry (accept lower-confidence opportunities to learn)

#### Phase 5: Market Entry Metrics & Learning Loops (Continuous Improvement Agent)

- **Leading indicators**: Early signals of market fit (meeting acceptance rate, discovery quality, pilot conversion)
- **Validation milestones**: What constitutes ICP validation? (e.g., 3+ lighthouse wins with similar profile)
- **Feedback integration**: How to update the ICP, personas, JTBDs, and VPs based on what you learn
- **Scale decision criteria**: When is the beachhead proven enough to scale to full Acquire motion?

### Output Format

Present the guidance as a market entry playbook with:
- Beachhead strategy one-pager
- ICP hypothesis validation framework
- Lighthouse account target list criteria
- Adapted outreach sequences (credibility-focused, not feature-focused)
- Hypothesis validation discovery questions
- Pilot program structure
- Learning loop metrics dashboard
- Clear criteria for when Enter transitions to Acquire

## Lean Sales Context

The Enter workflow is the most Lean-aligned motion — it explicitly treats everything as a hypothesis and builds validation loops. In the Lean Sales method, the Enter workflow uses the Strategic Market Intelligence Agent, Segment Strategy Agent, Value Proposition Optimization Agent, and Offering Configuration Agent in a tight feedback loop. The Continuous Improvement Agent monitors learning velocity and signals when hypotheses are validated or need revision. The key Lean principle here is to minimize waste by testing assumptions before investing in scale.
