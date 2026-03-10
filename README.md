# Lean Sales Skills

A set of [Claude Code](https://claude.com/claude-code) Skills implementing the **Lean Sales Method** — an end-to-end sales management system based on systems thinking and Lean principles.

## What is the Lean Sales Method?

The Lean Sales Method applies Lean principles to B2B sales management:

- **Flow efficiency** — minimize wait time, maximize value-adding activity
- **Waste elimination** — stop pursuing poor-fit prospects, generic outreach, and redundant meetings
- **Pull-based flow** — only pull new opportunities when capacity exists
- **Constraint management** — identify and optimize the bottleneck
- **Continuous improvement** — systematic learning loops across the sales process

The method is built on a **26-agent architecture** across three layers:

| Layer | Agents | Purpose |
|-------|--------|---------|
| **Strategy** | 6 | Define WHO to target, WHAT to offer, HOW to position |
| **Management** | 5 | Optimize flow, quality, and performance |
| **Execution** | 15 | Execute the sales process end-to-end |

These agents are organized into two core systems:

1. **Opportunity Generation Engine** — transforms strategy into qualified opportunities
2. **Opportunity Pursuit System** — converts qualified opportunities into closed deals

## The GTM Play — Core Concept

A **GTM Play** is the foundational unit of execution. It binds together:

```
GTM Play
├── Strategy: expand | acquire | enter
├── ICP (Ideal Customer Profile)
│   ├── Buyer Persona 1
│   │   ├── JTBD (Jobs-To-Be-Done)
│   │   └── Value Proposition
│   ├── Buyer Persona 2
│   │   ├── JTBD
│   │   └── Value Proposition
│   └── ...
├── Market Context
└── Success Metrics
```

| Concept | What It Defines |
|---------|----------------|
| **ICP** | Company-level targeting — firmographics, technographics, behavioral signals |
| **Buyer Persona** | Individual-level engagement — role, pain points, motivations, DMU role |
| **JTBD** | The job the buyer hires a solution to do — functional, emotional, social dimensions |
| **Value Proposition** | Tailored messaging per persona — benefits, proof points, differentiation |

## Three Workflows

| Workflow | Target | When to Use |
|----------|--------|-------------|
| **Expand** | Existing customers | Account growth, upsell/cross-sell, whitespace analysis |
| **Acquire** | New customers in known markets | Competitive displacement, outreach sequences |
| **Enter** | New markets | Beachhead strategy, hypothesis validation, lighthouse accounts |

## Skills

### Play Creation

| Skill | Description |
|-------|-------------|
| `/create-gtm-play` | Full orchestrator — walks through strategy, ICP, personas, JTBD, and value props |
| `/create-icp` | Define an Ideal Customer Profile |
| `/create-persona` | Create a Buyer Persona linked to an ICP |
| `/create-jtbd` | Define a Jobs-To-Be-Done for a persona |
| `/create-value-prop` | Craft a Value Proposition for a persona + JTBD |

### Play Management

| Skill | Description |
|-------|-------------|
| `/list-plays` | Overview of all GTM Plays |
| `/show-play` | Full view of a play with all linked entities |
| `/validate-play` | Structural, completeness, and quality validation |

### Workflow Execution

| Skill | Description |
|-------|-------------|
| `/expand-play` | Generate Expand workflow guidance for existing customer growth |
| `/acquire-play` | Generate Acquire workflow guidance for new customer acquisition |
| `/enter-play` | Generate Enter workflow guidance for new market penetration |

### Background Knowledge (auto-loaded by Claude)

| Skill | Triggers When |
|-------|---------------|
| `lean-sales-method` | Discussing sales methodology, pipeline, Lean principles |
| `gtm-play-design` | Discussing GTM plays, data model, entity relationships |

## Getting Started

1. Open this project in Claude Code
2. Run `/create-gtm-play` to build your first play end-to-end
3. Or build bottom-up: `/create-icp` → `/create-persona` → `/create-jtbd` → `/create-value-prop`
4. Validate with `/validate-play`
5. Generate execution guidance with `/expand-play`, `/acquire-play`, or `/enter-play`

## Project Structure

```
LeanSalesSkills/
├── .claude/skills/          # Claude Code Skills (13 skills)
├── schemas/                 # JSON Schema definitions
│   ├── gtm-play.schema.json
│   ├── icp.schema.json
│   ├── persona.schema.json
│   ├── jtbd.schema.json
│   └── value-proposition.schema.json
├── data/                    # Runtime data (created by skills)
│   ├── gtm-plays/
│   ├── icps/
│   ├── personas/
│   ├── jtbd/
│   └── value-propositions/
├── CLAUDE.md                # Project instructions for Claude
└── *.md                     # Reference documentation
```

## Data Model

All entities are stored as JSON files in the `data/` directory, linked by ID references:

- **IDs** use type-prefix + slug: `play-nordic-manufacturing`, `icp-midmarket-saas`, `persona-cto-digital`, `jtbd-vendor-assessment`, `vp-cto-automation`
- **Schemas** in `schemas/` define the structure and validation rules
- **Cross-references** are bidirectional (e.g., ICP lists persona IDs, personas reference back to ICP)

## Reference Documents

- `Agentic_Sales_Systems_Simplified_Illustrations_v3.md` — System architecture, workflow diagrams, and worked examples
- `Functional_Requirements_for_Individual_AI_Agents_in_the_Agentic_Sales_System_v3.md` — Detailed functional requirements for all 26 agents

## Learn More

The Lean Sales Method is a comprehensive B2B sales management system developed by Tapio Nissilä. To learn more about the methodology, the agentic sales architecture, and how to apply Lean principles to your sales organization:

- **Website**: [leansales.fi](https://leansales.fi) — methodology overview, resources, and latest updates
- **Book**: [*Lean Sales Method — End to End Sales Management System*](https://www.amazon.com) — available on Amazon.com

## License

Proprietary. Based on the book *Lean Sales Method — End to End Sales Management System* by Tapio Nissilä.
