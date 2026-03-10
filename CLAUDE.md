# Lean Sales Skills

This project implements the **Lean Sales Method** as a set of Claude Code Skills. The Lean Sales Method is an end-to-end sales management system based on systems thinking and Lean principles, focused on improving flow efficiency, eliminating waste, and performing continuous improvement.

## Architecture

- **26 AI Agents** across 3 layers: Strategy (6), Management (5), Execution (15)
- **Two core systems**: Opportunity Generation Engine + Opportunity Pursuit System
- **Three workflows**: Expand (existing customers), Acquire (new customers), Enter (new markets)

## Key Concepts

- **GTM Play**: The foundational construct — a combination of Strategy, ICP, Buyer Persona(s), and JTBD(s) for a go-to-market motion
- **ICP (Ideal Customer Profile)**: Structured company-level targeting profile with firmographic, technographic, and behavioral attributes
- **Buyer Persona**: Role-level profile of a decision-maker within an ICP. One ICP may have one or more Buyer Personas
- **JTBD (Jobs-To-Be-Done)**: Each Buyer Persona has one JTBD describing the job they hire a solution to do
- **Value Proposition**: Tailored messaging per Persona x JTBD combination

## Data Model

```
GTM Play
├── Strategy: expand | acquire | enter
├── ICP (1 per play)
│   ├── Buyer Persona 1
│   │   ├── JTBD
│   │   └── Value Proposition
│   ├── Buyer Persona 2
│   │   ├── JTBD
│   │   └── Value Proposition
│   └── ...
└── Market Context + Success Metrics
```

## File Structure

- `schemas/` — JSON Schema definitions for all entities
- `data/` — Runtime data (GTM plays, ICPs, personas, JTBDs, value propositions)
- `.claude/skills/` — Claude Code Skills (slash commands)
- `Agentic_Sales_Systems_Simplified_Illustrations_v3.md` — System architecture reference
- `Functional_Requirements_for_Individual_AI_Agents_in_the_Agentic_Sales_System_v3.md` — Agent requirements reference

## ID Convention

All entities use slugified IDs with type prefix: `play-{slug}`, `icp-{slug}`, `persona-{slug}`, `jtbd-{slug}`, `vp-{slug}`

## Skills

| Skill | Purpose |
|-------|---------|
| `/create-gtm-play` | Create a complete GTM Play (orchestrator) |
| `/create-icp` | Define an Ideal Customer Profile |
| `/create-persona` | Create a Buyer Persona linked to an ICP |
| `/create-jtbd` | Define a Job-To-Be-Done for a Persona |
| `/create-value-prop` | Craft a Value Proposition for a Persona x JTBD |
| `/list-plays` | List all GTM Plays |
| `/show-play` | Display a complete GTM Play with all linked entities |
| `/validate-play` | Check play completeness and consistency |
| `/expand-play` | Generate Expand workflow guidance for a play |
| `/acquire-play` | Generate Acquire workflow guidance for a play |
| `/enter-play` | Generate Enter workflow guidance for a play |
