# Memory Model (v1 – frozen)

## Memory Types

### 1. Identity Memory
Stores **long-term traits** of the user.

**Examples:**
- Writing tone (direct, reflective, aggressive, calm)
- Belief stances (e.g. anti-growth-hacks, pro-quality)
- Topics avoided
- Vocabulary preferences

**Characteristics:**
- Rarely changes
- High trust
- **Manually editable only**

### 2. Episodic Memory
Stores outcomes and learning from past actions.

**Examples:**
- Posts that performed well
- Posts that failed
- Reason for user edits
- Why a suggestion was rejected

**Characteristics:**
- Grows over time
- Used for learning
- Time-scoped

### 3. Interaction Memory
Stores social context.

**Examples:**
- Frequent commenters
- Relationship notes
- Past conversation summaries

**Characteristics:**
- Lightweight
- Contextual
- **Never speculative**

### 4. Instruction Memory
Stores explicit user rules.

**Examples:**
- Style constraints
- Strategic goals
- Hard rules (“never sound motivational”)

**Characteristics:**
- **Highest priority**
- Always applied
- **User-controlled**

## What Gets Written to Memory

### High-signal (always store)
- User edits
- Rewrites
- Deletions
- Rejections
- Manual notes

### Low-signal (store lightly)
- Likes
- Impressions
- Engagement counts

### Never store
- Raw scraped feed data
- Other people’s content verbatim
- Temporary prompts

## Memory Write Triggers

Memory updates happen **only** when:

- User edits generated text
- User approves a draft
- User explicitly gives feedback
- User overrides a suggestion

**No silent learning. No guessing.**

## Learning Loop
Observe → Suggest → User edits → Store delta → Improve next output


**If this loop breaks, the product fails.**

## Why this matters (tell-it-like-it-is)

Without this system:

- You will start logging everything
- Memory becomes noisy
- The model “feels smart” but gets worse
- You lose trust in your own system

**This file prevents future stupidity.**