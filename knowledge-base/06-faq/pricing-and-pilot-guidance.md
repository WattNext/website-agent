# Pricing And Pilot Guidance

## Answer Unit

```md
title: pricing_overview_public_safe
category: faq
trigger: how does pricing work; what are your pricing bands; what are the tiers
short_answer: At a high level, pricing is tiered by company size up to 500 employees, with enterprise pricing stepping up gradually above that rather than jumping sharply.
approved_answer: The public-safe overview is that the annual program uses tiered pricing up to 500 employees, and enterprise pricing continues above that on a stepped basis rather than creating a cliff. The current working bands are Growth for 50 to 150, Expansion for 150 to 250, Scale for 250 to 500, and Enterprise above that.
expand_if_asked: The exact enterprise figure depends on company size and scope, but the principle is that pricing rises gradually rather than penalizing a company for crossing one threshold.
cta: If helpful, I can explain the tier logic at a high level or point you to a short conversation with Polly for a scoped estimate.
confidence_level: medium
source_owner: user-approved working pricing framework
last_updated: 2026-07-03
```

## Answer Unit

```md
title: why_enterprise_pricing_steps_gradually
category: faq
trigger: why is enterprise custom; why not one flat enterprise price; what happens above 500
short_answer: The enterprise step should be gradual, because a buyer should not be punished for having 501 people instead of 500.
approved_answer: The logic above 500 is meant to be gradual rather than cliff-based. The idea is to avoid a pricing shock at the moment a company crosses into enterprise territory, while still reflecting the fact that larger participant volumes create more delivery cost and processing load.
expand_if_asked: The public-safe explanation is that enterprise pricing balances broader inclusion, stronger anonymity, and heavier delivery requirements.
cta: If useful, I can give the high-level enterprise logic or route you to Polly for a tailored estimate.
confidence_level: high
source_owner: user-approved working pricing framework
last_updated: 2026-07-03
```

## Answer Unit

```md
title: pilot_vs_annual_program
category: faq
trigger: what is the pilot; how is pilot different; why is the pilot priced differently
short_answer: The pilot is meant as a low-risk trust buy-in. It is a smaller one-wave subset, while the annual program is broader and designed to run twice yearly.
approved_answer: The pilot is a lower-scope entry point designed to help a buyer build trust with limited downside. It is priced per participant, runs once, and is meant for a smaller subset. The annual program is a broader operating model, typically run twice yearly, with stronger organizational signal, wider participation, and more complete output.
expand_if_asked: The idea is simple: if the buyer likes the pilot, they can roll it out more broadly. If they do not, they have lost very little. That is why the pilot should not be treated as a simple proxy for annual pricing.
cta: If helpful, I can explain which starting point is more likely to fit your situation.
confidence_level: high
source_owner: user-approved working pricing framework
last_updated: 2026-07-03
```

## Answer Unit

```md
title: why_offer_a_pilot_first
category: faq
trigger: why do a pilot first; why start with a pilot; what is the point of the pilot
short_answer: The pilot is there to create trust and give the buyer a low-risk way to test whether the approach is worth rolling out.
approved_answer: The point of the pilot is to create trust with limited downside. It gives the buyer a way to test the experience, the quality of the signal, and the practical value before committing to a broader annual rollout. If it works, the next step is wider adoption. If it does not, the buyer has not taken a large commercial risk.
expand_if_asked: That makes the pilot a commercial trust step, not just a cheaper version of the full program.
cta: If useful, I can explain how the pilot differs from the annual program in scope and intent.
confidence_level: high
source_owner: user-approved working pricing framework
last_updated: 2026-07-03
```

## Answer Unit

```md
title: can_the_agent_show_pricing_visually
category: faq
trigger: can you show me the pricing; can you put that in a chart; can you summarize this visually
short_answer: Yes, if the front end supports it, the agent can turn the pricing framework into a structured visual summary rather than just describing it in text.
approved_answer: Yes. The cleanest implementation is for the agent to gather the right inputs, turn them into a structured pricing object, and then let the front end render that as a pricing card, tier table, comparison view, or estimate chart. That keeps the visual output consistent and avoids free-form number generation on the fly.
expand_if_asked: The important part is that the chart should be template-driven and based on approved pricing logic, not improvised each time.
cta: If useful, I can outline the kinds of visuals the pricing flow could support.
confidence_level: high
source_owner: implementation guidance based on user request
last_updated: 2026-07-03
```
