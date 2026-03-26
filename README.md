# Lean Sales Skills

Claude Code Skills for B2B sales development, built on the **Lean Sales methodology**.

## Why Lean Thinking in Sales?

Most B2B sales organizations suffer from the same problems: reps chase wrong-fit prospects, pipelines are unpredictable, and activity is confused with progress. The root cause is the same one Lean manufacturing solved decades ago — **waste**.

Lean Sales applies proven Lean principles to B2B sales:

| Lean Principle | What It Means in Sales |
|---|---|
| **Eliminate waste** | Stop pursuing prospects who will never buy. Stop writing generic outreach. Stop holding meetings without clear next steps. |
| **Flow efficiency** | Measure how much of the sales cycle is value-adding vs. waiting. Most B2B deals spend 80%+ of their lifecycle waiting — for internal approvals, for follow-ups, for decisions. |
| **Pull, don't push** | Only pull new opportunities into the pipeline when you have capacity to work them properly. Overloaded pipelines kill conversion rates. |
| **Find the constraint** | Every sales organization has one bottleneck that limits throughput. Find it, fix it, then find the next one. |
| **Continuous improvement** | Systematic win/loss reviews, not anecdotal war stories. Every closed deal teaches something — capture it. |

The result: **more revenue from fewer, better-qualified opportunities** — with less wasted effort across the team.

## What This Repo Does

This repo provides a set of Claude Code Skills that operationalize Lean Sales as an interactive AI-assisted workflow. You define your go-to-market strategy, and the skills help you build, validate, and execute it step by step.

### Core Concept: The GTM Play

A **GTM Play** is the foundational unit of execution. It binds together your target market, buyer personas, their jobs-to-be-done, and your value propositions into a coherent, executable plan.

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

### Skills

**Play Creation:**
- `/create-gtm-play` — Full orchestrator: strategy, ICP, personas, JTBD, and value props
- `/create-icp` — Define an Ideal Customer Profile
- `/create-persona` — Create a Buyer Persona linked to an ICP
- `/create-jtbd` — Define Jobs-To-Be-Done for a persona
- `/create-value-prop` — Craft a Value Proposition for a persona + JTBD

**Play Management:**
- `/list-plays` — Overview of all GTM Plays
- `/show-play` — Full view of a play with all linked entities
- `/validate-play` — Structural, completeness, and quality validation

**Workflow Execution:**
- `/expand-play` — Guidance for growing existing accounts
- `/acquire-play` — Guidance for winning new customers
- `/enter-play` — Guidance for entering new markets

### Background Knowledge (auto-loaded)
- `lean-sales-method` — Triggers when discussing sales methodology or Lean principles
- `gtm-play-design` — Triggers when discussing GTM plays or data model

## Getting Started

1. Open this project in Claude Code
2. Run `/create-gtm-play` to build your first play end-to-end
3. Or build bottom-up: `/create-icp` → `/create-persona` → `/create-jtbd` → `/create-value-prop`
4. Validate with `/validate-play`
5. Execute with `/expand-play`, `/acquire-play`, or `/enter-play`

## 26-Agent Architecture

The skills are built on a 26-agent architecture across three layers:

| Layer | Agents | Purpose |
|-------|--------|---------|
| **Strategy** | 6 | Define WHO to target, WHAT to offer, HOW to position |
| **Management** | 5 | Optimize flow, quality, and performance |
| **Execution** | 15 | Execute the sales process end-to-end |

## Learn More

- **Website**: [leansales.fi](https://leansales.fi)
- **Book**: *Lean Sales — More Sales with Less Selling* by Tapio Nissilä (2013), available on [Amazon](https://www.amazon.com)

## License

Proprietary. Based on the Lean Sales methodology by Tapio Nissilä.
