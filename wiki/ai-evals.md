---
title: AI Evals
type: concept
created: 2026-04-11
updated: 2026-04-11
tags: [ai-engineering, ai-products, ai-evals, post-training]
sources: [lenny-podcast/hamel-husain-shreya-shankar.md, lenny-podcast/aishwarya-naresh-reganti-kiriti-badam.md, lenny-podcast/brendan-foody.md, lenny-podcast/chip-huyen.md, lenny-podcast/edwin-chen.md, lenny-podcast/jason-droege.md, lenny-podcast/sander-schulhoff-20.md]
---

# AI Evals

The practice of systematically measuring whether an AI product does what users need. In B1 (AI products 2025+), evals are the **single most-cited "core skill" for AI product builders** — appearing substantively in 7 of 29 transcripts.

## Canonical methodology

From [[source-hamel-husain-shreya-shankar|Hamel Husain & Shreya Shankar's episode]] (the definitive B1 evals episode):

1. **Ship something, collect real user interactions.** You can't eval what doesn't exist.
2. **Open coding** — manually read logs, tag failure modes with free-form labels.
3. **Axial coding** — cluster the open codes into structured failure categories.
4. **Theoretical saturation** — keep reading until new logs no longer introduce new failure modes. This is your target coverage.
5. **Write binary LLM-as-judge evals** for each failure category.
6. **Iterate.** Evals are never done; they evolve with the product.

Hamel's consulting frame: evals *are* the PRD. If you can't describe the eval, you don't know what you're building.

## Contrasting views across B1

| Source | Stance on evals |
|---|---|
| [[source-hamel-husain-shreya-shankar|Hamel & Shreya]] | Evals are the **core discipline** of AI engineering — everything else flows from them. |
| [[source-brendan-foody|Brendan Foody (Mercor)]] | Evals are the **product bottleneck** — frontier labs pay PhDs to write them because they limit deployment. See [[mercor]]. |
| [[source-aishwarya-naresh-reganti-kiriti-badam|Aishwarya & Kiriti]] | Evals are **necessary but not sufficient** — they can miss non-deterministic production failures that only surface via user feedback. |
| [[source-chip-huyen|Chip Huyen]] | Evals catch regressions but are **no substitute for talking to users**; she's skeptical of eval-heavy teams. |
| [[source-edwin-chen|Edwin Chen (Surge)]] | Evals encode values — your eval set *is* your product's personality. |
| [[source-jason-droege|Jason Droege]] | Enterprise evals are **domain-specific**; generic benchmarks don't matter for real customers. |
| [[source-sander-schulhoff-20|Sander Schulhoff]] | Evals **fundamentally don't catch adversarial attacks** (jailbreaks, prompt injection) — evals are for friendly users. |

## B1 consensus

- Evals are the bottleneck between "impressive demo" and "deployed product."
- Evals must be **written by domain experts**, not crowdsourced labelers — this is why [[mercor|Mercor]] and [[scale-ai|Scale AI]] pivoted to expert-human supply.
- LLM-as-judge is the current standard technique, with calibration against human ground truth.
- **Evals are the new PRD**: they define what the product is supposed to do, more precisely than any doc.

## Open disagreements

- Are evals the *start* of the process (Hamel) or the *last* step after user research (Chip)?
- Do evals replace user research (some AI startups claim) or complement it (most B1 guests)?
- Can generic evals generalize, or must every domain have its own? (Jason Droege says no to generic.)

## See also

- [[post-training-data-moat]] — why evals and post-training data are the same market.
- [[mercor]] / [[scale-ai]] — expert labelers who write evals.
- [[product-velocity-ai-era]] — fast iteration depends on fast evals.
- [[source-sander-schulhoff-20]] — what evals *can't* do (adversarial robustness).
