# Source Of Truth

This document defines where knowledge for the WattNext website agent should come from, how it should be validated, and how conflicts should be handled.

## Purpose

The website agent needs a curated front-of-house knowledge base.

That means this repository should contain approved, reusable answers for presales and trust-building conversations, not raw research and not every internal document.

## Source Priority

Use sources in the following order.

### 1. Google Drive AI/LLM knowledge base

This is the primary source for:

- approved messaging
- current positioning
- methodology language that is safe to share
- founder and company framing
- offer descriptions

Treat Drive as the default source of truth unless there is a clearly newer approved version elsewhere.

### 2. Sage repository

Use Sage as the secondary source for:

- product context
- implementation-relevant detail
- terminology consistency
- supporting workflow descriptions

Sage is useful for grounding product statements, but it should not override approved public messaging from Drive on its own.

### 3. Sales-agent repository and Bolt project

Use these as supporting sources for:

- likely buyer questions
- objection patterns
- conversion language
- example flows
- draft framing that may be worth promoting later

Do not treat this material as automatically approved. It may be incomplete, stale, exploratory, or optimized for a different use case.

## Trust Levels

When adding material to this repository, classify it mentally in one of three buckets.

### Approved

Use directly in the main section folders when:

- the claim is present in Drive, or
- it is confirmed by Drive plus another reliable source, or
- it has been explicitly approved for public use

### Supported But Not Yet Approved

Put in `drafts/` when:

- it appears in Sage or sales-agent material but not in Drive
- it sounds plausible but needs confirmation
- the wording is useful but the claim needs tightening

### Not Usable

Do not include as approved knowledge when:

- the claim cannot be traced to a source
- the material reads like internal speculation
- it makes performance or client claims that are not approved
- it implies features, outcomes, or pricing that are not settled

## Conflict Rules

If sources disagree:

1. Drive wins by default.
2. If Sage is newer and clearly more accurate, mark the item for review rather than silently replacing the Drive version.
3. If sales-agent or Bolt material conflicts with Drive or Sage, treat it as draft only.
4. If no source is fully reliable, do not publish the claim into the main KB.

## What Belongs In This Repo

Include:

- short answer units for the website agent
- FAQs
- conversation routing rules
- trust-safe product explanations
- qualification and CTA language
- explicit guardrails

Do not include:

- giant raw document dumps
- full internal methodology archives
- technical implementation notes for engineering unless directly needed for agent behavior
- unapproved case studies
- invented examples or made-up proof points

## Writing Standard

All content in this repository should be:

- easy to say out loud
- easy to retrieve in small pieces
- safe to use in a public-facing conversation
- explicit about uncertainty when needed

The agent should sound helpful and credible, not exhaustive.

## Promotion Workflow

When new source material is found:

1. Identify the underlying claim.
2. Trace it to the best available source.
3. Rewrite it into answer-unit format.
4. Place it in the correct section if approved.
5. Place it in `drafts/` if not yet approved.
6. Update `content-status.md` if a section still has gaps or unresolved questions.

## Working Principle

This repository is the final cleaned layer between upstream source material and the website agent.

It should function as a publishing repo for approved conversational knowledge, not as a storage bucket for everything WattNext knows.
