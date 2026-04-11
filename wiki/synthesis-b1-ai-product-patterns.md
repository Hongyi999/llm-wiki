---
title: "Synthesis: B1 AI Product Patterns"
type: synthesis
created: 2026-04-11
updated: 2026-04-11
tags: [ai-products, synthesis, b1]
sources: [lenny-podcast/aishwarya-naresh-reganti-kiriti-badam.md, lenny-podcast/asha-sharma.md, lenny-podcast/brandon-chu.md, lenny-podcast/brendan-foody.md, lenny-podcast/bret-taylor.md, lenny-podcast/brian-balfour.md, lenny-podcast/chip-huyen.md, lenny-podcast/dan-shipper.md, lenny-podcast/dhanji-r-prasanna.md, lenny-podcast/dr-fei-fei-li.md, lenny-podcast/dylan-field.md, lenny-podcast/edwin-chen.md, lenny-podcast/elena-verna-40.md, lenny-podcast/eoghan-mccabe.md, lenny-podcast/ethan-smith.md, lenny-podcast/garrett-lord.md, lenny-podcast/grant-lee.md, lenny-podcast/hamel-husain-shreya-shankar.md, lenny-podcast/howie-liu.md, lenny-podcast/jason-droege.md, lenny-podcast/jason-m-lemkin.md, lenny-podcast/julian-shapiro.md, lenny-podcast/julie-zhuo.md, lenny-podcast/madhavan-ramanujam.md, lenny-podcast/nick-turley.md, lenny-podcast/nicole-forsgren.md, lenny-podcast/robby-stein.md, lenny-podcast/sander-schulhoff-20.md, lenny-podcast/tomer-cohen.md]
---

# Synthesis: B1 AI Product Patterns

Cross-source patterns that appear in at least 3–4 of the 29 [[index-by-theme|B1 (AI products 2025+)]] transcripts. This is the "what they agree on, whether or not they say it" layer. See [[comparison-b1-ai-product-approaches]] for the explicit disagreements.

## Pattern 1: Evals are the new PRD

Across [[source-hamel-husain-shreya-shankar|Hamel & Shreya]], [[source-brendan-foody|Brendan Foody]], [[source-chip-huyen|Chip Huyen]], [[source-aishwarya-naresh-reganti-kiriti-badam|Aishwarya & Kiriti]], [[source-edwin-chen|Edwin Chen]], [[source-jason-droege|Jason Droege]], and [[source-sander-schulhoff-20|Sander Schulhoff]], the consensus is clear: **you cannot build an AI product without evals, and evals are more definitional than any written spec.** The PRD of the AI era is a test set you can run against. This is the B1 signature shift from "describe what to build" to "define what it must pass."

Corollary: [[ai-evals|evals and post-training data are the same market]], which is why [[mercor|Mercor]], [[scale-ai|Scale AI]], and [[source-garrett-lord|Handshake]] are all converging on expert-human labeling. See [[post-training-data-moat]].

## Pattern 2: Outcomes replace seats

Across [[source-bret-taylor|Bret Taylor]] (Sierra), [[source-madhavan-ramanujam|Madhavan Ramanujam]], [[source-eoghan-mccabe|Eoghan McCabe]] (Intercom Fin), [[source-elena-verna-40|Elena Verna]], and [[source-dan-shipper|Dan Shipper]] (Every), there is strong agreement that **per-seat pricing structurally underprices AI**. When software completes a job, it should be paid from the labor budget (10-100x bigger), not the software budget. The near-term move is [[outcomes-based-pricing]]; the controversy is only about timing.

## Pattern 3: Agents > chat, with human oversight

