---
title: "Source: Anthropic's CPO on what comes next | Mike Krieger (co-founder of Instagram)"
type: source
created: 2026-04-12
updated: 2026-04-12
tags: [anthropic, ai-development, claude, product-strategy, coding-tools, mcp, ai-native-workflows]
guest: "Mike Krieger"
publish_date: 2025-06-05
duration: "1:06:22"
sources: [lenny-podcast/mike-krieger.md]
---

# Source: Anthropic's CPO on what comes next | Mike Krieger (co-founder of Instagram)

**Guest**: Mike Krieger
**Published**: 2025-06-05
**Duration**: 1:06:22
**YouTube**: https://www.youtube.com/watch?v=DKrBGOFs0GY

## Executive summary

Mike Krieger, CPO of Anthropic and co-founder of Instagram, offers a rare insider view of how product development transforms when 90% of your code is written by AI—a reality Anthropic has already reached. He reveals that the Claude Code team uses Claude Code to build Claude Code (likely 95%+ AI-written), that over 70% of Anthropic's pull requests are AI-generated, and that this has shifted bottlenecks from engineering to decision-making/alignment upstream and merge queue/deployment downstream. Krieger shares that Opus 4 was the first model to genuinely surprise him with novel strategic thinking, fundamentally changing his view on AI's capacity for creative, independent thought. He discusses how MCP (Model Context Protocol) will wire together the full product development loop from user feedback to pull request, and candidly addresses the OpenAI competitive dynamic, the future of skills in an AI world, and why he shut down Artifact.

## Key ideas

1. **90% AI-written code shifts bottlenecks, not eliminates them**: At Anthropic, engineering is no longer the bottleneck. Decision-making and strategic alignment upstream, and merge queues and deployment infrastructure downstream, are the new constraints. The merge queue had to be completely re-architected because AI-generated pull requests overwhelmed it.
2. **Claude Code building Claude Code is the frontier of AI-assisted development**: The Claude Code team operates in the most futuristic way at Anthropic—using Claude to build Claude in a self-improving loop. They've shifted from line-by-line code review to using another Claude instance for review, with humans doing acceptance testing rather than line-level inspection.
3. **Opus 4 crossed the threshold for genuinely novel strategic thought**: Krieger's go-to product strategy partner is Claude, and with Opus 4 combined with advanced research capabilities, it returned strategic insights he hadn't considered and immediately incorporated. This shifted his belief about AI's capacity for creative, independent thinking.
4. **MCP enables the full autonomous product development loop**: The vision is an AI that monitors user feedback channels, identifies problems, proposes solutions, generates pull requests, and spins up A/B tests—all autonomously. Krieger believes this is achievable in 2025, limited more by context plumbing than model capability.
5. **Nurturing curiosity and independent thought in children is the key skill for the AI era**: Rather than reaching for Claude to answer his kids' questions, Krieger asks 'how would we find out?' to preserve the process of inquiry and independent thinking—a skill both he and Shopify CEO Tobias Lütke independently identified as most important.

## Entities

- **Mike Krieger** — Chief Product Officer of Anthropic and co-founder of Instagram, leading product strategy at one of the most important AI companies.
- [[anthropic]] — AI safety company behind Claude, where 90%+ of code is now AI-written and the Claude Code team uses Claude Code to build itself.
- **Claude** — Anthropic's AI assistant, used internally as a product strategy partner and code generation tool.
- **Claude Code** — Anthropic's CLI tool for AI-assisted development, written in TypeScript, likely 95%+ self-authored by Claude.
- [[openai]] — Primary competitor discussed in the context of consumer mindshare dominance with ChatGPT.
- **Kevin Weil** — CPO of OpenAI who appeared on a panel with Krieger at the Lenny and Friends Summit.
- **Dario Amodei** — CEO of Anthropic, cited for making bold predictions about AI capabilities that keep coming true.
- **Artifact** — AI-powered news app co-founded by Krieger after leaving Meta, which he shut down before joining Anthropic.
- **MCP** — Model Context Protocol—Anthropic's open protocol for connecting AI models to external data and tools.
- **Opus 4** — Anthropic's latest frontier model that crossed the threshold for genuinely novel strategic thinking in Krieger's experience.

## Concepts & frameworks

- **Patient zero for AI-native development** — Anthropic describes itself as patient zero for the transformation of software development when the vast majority of code is AI-written.
- [[taste-as-differentiator|Bottleneck migration]] — When AI eliminates engineering as the bottleneck, constraints shift to upstream (decision-making, alignment) and downstream (merge queues, deployment, launch coordination).
- **Minimum viable strategy** — Krieger's concept of providing just enough strategic direction to let empowered teams explore at the edge of model capabilities.
- **AI 2027** — A speculative paper about near-term AI trajectories that Krieger found eerily convergent with his own product strategy documents.
- [[ai-coding-tools|SWE-Bench]] — A benchmark for AI coding capability where Anthropic went from 50% to ~72%, tracking toward Dario Amodei's prediction of 90% by end of 2025.

## Memorable quote

> Mike Krieger (00:00:03): 'The team that works in the most futuristic way is the Claude Code team. They're using Claude Code to build Claude Code in a very self-improving kind of way.'

## B2 angle

Provides the only insider account of what product development actually looks like when 90%+ of code is AI-written—revealing that the transformation is less about coding speed and more about reorganizing human decision-making around new bottlenecks.

## See also

- [[index-by-theme]] — batch plan (this source is in **B2: AI products & LLMs 2024 and earlier**)
- [[synthesis-b2-ai-product-patterns]] — cross-source patterns from B2
- [[comparison-b2-ai-product-approaches]] — how B2 guests differ on AI product strategy
