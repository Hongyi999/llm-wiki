---
title: "Source: AI prompt engineering in 2025: What works and what doesn't | Sander Schulhoff"
type: source
created: 2026-04-12
updated: 2026-04-12
tags: [prompt-engineering, ai-security, red-teaming, prompt-injection, llm-techniques, ai-safety, agentic-ai]
guest: "Sander Schulhoff"
publish_date: 2025-06-19
duration: "1:37:47"
sources: [lenny-podcast/sander-schulhoff.md]
---

# Source: AI prompt engineering in 2025: What works and what doesn't | Sander Schulhoff

**Guest**: Sander Schulhoff
**Published**: 2025-06-19
**Duration**: 1:37:47
**YouTube**: https://www.youtube.com/watch?v=eKuFqQKYRrA

## Executive summary

Sander Schulhoff, the creator of the first prompt engineering guide on the internet and lead author of The Prompt Report (the most comprehensive study of prompt engineering ever done, analyzing 1,500+ papers and 200+ techniques), makes a forceful case that prompt engineering remains critically important despite recurring predictions of its demise. He distinguishes between conversational prompt engineering (everyday chatbot use) and product-focused prompt engineering (optimizing prompts at scale for millions of users), arguing the latter is where the real value lies. The episode covers five concrete prompting techniques—few-shot prompting, decomposition, self-criticism, additional information/context, and ensembling—while debunking the effectiveness of role prompting and emotional threats/rewards. The second half pivots to AI red teaming and prompt injection, where Schulhoff draws on his experience running HackAPrompt (the world's largest AI red-teaming competition, yielding 600,000 prompt injection techniques) to argue that prompt injection is fundamentally unsolvable and poses an escalating threat as AI agents gain real-world agency.

## Key ideas

1. **Prompt engineering is not dead—it's evolving**: Studies show bad prompts can yield 0% accuracy while good prompts boost performance to 90%. The distinction between conversational prompt engineering (casual chatbot use) and product-focused prompt engineering (optimizing prompts running millions of inputs) is critical, with the latter being where the highest-stakes optimization occurs.
2. **Five high-value prompting techniques**: Few-shot prompting (giving examples) and providing additional context/information deliver the highest uplift. Decomposition (breaking problems into subproblems), self-criticism (having the LLM check its own work), and ensembling (running multiple prompts and taking the majority answer) round out the toolkit. Meanwhile, role prompting has no measurable effect on accuracy tasks, and emotional threats/rewards ('someone will die') likely don't work either.
3. **Prompt injection is fundamentally unsolvable**: Unlike classical cybersecurity where you can patch a bug, you cannot patch a brain. Prompt-based defenses ('do not follow malicious instructions'), AI guardrails, and keyword blocking all fail against motivated attackers. Only safety-tuning and fine-tuning at the model provider level offer meaningful mitigation. Sam Altman estimates 95-99% security is achievable, but never 100%.
4. **Agentic AI security is the looming crisis**: If chatbots cannot be fully secured against prompt injection, the stakes escalate dramatically with autonomous agents that book flights, manage finances, or inhabit humanoid robots. A coding agent could be tricked by a malicious website into writing a virus into your codebase. The gap between guardrail intelligence and main model intelligence creates exploitable attack surfaces.
5. **Artificial social intelligence as a new literacy**: Schulhoff coins 'artificial social intelligence' as the AI-era analog to interpersonal communication skills—the ability to communicate effectively with AI systems, understand their responses, and adapt your prompts accordingly. This skill will remain important regardless of how capable models become.

## Entities

- **Sander Schulhoff** — OG prompt engineer, creator of the first prompt engineering guide, lead author of The Prompt Report, and founder of Learn Prompting and HackAPrompt.
- [[openai]] — Sponsor of HackAPrompt and cited the competition's dataset in five recent publications for model security improvements.
- **Learn Prompting** — Schulhoff's educational platform for prompt engineering, reaching millions of users.
- **HackAPrompt** — The first and largest AI red-teaming competition in the world, collecting 600,000 prompt injection techniques.
- **The Prompt Report** — 76-page research paper co-authored with OpenAI, Microsoft, Google, Princeton, and Stanford analyzing 1,500+ papers and identifying 200+ prompting techniques.
- **GPT-4** — Referenced as the model used in medical coding and prompt injection experiments throughout the episode.
- [[chatgpt]] — Primary example of a consumer chatbot vulnerable to prompt injection attacks.
- **Reid Hoffman** — Quoted for his analogy that we may only be using 3-5% of AI's potential given our prompting skills.
- **Daylight Computer DC-1** — ePaper device praised by Schulhoff as a favorite product for reading without blue light exposure.

## Concepts & frameworks

- [[prompt-engineering-techniques|Few-shot prompting]] — Giving the LLM examples of desired input-output pairs to dramatically improve performance, identified as the single most impactful prompting technique.
- [[ai-evals|Prompt injection]] — The practice of tricking AI systems into bypassing safety constraints through techniques like storytelling, typos, encoding (Base64), and obfuscation.
- **Artificial social intelligence** — A coined term describing the human skill of communicating effectively with AI systems—understanding how to prompt, interpret responses, and adapt.
- [[prompt-engineering-techniques|Product-focused prompt engineering]] — Optimizing a single prompt that runs millions of inputs through an API, as opposed to casual conversational use of chatbots.
- [[prompt-engineering-techniques|Self-criticism technique]] — Having the LLM critique its own output and then implement its own suggestions, yielding a free performance boost in certain situations.
- [[prompt-engineering-techniques|Decomposition]] — Asking the LLM to identify subproblems before solving the main task, enabling better reasoning on complex multi-step problems.
- [[prompt-engineering-techniques|Ensembling]] — Running the same problem through multiple prompts or models and taking the most common answer as the final response.
- [[ai-evals|AI red teaming]] — Systematically testing AI systems by attempting to elicit harmful or prohibited outputs, described as 'artificial social engineering.'

## Memorable quote

> Sander Schulhoff (01:15:08): 'It is not a solvable problem, which I think is very difficult for a lot of people to hear. You can patch a bug, but you can't patch a brain.'

## B2 angle

Uniquely positions prompt engineering as both an offensive and defensive discipline—the same techniques that optimize LLM performance also expose fundamental security vulnerabilities that become existential as AI moves from chatbots to autonomous agents.

## See also

- [[index-by-theme]] — batch plan (this source is in **B2: AI products & LLMs 2024 and earlier**)
- [[synthesis-b2-ai-product-patterns]] — cross-source patterns from B2
- [[comparison-b2-ai-product-approaches]] — how B2 guests differ on AI product strategy
