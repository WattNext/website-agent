# WattNext Website Agent

This repository is the working home for the WattNext website voice agent.

It contains:

- the approved knowledge base the bot is allowed to use
- conversation design for how the bot should behave
- source inventory and source-evaluation notes
- drafts and work-in-progress material that is not yet approved

The goal is to keep raw source material separate from approved bot-ready content.

## Current State

The repository now contains a first drafting pass across:

- company overview
- ideal customer profile
- problem patterns
- product explainer
- proof and trust
- FAQ
- conversation routes
- guardrails

Some sections are still intentionally conservative where approval is not yet settled, especially:

- pricing
- exact report-detail wording
- whether `anonymous voice conversations` should be the default public phrasing everywhere

## What This Repo Is For

The website agent should be able to:

- explain what WattNext is
- explain who it is for
- explain how the offer works
- answer common buyer questions clearly
- ask useful discovery questions
- build trust without overselling
- move a visitor toward a sensible next step

## Repository Layout

```text
website-agent/
  README.md
  .gitignore
  source-of-truth.md
  knowledge-base/
  conversation-design/
  sources/
  drafts/
```

## Folder Purpose

### `knowledge-base/`

Final approved answer units for the website agent.

This is the clean layer the bot should ultimately use.

### `conversation-design/`

Behavior and flow design for the agent, such as:

- demo mode
- discovery mode
- trust and FAQ mode
- booking mode
- referral or share mode

### `sources/`

Inventory of upstream material and notes on what each source is useful for.

This is where we track:

- Drive source files
- GitHub repos
- legacy tools
- prototypes
- websites
- supporting scripts

### `drafts/`

Unapproved material, brainstorms, experiments, and partially cleaned source content.

This is also the place to keep:

- review queues
- unresolved wording questions
- temporary holding answers

## Source Hierarchy

Use sources in this order:

1. Google Drive AI/LLM knowledge base
2. Sage repository
3. Sales-agent repository and related tools or prototypes

If sources conflict, prefer Drive unless a newer version has been explicitly approved for promotion into this repository.

See [source-of-truth.md](/Users/pollywatt/Website%20Chatbot/website-agent/source-of-truth.md) for the detailed content policy.

## Working Rule

Do not dump raw source files straight into the approved knowledge base.

The normal flow should be:

1. identify source material
2. evaluate whether it is primary, supporting, or reference-only
3. extract the useful claims or patterns
4. rewrite them into bot-ready units or conversation logic
5. only then promote them into `knowledge-base/`

## Current Scope

The current website agent is a presales and trust-building layer.

It may:

- explain
- demo
- ask probing questions
- qualify lightly
- offer next steps

It should not:

- invent claims
- pretend unfinished capabilities are live
- give consulting advice beyond presales framing
- state unapproved pricing
