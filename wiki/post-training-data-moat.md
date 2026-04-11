---
title: Post-Training Data as Moat
type: concept
created: 2026-04-11
updated: 2026-04-11
tags: [ai-products, ai-data, post-training, foundation-models]
sources: [lenny-podcast/brendan-foody.md, lenny-podcast/asha-sharma.md, lenny-podcast/chip-huyen.md, lenny-podcast/edwin-chen.md, lenny-podcast/garrett-lord.md, lenny-podcast/jason-droege.md]
---

# Post-Training Data as Moat

The thesis that in 2025+ the key differentiator between frontier AI models is **post-training** (RLHF, supervised fine-tuning, reinforcement learning from expert feedback), not **pre-training** on scraped web data. Expert human judgment is therefore the new scarce resource — and the companies that can efficiently supply it to frontier labs are in a defensible position.

## Why post-training matters now

[[source-chip-huyen|Chip Huyen]] (NVIDIA NeMo) makes the most explicit version: **pre-training has hit saturation** on available internet data. Additional gains from bigger pre-training runs are diminishing. But post-training — where the raw model is shaped into a useful assistant — is still far from its ceiling. Post-training is where models learn:

- What behaviors to reinforce (helpful vs. harmful, direct vs. hedged)
- Domain-specific competence (code, math, medical, legal)
- Safety and refusal patterns
- "Personality" and tone

## The data market pivot

Six B1 guests describe the same industry shift from different angles:

| Source | Perspective | Key claim |
|---|---|---|
| [[source-brendan-foody|Brendan Foody]] ([[mercor|Mercor]]) | New entrant | Frontier labs will pay $100/hr+ for PhDs to write evals and grade outputs — impossible with [[scale-ai|Scale AI's]] original labeler pool. Mercor grew $1M → $500M ARR in 17 months. |
| [[source-garrett-lord|Garrett Lord]] ([[source-garrett-lord|Handshake]]) | Adjacent pivot | Handshake's 18M-student network (including PhD candidates) is an "audience as unfair advantage" for expert labeling. $50M in 4 months after pivot. |
| [[source-jason-droege|Jason Droege]] (ex-[[scale-ai]]) | Incumbent view | Even Scale pivoted: 80%+ of its workforce now has a bachelor's degree, up from near-zero at founding. The commodity-labeling era is over. |
| [[source-edwin-chen|Edwin Chen]] (Surge AI) | Values-first | Post-training data is how you *teach values* to a model. Labs diverge on values, and that divergence produces distinct model personalities. Worth building a company around. |
| [[source-chip-huyen|Chip Huyen]] (NVIDIA NeMo) | Technical | Pre-training vs post-training asymmetry is the single most important concept for AI engineers to internalize. |
| [[source-asha-sharma|Asha Sharma]] (Microsoft AI) | Buyer side | The post-training economics reshape model-supplier relationships; cost-to-train is dominated by human feedback, not compute. |

## Convergent claims

1. **Expert human judgment is the new scarce resource.** Labels written by PhDs, doctors, lawyers, engineers — not clickworkers.
2. **Evals are the data.** [[ai-evals|Evals and post-training data are the same market]]: the examples you label to measure a model become the examples you train on next.
3. **Generic benchmarks are worthless.** Real differentiation comes from **domain-specific** data and evals.
4. **Model differentiation is now cultural.** Different labs teach different values; buyers should pick the lab whose values match their use case. This is [[source-edwin-chen|Edwin Chen's]] core claim.
5. **Bootstrapped research wins.** Edwin argues research-first, VC-light structures (like Surge) enable deeper work than venture-scaled labs.

## Open questions

- Is this moat durable, or will synthetic data eventually catch up? (Jason Droege: partly — synthetic helps but doesn't replace.)
- Will labs in-source expert labeling once it's strategic? (Some are already trying.)
- Can small AI product companies benefit from this, or only frontier labs? (Chip Huyen: yes — you can fine-tune on your own post-training data for your domain.)

## See also

- [[mercor]], [[scale-ai]] — the supply side.
- [[openai]], [[anthropic]], [[meta]] — the demand side.
- [[ai-evals]] — the adjacent discipline and the same market.
- [[source-edwin-chen]] — the values-teaching framing.
- [[source-chip-huyen]] — the technical framing.
