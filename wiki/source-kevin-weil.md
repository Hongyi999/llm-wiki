---
title: "Source: OpenAI's CPO on how AI changes must-have skills, moats, coding, startup playbooks, more | Kevin Weil"
type: source
created: 2026-04-12
updated: 2026-04-12
tags: [openai, evals, product-management, ai-product-development, model-maximalism, fine-tuning, chatgpt, vibe-coding]
guest: "Kevin Weil"
publish_date: 2025-04-10
duration: "1:31:41"
sources: [lenny-podcast/kevin-weil.md]
---

# Source: OpenAI's CPO on how AI changes must-have skills, moats, coding, startup playbooks, more | Kevin Weil

**Guest**: Kevin Weil
**Published**: 2025-04-10
**Duration**: 1:31:41
**YouTube**: https://www.youtube.com/watch?v=scsW6_2SPC4

## Executive summary

Kevin Weil, CPO of OpenAI, shares how the rapid pace of model improvement fundamentally changes product development, making traditional roadmapping obsolete and requiring teams to embrace ambiguity and iterative deployment. He argues that writing evals is becoming a core PM skill because AI products must be designed differently depending on whether the model gets something right 60%, 95%, or 99.5% of the time. Weil advocates for 'model maximalism' -- building at the edge of current capabilities knowing the next model will close the gap -- and explains how OpenAI uses ensembles of fine-tuned models internally rather than relying on a single general-purpose model. He also discusses why chat is an enduring interface for AI, the importance of bottoms-up empowered teams, and why the future of product teams will include researchers as core members working alongside PMs and engineers.

## Key ideas

1. **Evals as a core PM skill**: Because LLMs produce fuzzy outputs at varying reliability levels, product teams must design evals (unit tests for models) to measure how well models perform on specific use cases. The product you build at 60% accuracy is fundamentally different from one at 99.5%, and evals are the mechanism for tracking and improving that number over time.
2. **Model maximalism and iterative deployment**: OpenAI's philosophy is to build at the bleeding edge of current model capabilities rather than adding scaffolding for limitations, because a better model will arrive in roughly two months. This means launching early, iterating in public, and co-evolving with users rather than waiting for perfection.
3. **Ensembles of fine-tuned models**: Rather than sending all tasks to one general model, OpenAI internally breaks problems into specific sub-tasks and uses different models (varying in size, cost, and specialization) for each. This mirrors how companies are ensembles of specialized humans, and Weil believes every product team will eventually include researchers to fine-tune models for their specific use cases.
4. **Chat as a universal interface**: Contrary to the popular belief that chat is a placeholder UI, Weil argues it is the most versatile interface possible because it mirrors unrestricted human communication. It works across all intelligence levels and use cases, serving as a catch-all for any interaction that falls outside prescribed workflows.
5. **Human reasoning as a design heuristic for AI UX**: When designing AI product experiences (like the thinking animation for reasoning models or brainstorming with model ensembles), reasoning about how a human would behave in the same situation turns out to be a surprisingly effective design heuristic.

## Entities

- **Kevin Weil** — CPO of OpenAI, formerly head of product at Instagram and Twitter, sharing how OpenAI builds products and where the AI industry is heading.
- [[openai]] — The AI company at the center of the discussion, building ChatGPT, the API, and frontier models.
- **Sam Altman** — CEO of OpenAI, described as pushing teams to move fast while tolerating mistakes.
- [[anthropic]] — Competitor acknowledged for strong coding models, particularly Claude Sonnet.
- [[chatgpt]] — OpenAI's flagship consumer product with 400M+ weekly active users, discussed as a platform for AI interaction.
- **Libra (Diem)** — Facebook's cryptocurrency project led by Weil that failed due to regulatory and reputational challenges, described as his biggest career disappointment.
- **Waymo** — Referenced as an example of how miraculous technology quickly becomes normalized.

## Concepts & frameworks

- [[ai-evals|Evals]] — Systematic tests or benchmarks for measuring model performance on specific tasks, analogous to unit tests for software but applied to AI model capabilities.
- **Model Maximalism** — The philosophy of building products at the frontier of current model capabilities rather than engineering around limitations, trusting that better models will arrive soon.
- [[product-velocity-ai-era|Iterative Deployment]] — OpenAI's practice of shipping early and co-evolving with users in public rather than perfecting products internally before release.
- [[ai-coding-tools|Vibe Coding]] — A coding approach where developers let AI write most of the code with minimal intervention, accepting suggestions rapidly and pasting errors back for fixes.
- [[post-training-data-moat|Fine-tuning]] — The process of giving a model examples of desired input-output pairs to specialize it for a particular use case or domain.
- **Model Ensembles** — Using multiple specialized models of varying sizes and capabilities to solve different sub-tasks within a larger problem, analogous to a team of specialists.

## Memorable quote

> Kevin Weil (00:00:00): 'The AI models that you're using today is the worst AI model you will ever use for the rest of your life, and when you actually get that in your head, it's kind of wild.'

## B2 angle

Provides the foundational model provider's perspective on how product teams should build with LLMs, uniquely arguing that every company will need fine-tuned model ensembles and that evals will become the core PM skill of the AI era.

## See also

- [[index-by-theme]] — batch plan (this source is in **B2: AI products & LLMs 2024 and earlier**)
- [[synthesis-b2-ai-product-patterns]] — cross-source patterns from B2
- [[comparison-b2-ai-product-approaches]] — how B2 guests differ on AI product strategy
