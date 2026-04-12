---
title: Anthropic
type: entity
created: 2026-04-11
updated: 2026-04-12
tags: [ai-lab, foundation-models, claude]
sources: [lenny-podcast/edwin-chen.md, lenny-podcast/hamel-husain-shreya-shankar.md, lenny-podcast/amjad-masad.md, lenny-podcast/eric-simons.md, lenny-podcast/karina-nguyen.md, lenny-podcast/kevin-weil.md, lenny-podcast/mike-krieger.md]
---

# Anthropic

Frontier AI lab, maker of Claude. Frequently paired with [[openai|OpenAI]] as the two leading labs — 2 B1 sources and 5 B2 sources (7 total). In B2, Anthropic's role expands beyond "values-differentiated alternative" to become **the dominant coding model provider**: Claude Sonnet is the model powering [[bolt|Bolt]], [[replit|Replit]], and acknowledged by [[openai|OpenAI]]'s own CPO as the strongest coding competitor.

## B1 appearances

- [[source-edwin-chen]] — Edwin contrasts **Anthropic's** objective function choices with OpenAI's: the two labs explicitly teach different values via post-training data, producing measurably different model behaviors. Edwin argues this is the deepest form of [[post-training-data-moat|model differentiation]].
- [[source-hamel-husain-shreya-shankar]] — Hamel and Shreya use **Claude** as one of several models when discussing [[ai-evals|LLM-as-judge]] setups and error analysis methodology.

## B1 framing

In B1 Anthropic is the go-to example that *how* you do post-training matters as much as *how much* compute you have. Edwin Chen's episode is the most detailed: different labs make different calls about what behaviors to reinforce, and those calls compound into distinct model personalities that users can feel.

## B2 appearances

- [[source-mike-krieger|Mike Krieger]] — **Anthropic's CPO** (co-founder of Instagram). Reveals that 90%+ of Anthropic's code is now AI-written; Claude Code uses Claude Code to build itself. The bottleneck has migrated from engineering to decision-making.
- [[source-eric-simons|Eric Simons]] — **Claude Sonnet** was the model that unlocked production-quality AI coding and enabled [[bolt|Bolt]]'s explosive growth. Eric describes the specific moment Sonnet crossed the quality threshold.
- [[source-amjad-masad|Amjad Masad]] — [[replit|Replit]] uses Claude Sonnet as the primary foundation model for its coding agent, described as "the best coding model."
- [[source-karina-nguyen|Karina Nguyen]] — Former Anthropic employee where she learned model craft, post-training methodology, and built the 100K context file upload feature for Claude.
- [[source-kevin-weil|Kevin Weil]] — **OpenAI's CPO** acknowledges Anthropic for strong coding models, particularly Claude Sonnet, as a direct competitor.

## See also

- [[openai]] — the other frontier lab, usually compared side-by-side.
- [[post-training-data-moat]] — why the post-training layer is where differentiation now lives.
- [[ai-evals]] — methodology for measuring the differences Anthropic and OpenAI encode.
- [[ai-coding-tools]] — Claude Sonnet powers multiple B2 AI coding tools.
