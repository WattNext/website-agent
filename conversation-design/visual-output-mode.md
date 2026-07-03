# Visual Output Mode

This document defines how the website voice agent can produce live on-screen visual outputs in the style of the 1mind references.

The reference pattern is not just a chatbot.

It is:

- conversation on the left
- a live visual canvas on the right
- slide-like cards that change based on the conversation
- a presenter flow that feels tailored in real time

## Purpose

Visual output mode should help the agent:

- explain complex ideas quickly
- make pricing and fit easier to grasp
- show structured outputs without sounding abstract
- create a stronger demo effect on the website

## Best Use Cases

Strong uses:

- pricing overview
- pilot versus annual comparison
- enterprise estimate summary
- implementation flow
- trust and proof summaries
- fit and qualification explanation
- friction calculator results summary

Weak uses:

- raw long-form text
- complex legal language
- highly tentative or unapproved claims

## How It Should Work

The voice agent should not directly "draw" visuals.

Instead, it should produce a structured presentation payload that the front end renders.

Recommended flow:

1. gather the needed inputs in conversation
2. convert them into a structured object
3. choose a visual template
4. send the payload to the front end
5. let the front end render the card, table, or comparison view

## Pricing Visual Templates

### Template 1. Fixed-band pricing summary

Use when the visitor asks:

- how pricing works
- what the tiers are
- whether there are bands

Suggested content:

- `Growth`
- `Expansion`
- `Scale`
- `Enterprise`

### Template 2. Enterprise estimate card

Use when the visitor gives employee count above `500`.

Suggested content:

- company size
- annual program type
- pricing anchor at `500`
- incremental enterprise amount
- estimated annual total
- note that final scope may vary with complexity

### Template 3. Pilot versus annual comparison

Use when the visitor asks:

- should we start with a pilot
- how the pilot differs
- why annual pricing is different

Suggested columns:

- scope
- waves per year
- participant volume
- type of output
- price logic
- commercial purpose

The commercial-purpose row should make the distinction clear:

- `Pilot`: trust buy-in, low-risk test
- `Annual`: broader operating rollout

### Template 4. Value framing card

Use when the visitor wants a quick pricing explanation with business context.

Suggested sections:

- what is included
- why anonymity matters
- why full inclusion matters
- why enterprise pricing steps gradually

## Example Presentation Payload

```json
{
  "template": "enterprise-estimate-card",
  "title": "Estimated annual pricing",
  "subtitle": "Balanced model for full-participant coverage",
  "theme": "wattnext-pricing",
  "data": {
    "company_name": "ExampleCo",
    "employee_count": 780,
    "program_type": "annual",
    "tier": "Enterprise",
    "price_eur": 49800,
    "note": "Final pricing may vary with delivery complexity."
  }
}
```

## Recommended Front-End Components

If implemented in the website app, the front end should support:

- title plus subtitle hero card
- two-column explanation card
- tier table
- comparison cards
- simple bar or step chart
- metrics tiles

These should be template-driven rather than free-form generated each time.

## Why Template-Driven Is Better

Template-driven visuals are safer because they:

- reduce hallucinated numbers
- keep layout consistent
- protect brand style
- allow content approval
- make engineering simpler

## Pricing-Specific Guardrail

The agent should only render pricing visuals from approved pricing objects.

It should not render:

- speculative custom numbers
- outdated pricing logic
- internal cost assumptions
- ROI claims that are not approved

## Conversation Pattern

Good flow:

- ask company size
- ask whether they are exploring pilot or annual
- explain the band or estimate
- offer to show a pricing summary card
- route to Polly if they want a scoped commercial discussion

## Fallback

If visual rendering is unavailable, the agent should still be able to:

- explain the pricing in plain language
- provide a text summary
- offer a follow-up conversation