Seven B1 guests ([[source-bret-taylor|Bret]], [[source-nick-turley|Nick]], [[source-eoghan-mccabe|Eoghan]], [[source-asha-sharma|Asha]], [[source-dhanji-r-prasanna|Dhanji]], [[source-jason-droege|Jason]], [[source-dan-shipper|Dan]]) agree that **agents are the new primary form factor** for AI products, replacing chat interfaces. Every single one of them adds the constraint "with human oversight somewhere in the loop" — not because of philosophy but because of [[source-sander-schulhoff-20|Sander Schulhoff's]] warning that agents scale the blast radius of prompt injection and jailbreaks. See [[ai-agents]].

## Pattern 4: Post-training is the moat, not pre-training

Six guests converge explicitly on this ([[source-chip-huyen|Chip]], [[source-brendan-foody|Brendan]], [[source-edwin-chen|Edwin]], [[source-garrett-lord|Garrett]], [[source-jason-droege|Jason]], [[source-asha-sharma|Asha]]). **Pre-training has saturated; post-training is where differentiation now lives.** Post-training is:
- Expensive (requires expert human judgment)
- Values-laden (encodes what the lab considers "good behavior")
- Domain-specific (what works for code doesn't work for law)
- **The single largest AI data market by revenue in 2025–2026**.

This is the underlying reason [[mercor|Mercor]] and Handshake grew to 9-figure revenues in under 2 years. See [[post-training-data-moat]].

## Pattern 5: AI-native org restructuring, top-down

Seven guests ([[source-tomer-cohen|Tomer]], [[source-dhanji-r-prasanna|Dhanji]], [[source-julie-zhuo|Julie]], [[source-dan-shipper|Dan]], [[source-howie-liu|Howie]], [[source-eoghan-mccabe|Eoghan]], [[source-asha-sharma|Asha]]) describe variants of the same pattern: **restructuring the company from the top down around AI as a first-class teammate.** Consistent design moves:
- Functional org over divisional.
- New roles (Full Stack Builder, Head of AI Ops).
- Manager as orchestrator of mixed human-AI teams.
- Top-down mandate over grassroots adoption.
- "Builders" replaces distinct "PM / designer / engineer" identities.

[[source-dhanji-r-prasanna|Dhanji]] is most explicit: *grassroots AI adoption alone does not work at scale; you must mandate it.* See [[ai-native-organization]].

## Pattern 6: Ship daily, discover product empirically

Eight guests ([[source-nick-turley|Nick]], [[source-dan-shipper|Dan]], [[source-grant-lee|Grant]], [[source-robby-stein|Robby]], [[source-elena-verna-40|Elena]], [[source-brian-balfour|Brian]], [[source-howie-liu|Howie]], [[source-asha-sharma|Asha]]) describe cultures where **daily shipping is the source of product discovery**, not a consequence of it. The strategy doc comes *after* shipping, not before. Quarterly roadmaps are anti-patterns. See [[product-velocity-ai-era]].

Related: [[source-chip-huyen|Chip Huyen's]] warning that most teams mistake "keeping up with AI news" for "making progress on product." The answer is: ship to real users every day.

## Pattern 7: Non-engineers benefit more than engineers

Multiple guests ([[source-dhanji-r-prasanna|Dhanji]], [[source-julie-zhuo|Julie]], [[source-dan-shipper|Dan]], [[source-chip-huyen|Chip]]) independently observe that **AI productivity gains are larger for non-technical roles** (product, ops, support, design, writing) than for engineers. The intuition: engineers already have muscle memory and skepticism; non-engineers have neither, so they accept more AI help and realize more benefit.

## Pattern 8: Craft and taste become the moat (paradoxically)

When AI commoditizes execution, **judgment about what to make becomes the differentiator**. [[source-dylan-field|Dylan Field]] ([[figma|Figma]]) is the loudest voice; [[source-brandon-chu|Brandon Chu]] (writing), [[source-julie-zhuo|Julie Zhuo]] (design management), and [[source-nicole-forsgren|Nicole Forsgren]] (developer craft) echo the pattern. The surprising lesson: *the more AI writes your code / designs your UI / drafts your copy, the more valuable the person who decides which output is actually worth shipping.*

## Pattern 9: Disruption is violent

Multiple guests warn that AI transition is not gradual. [[source-eoghan-mccabe|Eoghan McCabe]] says it explicitly: "AI bet or death." [[source-brian-balfour|Brian Balfour]] frames it as **platform cycle theory** — new platforms reset market leadership every few years and missing a cycle is fatal. [[source-elena-verna-40|Elena Verna]] frames it as the **pioneer-to-majority gap risk**. The pattern is consistent: *slow adoption is worse than no adoption, because it wastes the window.*

## Anti-signals: what B1 guests agree you should NOT do

- **Obsess over model news instead of user feedback.** ([[source-chip-huyen|Chip]])
- **Optimize for code quality.** ([[source-dhanji-r-prasanna|Dhanji]]: uncorrelated with product success.)
- **Pre-write PRDs, then build.** ([[source-nick-turley|Nick]], [[source-dan-shipper|Dan]]: ship first, discover second.)
- **Default to per-seat pricing for AI that completes jobs.** ([[source-bret-taylor|Bret]], [[source-madhavan-ramanujam|Madhavan]])
- **Rely on guardrails for safety.** ([[source-sander-schulhoff-20|Sander]]: they fail.)
- **Do AI transformation bottom-up.** ([[source-dhanji-r-prasanna|Dhanji]], [[source-eoghan-mccabe|Eoghan]])
- **Mix fast and slow teams.** ([[source-howie-liu|Howie]])
- **Wait for more data before shipping.** ([[source-hamel-husain-shreya-shankar|Hamel & Shreya]]: ship, then eval on real traffic.)

## Meta-pattern: AI is a crisis that rewards decisiveness

The deepest pattern in B1 is emotional, not technical. The guests who are winning are the ones who **made a clear bet early, restructured to support it, and shipped against it every day**. The guests who are losing (or warning others about losing) are the ones who hedged, waited for more clarity, or tried to bolt AI onto existing products and orgs.

The most quoted sentiment, across multiple episodes, is some version of *"we might be wrong, but we are not confused"* ([[source-tomer-cohen|Tomer Cohen]]). In the B1 era, confusion kills; confident wrongness at least produces learning.

## Questions B1 does not answer

- How do you balance [[product-velocity-ai-era|daily shipping]] with [[source-sander-schulhoff-20|Sander's]] security warnings in practice?
- Does this velocity and restructuring work past ~500 engineers? No B1 guest speaks from that scale.
- What happens to the post-training data market if synthetic data catches up? ([[source-jason-droege|Jason Droege]] hedges.)
- Who owns the liability when an agent takes a harmful action? (Not addressed.)
- Is the "vibe over benchmarks" culture sustainable for safety-critical products? (Sander says no; most others ignore the question.)

## See also

- [[comparison-b1-ai-product-approaches]] — the explicit disagreements.
- [[index-by-theme]] — the full B1 list with links back to source pages.
- [[ai-evals]], [[ai-agents]], [[outcomes-based-pricing]], [[post-training-data-moat]], [[ai-native-organization]], [[product-velocity-ai-era]] — the six cross-source concepts derived from this batch.
