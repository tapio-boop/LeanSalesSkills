---
name: list-plays
description: List all GTM Plays with their strategy, ICP, status, and linked persona count. Use when the user wants an overview of defined plays.
allowed-tools: Read, Glob, Bash(ls:*)
---

# List GTM Plays

## Context

Play files:
!`ls data/gtm-plays/*/play.json 2>/dev/null || echo "No plays defined yet. Use /create-gtm-play to create one."`

## Instructions

1. Read all `data/gtm-plays/*/play.json` files
2. For each play, also read the linked ICP to get the ICP name and persona count
3. Display a summary table:

| Play Name | Strategy | Status | ICP | Personas | Created |
|-----------|----------|--------|-----|----------|---------|
| ... | expand/acquire/enter | draft/active/... | ICP name | count | date |

4. If no plays exist, suggest using `/create-gtm-play`
5. If plays exist, offer to show details with `/show-play {play-id}`
