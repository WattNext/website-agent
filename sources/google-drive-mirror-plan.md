# Google Drive Mirror Plan

This file describes how the repository should later be mirrored into the AI / LLM Google Drive for shared use by other models.

## Purpose

GitHub should remain the working and versioned build environment.

Google Drive should hold a clean mirrored copy that:

- other LLM workflows can access
- humans can browse quickly
- stays curated rather than becoming a raw dump

## Mirror Structure

Recommended Drive folder structure:

- `01-company-overview`
- `02-ideal-customer-profile`
- `03-problem-patterns`
- `04-product-explainer`
- `05-proof-and-trust`
- `06-faq`
- `07-conversation-routes`
- `08-guardrails`
- `sources`
- `drafts`

## Mirror Rule

The Drive mirror should follow the repository structure closely.

That makes it easier to:

- keep parity between GitHub and Drive
- let other LLMs find the same material
- avoid duplicate or conflicting copies

## What Should Go To Drive

Safe to mirror:

- cleaned answer units
- conversation design docs
- source inventory
- review queue
- source-of-truth rules

Do not mirror as if approved:

- raw upstream exports
- internal-only documents
- private client material
- unapproved proof examples

## Suggested Mirror Timing

Best sequence:

1. finish a stable first pass in GitHub
2. review and tighten the wording
3. push the repo
4. create the matching Drive mirror
5. periodically refresh the Drive copy from the repo

## Open Question

Still to decide:

- whether Drive should contain exact file copies, exported PDFs, or a mix of both for easier non-technical browsing
