# Morning Handoff

This is the quick review note for the current first-pass build of the WattNext website agent repository.

## What Is Now In Place

- source hierarchy and source-of-truth rules
- source inventory
- canonical Q&A shortlist
- conversation design for:
  - discovery
  - trust / FAQ
  - booking
- guardrails and non-share rules
- first-pass answer units for:
  - company overview
  - ideal customer profile
  - problem patterns
  - product explainer
  - proof and trust
  - FAQ
  - conversation route summary

## Best Files To Review First

- [knowledge-base/content-status.md](/Users/pollywatt/Website%20Chatbot/website-agent/knowledge-base/content-status.md)
- [drafts/review-queue.md](/Users/pollywatt/Website%20Chatbot/website-agent/drafts/review-queue.md)
- [knowledge-base/04-product-explainer/vivo-pulse-basics.md](/Users/pollywatt/Website%20Chatbot/website-agent/knowledge-base/04-product-explainer/vivo-pulse-basics.md)
- [knowledge-base/06-faq/website-faq-starter.md](/Users/pollywatt/Website%20Chatbot/website-agent/knowledge-base/06-faq/website-faq-starter.md)
- [conversation-design/booking-mode.md](/Users/pollywatt/Website%20Chatbot/website-agent/conversation-design/booking-mode.md)

## Main Open Decisions

- pricing wording for public use
- whether `anonymous voice conversations` should stay as the default website phrasing
- how specific the bot should be about report outputs
- whether any approved public proof examples can be added

## Current Operating Stance

The repo is intentionally conservative where approval is uncertain.

That means the bot currently:

- explains clearly
- qualifies lightly
- offers Polly first and Mike second
- avoids pricing specifics
- avoids methodology internals
- avoids named proof unless approved

## Suggested Next Build Step

After review, the next likely step is:

- tighten approved wording
- decide what gets committed and pushed
- then create the Google Drive mirror from the cleaned repo structure
