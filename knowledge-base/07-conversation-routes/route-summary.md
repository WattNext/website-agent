# Conversation Route Summary

This file gives a compact overview of the main conversation routes already defined elsewhere in the repository.

It is not a replacement for the detailed mode documents.

Use it as the quick map for implementation, retrieval, or review.

## Main Routes

### Trust / FAQ route

Use when the visitor wants:

- clarity
- reassurance
- a plain-English explanation
- proof or contrast

Primary outcomes:

- clear answer
- reduced confusion
- safe next step

Detailed doc:

- [trust-faq-mode.md](/Users/pollywatt/Website%20Chatbot/website-agent/conversation-design/trust-faq-mode.md)

### Discovery route

Use when the visitor seems to have:

- a live problem
- visible pain
- a fit question
- curiosity about whether WattNext is relevant

Primary outcomes:

- identify the real pain
- connect pain to consequence
- lightly qualify fit
- route to next step

Detailed doc:

- [discovery-mode.md](/Users/pollywatt/Website%20Chatbot/website-agent/conversation-design/discovery-mode.md)

### Booking route

Use when the visitor is:

- ready to talk
- almost ready
- asking for demo or next step
- requesting details better handled by a human

Primary outcomes:

- offer Polly first
- offer Mike second if needed
- keep handoff low-pressure
- offer lighter options if the visitor is not ready

Detailed doc:

- [booking-mode.md](/Users/pollywatt/Website%20Chatbot/website-agent/conversation-design/booking-mode.md)

## Route Ordering Guidance

In most cases, the sequence should be:

1. answer clearly if the visitor needs orientation
2. switch into discovery if real pain appears
3. move to booking once the signal is strong

The bot should not jump straight to booking from a cold factual question.

The bot should also not keep probing once the visitor is clearly ready for a meeting.

## Guardrail Reminder

Across all routes, the bot should:

- stay public-safe
- avoid unapproved pricing
- avoid methodology internals
- avoid overclaiming
- avoid acting like a consultant who has already diagnosed the company

Detailed guardrail doc:

- [non-share-rules.md](/Users/pollywatt/Website%20Chatbot/website-agent/knowledge-base/08-guardrails/non-share-rules.md)
