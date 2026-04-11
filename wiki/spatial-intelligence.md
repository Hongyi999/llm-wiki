---
title: Spatial Intelligence
type: concept
created: 2026-04-11
updated: 2026-04-11
tags: [ai-research, 3d-ai, world-models, robotics, fei-fei-li]
sources: [lenny-podcast/dr-fei-fei-li.md]
---

# Spatial Intelligence

The ability to **create, reason about, interact with, and understand 3D and 4D worlds** — as distinct from language understanding (LLMs) or video prediction (generative video models). [[source-dr-fei-fei-li|Dr. Fei-Fei Li]] is the concept's primary advocate and founder of [[world-labs|World Labs]], which is building products around it.

## Why language models aren't enough

From [[source-dr-fei-fei-li]]:

- **LLMs are trained on text**; they know the world only through descriptions of it, not through perception of it.
- **Video generation models predict pixels**, but lack *structure*: they can't tell you where objects are, how they connect, or what happens if you push one. Prediction ≠ understanding.
- **World models** generate environments that can be **navigated, manipulated, and reasoned about** — the way a human imagines a room they've never been in. This is the missing capability that unlocks robotics, game design, scientific simulation, and embodied AI.

## Why it's hard

Unlike language, spatial intelligence cannot be solved by scaling pre-training on internet data:

- **Data is missing.** Most internet data has no 3D structure, no action labels, no physics.
- **Bitter lesson has limits.** Scaling compute + data works for language and vision because both are abundant and well-labeled. 3D/4D data is scarce; synthetic data and teleoperation are required.
- **Physical embodiment introduces irreducible complexity.** A robot that picks up an object must model friction, compliance, occlusion — things no video dataset teaches.
- **20-year analogy to self-driving cars.** Self-driving is a *simpler* robotics problem (2D, no manipulation) and it still took 20 years of work with limited rollout. True robots will take longer.

## What it enables

- **Robotics** — robots that plan and manipulate in unfamiliar environments.
- **Game and VFX creation** — prompt-to-world for creative tools (World Labs' [[world-labs|Marble]] product).
- **Scientific simulation** — biology, drug discovery, climate modeling.
- **Accessibility and therapy** — Fei-Fei mentions immersive therapy environments as a current use case.
- **Human-centered AI** — spatial models let ordinary people interact with AI in physical space, not just via screens.

## Relationship to LLMs

Fei-Fei's framing is not "spatial replaces language" but "both are required for general intelligence." Language models handle abstract reasoning and communication; world models handle perception, action, and physical understanding. A complete AI system composes both.

## See also

- [[world-labs]] — the company built around this concept.
- [[source-dr-fei-fei-li]] — the B1 episode.
- [[post-training-data-moat]] — related discussion of what data is actually scarce.
