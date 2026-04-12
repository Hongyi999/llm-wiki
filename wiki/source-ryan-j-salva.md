---
title: "Source: The role of AI in new product development | Ryan J. Salva (VP of Product at GitHub)"
type: source
created: 2026-04-12
updated: 2026-04-12
tags: [github-copilot, openai, ai-product-development, developer-tools, r-and-d-incubation, ai-ethics, large-language-models, prompt-engineering]
guest: "Ryan J. Salva"
publish_date: 2022-09-04
duration: "1:05:00"
sources: [lenny-podcast/ryan-j-salva.md]
---

# Source: The role of AI in new product development | Ryan J. Salva (VP of Product at GitHub)

**Guest**: Ryan J. Salva
**Published**: 2022-09-04
**Duration**: 1:05:00
**YouTube**: https://www.youtube.com/watch?v=awcd3P1DnX4

## Executive summary

Ryan J. Salva, VP of Product at GitHub, tells the remarkable origin story of GitHub Copilot — from OpenAI accidentally hammering GitHub's servers while cloning repositories, to the Arctic Code Vault data snapshot that seeded the training data, to the iterative UX experiments that converged on inline gray-text autocomplete within ~18 months. The episode is a case study in incubating breakthrough AI products within large companies, detailing the GitHub Next R&D team's horizon-based structure (5-10% moonshots, 25-30% operations, ~60% incremental), the critical transition of researchers from R&D to product squads, and the 200-millisecond latency sweet spot that keeps developers in flow. Ryan also candidly addresses the ethical and legal challenges of building AI trained on public code — from crude blocklists to Azure's responsible AI models for content filtering — and frames Copilot as an 'AI pair programmer' whose persona principles guide what behavior is appropriate.

## Key ideas

1. **Serendipitous origin of Copilot**: GitHub Copilot originated when OpenAI's mass-cloning of GitHub repositories for training data nearly caused an outage. GitHub redirected this by providing the Arctic Code Vault snapshot — a preservation archive of public code — as clean training data, which became the foundation for Codex and then Copilot.
2. **R&D to product transition framework**: GitHub Next (the R&D team) incubated Copilot through horizon 2-3 research, then intentionally transferred researchers into EPD squads for knowledge transfer. Critically, researchers only returned to R&D when replacements were seated and the product team owned the roadmap — never on a calendar basis.
3. **200ms latency as the flow threshold**: Through extensive experimentation, the team discovered that ~200 milliseconds is the maximum acceptable response time for AI code suggestions before developers feel interrupted. This finding drove architecture decisions and GPU procurement strategy.
4. **AI pair programmer as ethical persona**: Framing Copilot as a 'pair programmer whispering in your ear' created actionable design principles for content filtering — if your pair programmer started spouting politics or slander, you couldn't focus on your work. This persona-based approach evolved from crude blocklists to Azure's responsible AI sentiment models.
5. **Portfolio allocation for bold bets**: Ryan recommends 5-10% of team capacity on experimental moonshots, 25-30% on operations (keeping in-market products healthy), and ~60% on incremental improvements to existing products. This structure only works at scale — startups are necessarily all-in on a single bet.

## Entities

- **Ryan J. Salva** — Guest; VP of Product at GitHub who led the incubation and launch of GitHub Copilot, with a background in philosophy and 10+ years at Microsoft.
- [[github]] — Subject company; platform where Copilot was incubated through the GitHub Next R&D team and transitioned to EPD squads for productization.
- [[github-copilot]] — AI pair programming tool trained on public code via OpenAI's Codex, providing multi-line inline autocomplete that writes 28-40%+ of code depending on language.
- [[openai]] — Partner that trained the Codex model (GPT-3 derivative) on GitHub's public code, accidentally discovering the use case when mass-cloning repositories.
- [[github|GitHub Next]] — GitHub's R&D team focused on horizon 2-3 moonshot projects, which incubated Copilot before transitioning it to operational product squads.
- [[microsoft]] — Parent company providing compute for model training, Azure's responsible AI models for content filtering, and the broader partnership with OpenAI.
- **Arctic Code Vault** — GitHub's preservation archive of public code stored on silver film in Finland, whose data snapshot was repurposed as the clean training data for Codex/Copilot.

## Concepts & frameworks

- **Horizon-Based R&D** — A framework for allocating innovation across three horizons: H1 (next year, incremental), H2 (3 years, medium ambiguity), H3 (5 years, moonshots) — with GitHub Next ring-fenced for H2/H3 work separate from operational EPD teams.
- [[ai-coding-tools|AI Pair Programmer]] — The persona framework used to guide Copilot's ethical design — if a real pair programmer behaved a certain way (spouting politics, profanity), it would be distracting, so the AI shouldn't either.
- [[prompt-engineering-techniques|Prompt Crafting]] — The art and science of engineering what context is fed to the AI model to return useful responses — a critical capability the Copilot team developed alongside model optimization.
- **R&D to EPD Knowledge Transfer** — The process of transitioning researchers from an R&D incubation team to operational product squads, with replacement-based (not calendar-based) criteria for when researchers return to R&D.
- **Portfolio Allocation for Bets** — Ryan's recommended distribution: 5-10% on experimental moonshots, 25-30% on operations, ~60% on incremental improvements — applicable at scale but not for startups.

## Memorable quote

> Ryan J. Salva (00:00:44): 'We had put this snapshot of public repositories on this silver film that would be preserved for thousands of years in this Arctic Code Vault. Well, we took that same data snapshot and we brought it to our friends over at OpenAI to see like, okay, what can we do with these large language models built on public code? Well, it turns out we can do some pretty cool things.'

## B2 angle

This is the earliest episode in the batch (Sep 2022, pre-ChatGPT) and provides the most detailed inside account of shipping an LLM-powered product at scale — from serendipitous data origins to 200ms latency tuning to ethical content filtering — making it the foundational 'how we actually built it' case study for the AI products theme.

## See also

- [[index-by-theme]] — batch plan (this source is in **B2: AI products & LLMs 2024 and earlier**)
- [[synthesis-b2-ai-product-patterns]] — cross-source patterns from B2
- [[comparison-b2-ai-product-approaches]] — how B2 guests differ on AI product strategy
