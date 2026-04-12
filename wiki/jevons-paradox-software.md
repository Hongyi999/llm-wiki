---
title: Jevons Paradox in Software
type: concept
created: 2026-04-12
updated: 2026-04-12
tags: [jevons-paradox, ai-coding, labor-market, software-economics, demand-elasticity]
sources: [lenny-podcast/amjad-masad.md, lenny-podcast/scott-wu.md]
---

# Jevons Paradox in Software

Jevons Paradox is the economic observation that when technological progress makes a resource cheaper to use, total consumption of that resource tends to increase rather than decrease. Originally formulated by William Stanley Jevons in 1865 about coal consumption, the paradox applies whenever efficiency gains unlock latent demand that dwarfs the savings. In the context of software, the argument is straightforward: as AI coding tools drive the cost of building software toward zero, the total amount of software produced -- and the total demand for people who can direct that production -- will explode rather than contract.

## Amjad Masad's framing: cheaper software, more software

[[source-amjad-masad|Amjad Masad]] applies Jevons Paradox directly to the economics of software creation. [[replit]] can now produce a full-stack application from a natural language prompt in under ten minutes for roughly fifteen cents of compute. At that price point, ideas that were never worth pursuing -- internal tools, one-off prototypes, niche consumer apps -- suddenly get built. Non-technical people (PMs, founders, operations teams) are already building tools they previously would have hired developers for.

Masad's complementary principle, "Amjad's Law," states that the ROI of learning to code doubles every six months. The implication is that even basic coding literacy (understanding app structure, prompting, debugging) becomes extraordinarily valuable, because each increment of human skill is amplified by rapidly improving AI. The bottleneck shifts from engineering capacity to **idea generation** -- the speed at which you can conceive, test, and iterate on product concepts.

## Scott Wu's framing: bricklayer to architect

[[source-scott-wu|Scott Wu]] arrives at the same conclusion from the supply side. [[devin]] enables engineers to shift from spending 90% of their time on implementation (debugging Kubernetes errors, fixing bugs, running migrations) to focusing on the 10% that matters most: defining problems, designing architecture, and specifying intent. Each engineer on Cognition's team works with up to five Devins simultaneously.

Wu predicts there will be **far more programmers in a few years, not fewer**, because humanity consistently finds more things to build software for. The demand for software far exceeds current capacity -- most businesses, workflows, and creative ideas that would benefit from custom software still lack it. As AI removes the implementation bottleneck, that latent demand surfaces.

## Where the two views converge

Both Masad and Wu agree on the core mechanism:

| Dimension | Masad (Replit) | Wu (Devin) |
|---|---|---|
| **Who builds** | Non-technical people gain access | Engineers become more productive |
| **What changes** | The cost floor drops to near-zero | The skill ceiling rises (architect, not bricklayer) |
| **Net effect** | More software gets built by more people | Each engineer tackles bigger, harder problems |
| **Bottleneck shift** | Idea generation replaces engineering capacity | Problem definition replaces implementation |

The shared prediction: total demand for software engineering talent increases, even as (or precisely because) per-unit cost collapses.

## Implications for the job market

1. **Role transformation, not elimination.** The engineer's job shifts toward architecture, specification, review, and taste. Implementation becomes delegable to AI agents.
2. **Broader participation.** People who were never "developers" -- PMs, designers, operators, domain experts -- can now ship working software, expanding the pool of builders.
3. **New bottlenecks emerge.** If coding is cheap, the scarce resources become product taste, problem selection, and the ability to evaluate AI output (see [[ai-evals]]).
4. **Historical precedent.** The pattern has played out before: spreadsheets did not eliminate accountants, CAD did not eliminate architects, and desktop publishing did not eliminate designers. Each tool expanded the market for the underlying skill.

## See also

- [[replit]] -- Amjad Masad's AI-powered development platform
- [[devin]] -- Cognition's autonomous AI software engineer
- [[ai-agents]] -- the broader agent paradigm that enables this shift
- [[product-velocity-ai-era]] -- how AI compresses development cycles
- [[ai-native-organization]] -- organizational restructuring around AI teammates
