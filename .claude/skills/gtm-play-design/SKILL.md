---
name: gtm-play-design
description: Knowledge about the GTM Play data model, entity relationships, and design best practices. Loaded automatically when discussing GTM plays, play creation, or entity relationships (ICP, Persona, JTBD, Value Prop).
user-invocable: false
---

# GTM Play Design — Data Model & Best Practices

## Data Model

```
GTM Play
├── Strategy: expand | acquire | enter
├── Market Context (geography, industry, maturity, competitive landscape)
├── Success Metrics (opportunities/quarter, win rate, deal size, cycle length)
├── ICP (1 per play)
│   ├── Firmographics (industry, size, revenue, geography, company type)
│   ├── Technographics (tech stack, digital maturity, key systems)
│   ├── Behavioral Signals (buying triggers, disqualifiers, cycle length)
│   └── Buyer Personas (1:many)
│       ├── Role Identity (title, department, seniority, DMU role)
│       ├── Psychology (pain points, motivations, success metrics, objections)
│       ├── Communication Preferences (channels, format, tone, meeting style)
│       ├── JTBD (1 per persona)
│       │   ├── Job Statement: "When [situation], I want to [motivation], so I can [outcome]"
│       │   ├── Dimensions: functional, emotional, social
│       │   ├── Current State: current solution, constraints
│       │   └── Underserved Outcomes (importance x satisfaction)
│       └── Value Proposition (1 per persona)
│           ├── Headline + Core Message
│           ├── Key Benefits (benefit + proof point + quantification)
│           ├── Differentiation (vs. status quo, vs. competitors, unique mechanism)
│           ├── Objection Responses
│           └── Elevator Pitches (30s, 60s) + Email Hook
```

## Entity Relationships

| From | To | Cardinality | Linked By |
|------|----|-------------|-----------|
| GTM Play | ICP | 1:1 | `play.icp_id` |
| ICP | Buyer Persona | 1:many | `icp.persona_ids[]` |
| Buyer Persona | ICP | many:1 | `persona.icp_id` |
| Buyer Persona | JTBD | 1:1 | `persona.jtbd_id` |
| Buyer Persona | Value Proposition | 1:1 | `persona.value_proposition_id` |
| JTBD | Buyer Persona | 1:1 | `jtbd.persona_id` |
| Value Proposition | Buyer Persona | 1:1 | `vp.persona_id` |
| Value Proposition | JTBD | 1:1 | `vp.jtbd_id` |

## ID Convention

All IDs use type-prefix + slugified-name: `play-{slug}`, `icp-{slug}`, `persona-{slug}`, `jtbd-{slug}`, `vp-{slug}`

## File Locations

- Plays: `data/gtm-plays/{play-id}/play.json`
- ICPs: `data/icps/{icp-id}.json`
- Personas: `data/personas/{persona-id}.json`
- JTBDs: `data/jtbd/{jtbd-id}.json`
- Value Props: `data/value-propositions/{vp-id}.json`
- Schemas: `schemas/*.schema.json`

## Design Best Practices

### ICP Design
- Be specific enough to disqualify — a good ICP says NO more than YES
- Include disqualifiers (not just positive criteria)
- Buying triggers are the most actionable part of an ICP
- Start with 1 primary ICP per play; add secondary only when primary is validated

### Persona Design
- Cover at least the economic buyer and one other DMU role
- Pain points should be specific and observable, not generic
- Objections should come from real sales conversations
- Communication preferences directly inform outreach strategy

### JTBD Design
- The job statement must be solution-agnostic (describe the job, not your product)
- Underserved outcomes are the most valuable part — they define where you win
- "Importance: critical + Satisfaction: unmet" = strongest opportunity
- Current solution is never "nothing" — there's always a workaround

### Value Proposition Design
- Every benefit should trace back to an underserved JTBD outcome
- Proof points > claims — always include evidence
- The email hook should reference the persona's world, not yours
- Differentiation vs. status quo is more important than vs. competitors (inertia is the biggest competitor)

### Play Completeness
A play is ready for execution when:
1. ICP has clear firmographic boundaries and buying triggers
2. At least 2 personas cover economic buyer + another DMU role
3. Each persona has a specific, solution-agnostic JTBD
4. Each VP addresses at least 2 underserved outcomes from the JTBD
5. Success metrics are set and realistic for the strategy type
