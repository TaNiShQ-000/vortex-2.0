# System Architecture (v1 – frozen)

## High-Level Flow
User
↓
Observation Layer (passive only)
↓
Control Layer (rules & permissions)
↓
Cognition Layer (memory + reasoning)
↓
Suggestions (drafts, replies, ideas)
↓
User edits / approval


## Layer Responsibilities

### Observation Layer
- Collects **passive signals** only
- **Never** triggers actions
- **Never** generates content

**Examples:**
- Edits made
- Rejections
- Dwell signals

### Control Layer
- Enforces rules
- Blocks unsafe or off-tone output
- Decides what requires approval

**Important:**  
This layer is **rules + heuristics** — **not** LLM creativity.

### Cognition Layer
- Generates drafts
- Suggests replies
- Maintains memory
- Outputs confidence & risk scores

**It cannot:**
- Click buttons
- Post content
- Send DMs
- Scrape LinkedIn
- Perform any external action

### Execution Layer
- **Not present in v1**
- Any automation is **explicitly out of scope**

## Non-Negotiable Rule

**Cognition can only suggest.**  
**It can never act.**

## Why this matters (no sugarcoating)

If you don’t freeze this architecture:

- You’ll blur cognition + control
- You’ll add “just one little automation”
- You’ll accidentally build a spam bot
- You’ll violate your own principles

**This document is your guardrail.**