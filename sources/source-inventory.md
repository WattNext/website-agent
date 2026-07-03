# Source Inventory

This document tracks the source material that may feed the WattNext website agent.

Use it to decide:

- what is safe to promote into the approved knowledge base
- what is only useful as supporting reference
- what still needs validation before use

## Status Labels

- `primary`: preferred source for approved claims
- `supporting`: useful source for framing, examples, questions, or structure, but not automatically approved
- `reference-only`: useful context, prototype behavior, or inspiration, but should not drive approved claims on its own

## Current Source Stack

### 1. Google Drive AI/LLM knowledge base

- Status: `primary`
- Location: Google Drive directory indexed in `_INDEX - AI LLM Drive Directory`
- Best for:
  - approved messaging
  - company framing
  - product explanation
  - brand language
  - ICP context
- Notes:
  - this is the default upstream source of truth
  - if another source conflicts with it, Drive wins unless a newer version is explicitly approved

### 2. `WattNext/wattnext-canonical-knowledge`

- Status: `primary`
- Link: [WattNext/wattnext-canonical-knowledge](https://github.com/WattNext/wattnext-canonical-knowledge)
- Best for:
  - canonical Q&A
  - FAQ and answer-engine content
  - organizational-friction explanations
  - topic-level trust-building answers
  - structured knowledge extraction
- Notes:
  - this appears to be a major upstream source for question-and-answer content
  - the `canonical-q-and-a/` directory is especially relevant for website-agent knowledge work
  - likely stronger than scattered FAQ drafts for approved long-form Q&A content
  - should probably outrank Drive FAQ drafts when the question is specifically about canonical Q&A wording

### 3. `_INDEX - AI LLM Drive Directory`

- Status: `primary`
- Link: [AI LLM Drive Directory](https://docs.google.com/document/d/13yH9haXA5pPbhgaBWig2psmQB6xXxmn2nHtKvAJIA0k)
- Best for:
  - locating the correct Drive folders
  - understanding intended folder purpose
  - confirming that `01 Knowledge Base Sources` is where LLM knowledge inputs should live
- Notes:
  - useful as the routing map for the rest of the Drive material
  - not itself a main messaging source, but part of the source-of-truth system

### 4. `WattNext_Canonical_Knowledge_Base_Master.xlsx`

- Status: `primary`
- Link: [WattNext_Canonical_Knowledge_Base_Master.xlsx](https://drive.google.com/file/d/1KmkdLxe9SOkoXz0VCzYtApt1BzMGke7g)
- Best for:
  - canonical claims
  - reusable messaging
  - KB extraction
- Notes:
  - this looks like the strongest single candidate for the master source document
  - should be one of the first files reviewed in detail when content drafting begins

### 5. `07-wattnext-company-context.md`

- Status: `primary`
- Link: [07-wattnext-company-context.md](https://drive.google.com/file/d/172nmWfQVXgne1zGOpmtoUz50uXgPQ5in)
- Best for:
  - plain-English company explanation
  - public positioning summary
  - ViVo Pulse overview
  - target audience cues
  - tone guidance
- Notes:
  - based on public website review as of June 24, 2026
  - strong source for first-pass website-agent language
  - still derived from public-facing material, so internal-only details should not be inferred from it

### 6. `WattNext_Brand_Guidelines.docx`

- Status: `primary`
- Link: [WattNext_Brand_Guidelines.docx](https://drive.google.com/file/d/1ifmMFOcigBoXt7U8K5MP6Iw6Lv5GS2Gs)
- Best for:
  - tone
  - brand consistency
  - wording choices
- Notes:
  - should be used to keep the agent aligned with how WattNext wants to sound

### 7. `WattNext_ICP_Review_Brief.md`

- Status: `primary`
- Link: [WattNext_ICP_Review_Brief.md](https://drive.google.com/file/d/1YUSY2lpbJ6wM5QjWGushrXAr6_8fG46P)
- Best for:
  - ideal-customer-profile section
  - qualification prompts
  - wrong-fit filtering
- Notes:
  - likely important for deciding who the bot should and should not qualify aggressively

## Product, Proof, And Sales Support

### 8. `20260521_WattNext_AI_Pitch.pptx`

- Status: `supporting`
- Link: [20260521_WattNext_AI_Pitch.pptx](https://drive.google.com/file/d/16qSWZHHDW7WhYXix91-59CUH4SROuD8i)
- Best for:
  - positioning support
  - story framing
  - investor or high-level narrative
- Notes:
  - useful for narrative structure
  - should not override more direct source documents

### 9. ViVo Pulse report templates and examples

- Status: `supporting`
- Links:
  - [Full Report Template](https://drive.google.com/file/d/1Q3ozeaUY79JxTegyIEChg4XJbdwdYvgd)
  - [Full Report Example](https://drive.google.com/file/d/1AZHtAkULsMYexTcj_W81VpYxCcS1jbK9)
  - [Short Report Example](https://drive.google.com/file/d/1he19Rh1hnTn0l0PaQK8I7dttx4Hms0lU)
- Best for:
  - explaining what buyers receive
  - describing outputs
  - trust-building
  - product-explainer content
- Notes:
  - especially valuable for `What do we get?` and `What happens after the diagnostic?`
  - any claims drawn from examples should remain conservative and client-safe

### 10. `ViVo_Pulse_-_Objection_Handling_Sheet.pdf`

- Status: `supporting`
- Link: [Objection Handling Sheet](https://drive.google.com/file/d/1NFmS9JS-GpVIaE6TPN4rTNlXWi6gS2tw)
- Best for:
  - FAQ
  - objection handling
  - skeptical prospect routes
- Notes:
  - likely useful for trust-building responses and conversion logic
  - should be checked against approved public claims before promotion

### 11. `KB From Insights to Action 18:07:2025.pdf`

### 12. `FAQ Page for New Website`

- Status: `supporting`
- Link: [FAQ Page for New Website](https://docs.google.com/document/d/1wtwQKeJ-x-Qvv3EeCKBdbFVLRgpM-33dQlgAffRNdwI)
- Best for:
  - website FAQ draft structure
  - visitor-facing question phrasing
  - identifying priority public questions
- Notes:
  - useful working draft
  - should not outrank the GitHub canonical Q&A source if wording conflicts

### 13. `faq-knowledge.md`

- Status: `supporting`
- Link: [faq-knowledge.md](https://drive.google.com/file/d/12MWlNQGeQXAe02ABvTmh7tiJYYL9eXWD)
- Best for:
  - FAQ support material
  - question clustering
  - SEO and AEO-related answer framing
- Notes:
  - probably useful as a companion source
  - should be checked against the canonical GitHub repo before promotion

### 14. Canonical Q&A Drive files

- Status: `supporting`
- Links:
  - [Canonical Q&As Strategic Alignment](https://drive.google.com/file/d/1sI0g8V61pbTrkTTiM8TS-khOGoGLaywI)
  - [Canonical Q&As Trust & Integrity](https://drive.google.com/file/d/1ni-n4TQBpVWet1c8Os2zioeNzcQTN1w2)
  - [Canonical Q&As Featured Snippet set](https://drive.google.com/file/d/12xvrqBHA9apjlKxBegAh8yqFtc3QvSNa)
- Best for:
  - search-oriented Q&A phrasing
  - featured snippet style
  - topic coverage cross-checking
- Notes:
  - these may overlap heavily with the GitHub canonical knowledge repo
  - if duplicated, GitHub is likely the cleaner canonical source

- Status: `supporting`
- Link: [KB From Insights to Action](https://drive.google.com/file/d/19H-2PFsQIHycDWsWWD8Xu_EsgOp0f4RG)
- Best for:
  - methodology framing
  - value explanation
  - outcome language
- Notes:
  - likely useful for bridge language between diagnosis and action
  - should be validated against newer materials if phrasing feels dated

## Sales-Flow And Prototype Sources

### 15. `explore.wattnext.ai`

- Status: `reference-only`
- Link: [explore.wattnext.ai](https://explore.wattnext.ai/)
- Best for:
  - guided-sales-call flow ideas
  - demo behavior inspiration
  - interaction design
- Notes:
  - user described this as a guided sales-call tool that never fully went live
  - good for flow inspiration, not for canonical claims

### 16. Bolt project: `ViVo Pulse Sales Training Dashboard 2`

- Status: `reference-only`
- Link: [Bolt project](https://bolt.new/~/sb1-km8hfryk)
- Best for:
  - sales training ideas
  - objection patterns
  - question patterns
- Notes:
  - useful if the sales-training GitHub is sparse
  - should be treated as exploratory unless mirrored in stronger sources

### 17. `vivo-pulse-sales-script_1.html`

- Status: `supporting`
- Path: [vivo-pulse-sales-script_1.html](/Users/pollywatt/Dropbox/My%20Mac%20(MacBook-Pro-de-Polly.local)/Downloads/vivo-pulse-sales-script_1.html)
- Best for:
  - discovery questions
  - consequence framing
  - friction-calculator bridge
  - CTA sequencing
  - conversation-route design
- Notes:
  - very strong for conversation design
  - especially useful for:
    - talent churn
    - leadership clarity
    - internal friction
    - strategic delays
    - decision quality
    - change readiness
  - any quantitative or process claims should be checked against primary sources before promotion

## Working Material For Related AI Helpers

### 18. `08-ashley-llm-instructions.md`

- Status: `reference-only`
- Link: [08-ashley-llm-instructions.md](https://drive.google.com/file/d/17SlbAv_kHZAn04MhVoZui2ddJ2WqQYuu)
- Best for:
  - reasoning style
  - evidence discipline
  - tone for analysis
- Notes:
  - not a website-agent knowledge source directly
  - useful as an example of good instruction style and careful handling of uncertainty

### 19. `WattNext Social Media & Website Analysis Handbook`

- Status: `reference-only`
- Link: [Handbook README](https://drive.google.com/file/d/1E2h1t6pIBosiAOVXtw7FJpCCRexy3v27)
- Best for:
  - related company context
  - channel-review framing
  - training logic
- Notes:
  - adjacent rather than core
  - relevant mainly where the website agent overlaps with public positioning

## Destination Repo

### 20. `WattNext/website-agent`

- Status: `destination`
- Link: [WattNext/website-agent](https://github.com/WattNext/website-agent)
- Best for:
  - approved, cleaned, bot-ready content
  - conversation design
  - source tracking
- Notes:
  - this is where final approved knowledge should live
  - it is not currently a meaningful upstream content source

## Codex Project Outputs

### 21. Codex thread: `Build sales knowledge base`

- Status: `supporting`
- Thread: `Build sales knowledge base`
- Project area: `/Users/pollywatt/Documents/WattNext.AI`
- Best for:
  - synthesized sales knowledge structures
  - call-practice positioning
  - ICP targeting
  - objection handling
  - pricing-for-training framing
  - scenario design
  - roleplay and training logic
  - voice-agent notes
- Notes:
  - this thread appears to have produced a substantial `rag-kb` and `knowledge-bank-exports` set
  - outputs referenced in the thread include:
    - `01_positioning_for_call_practice`
    - `02_icp_and_call_targeting`
    - `04_objections_and_reframes`
    - `05_pricing_for_call_training`
    - `07_call_scenario_library`
    - `08_roleplay_scorecard`
    - `09_voice_agent_design_notes`
    - multiple ICP profile documents
  - also produced export bundles such as:
    - `sales-knowledge-bank-txt.zip`
    - `sales-training-resources-expanded.zip`
  - treat these as high-value synthesized material, but still validate claims against primary sources before promotion

### 22. Codex project area: `Knowledge Bank (md)`

- Status: `supporting`
- Project area: `/Users/pollywatt/Library/CloudStorage/GoogleDrive-polly@wattnext.org/My Drive/WattNext Shared Folder/Knowledge Bank (md)`
- Best for:
  - sales-assistant documentation
  - friction-calculator framing
  - cold-call guide structure
  - framemaking notes
  - onboarding and sales workspace organization
- Notes:
  - relevant threads in this area include:
    - `Plan sales assistant wiki`
    - `Clean up outdated Notion content`
  - surfaced or created materials include:
    - `Friction Calculator Sales Guide`
    - `Sales Assistant Cold Call Guide`
    - `Framemaking Sales Guide`
    - sales onboarding and workspace-linking material
  - useful for operational sales behavior and assistant training, less useful as canonical company truth

### 23. Codex project area: `WattNext.AI`

- Status: `supporting`
- Project area: `/Users/pollywatt/Documents/WattNext.AI`
- Best for:
  - upstream working documents
  - generated drafts and exports
  - AI-created sales and product support material
- Notes:
  - this appears to be the main local working project area tied to multiple WattNext Codex threads
  - likely contains intermediate files that later landed in Drive or GitHub
  - good source for recovery and cross-checking when a Drive or Notion document is incomplete

### 24. Codex project area: `Vibe Coding`

- Status: `supporting`
- Project area: `/Users/pollywatt/Documents/Vibe Coding.`
- Best for:
  - prototype funnel concepts
  - Bolt app experiments
  - conversion-oriented UI and interaction ideas
  - lead-capture mechanics
  - sales-entry tools such as calculators or blind-spot scans
- Notes:
  - relevant threads include:
    - `Create sales funnel tool`
    - `Edit bolt.new app`
  - the `Create sales funnel tool` thread produced a CEO-facing “Leadership Blind Spot Scan” prototype and later shifted it toward branded slider-based assessment flow
  - useful as a source of conversion and experience ideas, not as canonical truth for claims or product positioning

## Still To Confirm

### 25. Whether the Codex-generated exports should be copied into `website-agent`

- Status: `decision pending`
- Notes:
  - some of the exported `.txt` or `.md` materials may be worth copying or summarizing into `drafts/`
  - others may be better left as referenced upstream assets

### 26. `WattNext/sage`

- Status: `supporting`
- Link: [WattNext/sage](https://github.com/WattNext/sage)
- Best for:
  - implementation context
  - knowledge retrieval behavior
  - how WattNext already structures KB access
  - example prompts and question types
- Notes:
  - private repo
  - README confirms Sage is a Slack slash-command bot for answering WattNext knowledge-base questions
  - uses semantic search over a Supabase-backed KB, then synthesizes an answer
  - useful mainly for architecture and KB access patterns, not for canonical public messaging

### 27. `WattNext/sales-training`

- Status: `supporting`
- Link: [WattNext/sales-training](https://github.com/WattNext/sales-training)
- Best for:
  - roleplay and training flow
  - sales-conversation practice
  - discovery and objection-handling behavior
  - CTA and booking flow ideas
- Notes:
  - private repo
  - top-level README points directly to the Bolt project `ViVo Pulse Sales Training Dashboard 2`
  - `package.json` identifies the app as `vivo-pulse-roleplay-arena`
  - this suggests it is best treated as a conversation-design and sales-training source rather than a canonical claims source

## Recommended Next Use

The first drafting pass should probably pull from:

1. `WattNext/wattnext-canonical-knowledge`
2. `WattNext_Canonical_Knowledge_Base_Master.xlsx`
3. `07-wattnext-company-context.md`
4. `WattNext_Brand_Guidelines.docx`
5. `WattNext_ICP_Review_Brief.md`
6. ViVo Pulse report examples
7. objection-handling material
8. `vivo-pulse-sales-script_1.html` for conversation design only

## Promotion Rule

Before moving any content into `knowledge-base/`, confirm:

- is the underlying claim present in a `primary` source?
- if not, is it only being used as phrasing or conversation structure?
- if it is neither, keep it in `drafts/` until validated
