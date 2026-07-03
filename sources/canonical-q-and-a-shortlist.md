# Canonical Q&A Shortlist For Website Agent

This document narrows the large canonical Q&A repository into the subset that is most useful for a public-facing website voice agent.

The goal is not to use all 157 questions.

The goal is to identify the questions that help the website agent:

- explain the problem clearly
- help visitors recognize their pain
- build trust in WattNext's way of thinking
- create a smooth bridge to calculator, sample report, or meeting

## Selection Rule

For the website agent, the best canonical Q&A topics are usually:

- clear enough for a first conversation
- relevant to leadership pain
- good at helping a buyer self-diagnose
- trust-building without sounding academic
- safe to discuss in a short spoken format

Less suitable topics can still be valuable later, but they do not belong in the first website-agent release.

## Tier 1: Use First

These are the strongest candidates for early extraction into the website knowledge base or conversation design.

### Core Problem Framing

- `what-is-organizational-friction-and-why-does-it-persist`
- `what-causes-execution-gaps-between-strategy-and-day-to-day-work`
- `what-makes-organizational-issues-systemic-rather-than-individual`
- `why-do-organizational-problems-keep-reappearing-after-interventions`

Why these matter:

- they explain the core WattNext worldview
- they help visitors understand that the problem is systemic, not just personal underperformance
- they create a strong bridge into ViVo Pulse

### Strategic Misalignment

- `why-do-leadership-teams-think-theyre-aligned-when-theyre-not`
- `alignment-vs-agreement`
- `how-do-you-test-for-strategic-alignment-before-execution-begins`
- `how-do-you-translate-strategy-into-operational-behavior-change`

Why these matter:

- leadership teams often recognize themselves immediately in these questions
- they support discovery questions and trust-building
- they are strong for qualified prospects

### Trust, Silence, And Signal Loss

- `why-do-employees-stop-telling-leaders-the-truth`
- `whats-the-difference-between-trust-and-psychological-safety`
- `why-do-engagement-surveys-show-high-trust-but-people-dont-speak-up`
- `why-do-well-intentioned-leaders-miss-early-warning-signs-of-risk`

Why these matter:

- they connect directly to the value of a voice-led diagnostic
- they help explain why surveys alone can miss reality
- they are strong trust-building topics for skeptical visitors

### Cross-Team Friction

- `how-to-break-down-silos-without-reorganizing`
- `what-causes-collaboration-theater-versus-genuine-collaborative-work`
- `how-incentive-structures-undermine-cross-functional-collaboration`
- `how-to-measure-cross-team-collaboration-effectiveness`

Why these matter:

- these are common and recognizable pains
- they are easy to connect to real buyer situations
- they help the bot ask better probing questions

### Role Clarity And Accountability

- `how-to-create-accountability-without-blame-culture`
- `what-causes-accountability-theater-versus-real-accountability`
- `how-to-define-ownership-cross-functional-initiatives`
- `how-to-match-authority-with-responsibility`

Why these matter:

- these show that WattNext understands real execution friction
- they are useful for discovery and objection handling

### Decision Quality

- `how-to-speed-up-decision-making-without-sacrificing-quality`
- `what-causes-gap-between-decision-and-execution`
- `why-decisions-get-escalated-unnecessarily`

Why these matter:

- these are highly relevant to CEOs and leadership teams
- they help the bot talk about friction in business terms, not just culture terms

## Tier 2: Use Soon After

These are good sources, but slightly less essential for the first release.

### Knowledge Management

- `what-causes-knowledge-silos`
- `what-causes-knowledge-hoarding-in-organizations`
- `how-do-you-capture-tacit-knowledge`
- `how-do-you-make-documentation-findable`
- `why-does-documentation-always-become-outdated`

Use for:

- later FAQ
- operations-heavy prospects
- more specific discovery conversations

### Process And Resourcing

- `why-dont-people-follow-documented-processes`
- `how-do-you-design-process-that-gets-followed`
- `how-do-you-know-when-process-is-too-rigid-vs-too-loose`
- `what-causes-the-peanut-butter-spread-of-resources`
- `how-do-you-know-if-you-have-resource-shortage-vs-resource-fragmentation`

Use for:

- more mature prospects
- operational leaders
- deeper follow-up conversations

### Leadership Pipeline And Change

- `why-do-great-individual-contributors-often-struggle-as-managers`
- `how-do-you-support-leadership-transitions`
- `what-do-new-hires-learn-in-their-first-90-days`

Use for:

- narrower use cases
- later-stage conversations
- content expansion

## Tier 3: Probably Not First-Release Website Bot Topics

These may still be excellent knowledge assets, but they are less likely to belong in an early public voice-bot experience unless the user asks very specific questions.

- highly technical resilience questions
- deep internal capability-development questions
- specialized documentation and support-system questions
- topics that need long, nuanced explanation to be safe and useful

Examples:

- `how-often-should-you-test-recovery-plans`
- `how-do-you-build-graceful-degradation`
- `how-do-you-reduce-support-burden-without-reducing-support-quality`
- `how-do-you-prepare-people-for-leadership-before-promoting-them`

These are better treated as later knowledge expansion or written content sources.

## Best Uses By Website-Agent Job

### Best for `company overview` and `problem patterns`

- `what-is-organizational-friction-and-why-does-it-persist`
- `what-makes-organizational-issues-systemic-rather-than-individual`
- `what-causes-execution-gaps-between-strategy-and-day-to-day-work`

### Best for `trust and proof`

- `why-do-employees-stop-telling-leaders-the-truth`
- `whats-the-difference-between-trust-and-psychological-safety`
- `why-do-well-intentioned-leaders-miss-early-warning-signs-of-risk`

### Best for `discovery mode`

- `why-do-leadership-teams-think-theyre-aligned-when-theyre-not`
- `alignment-vs-agreement`
- `how-to-break-down-silos-without-reorganizing`
- `how-to-create-accountability-without-blame-culture`
- `how-to-speed-up-decision-making-without-sacrificing-quality`

### Best for `skeptical visitor`

- `why-do-engagement-surveys-show-high-trust-but-people-dont-speak-up`
- `what-makes-organizational-issues-systemic-rather-than-individual`
- `why-do-organizational-problems-keep-reappearing-after-interventions`

## Extraction Guidance

When pulling from the canonical Q&A repo into the website-agent knowledge base:

1. Prefer the `Short Answer` first.
2. Compress long explanations into spoken form.
3. Avoid turning the bot into a lecture.
4. Keep the diagnostic mindset, but route toward a next step.
5. Where needed, combine canonical Q&A with primary product sources so the bot can bridge from:
   - problem explanation
   - to ViVo Pulse
   - to calculator, report, or meeting

## Recommended Next Drafting Pass

Start with these 10:

1. `what-is-organizational-friction-and-why-does-it-persist`
2. `what-causes-execution-gaps-between-strategy-and-day-to-day-work`
3. `what-makes-organizational-issues-systemic-rather-than-individual`
4. `why-do-organizational-problems-keep-reappearing-after-interventions`
5. `why-do-leadership-teams-think-theyre-aligned-when-theyre-not`
6. `alignment-vs-agreement`
7. `why-do-employees-stop-telling-leaders-the-truth`
8. `whats-the-difference-between-trust-and-psychological-safety`
9. `how-to-break-down-silos-without-reorganizing`
10. `how-to-speed-up-decision-making-without-sacrificing-quality`
