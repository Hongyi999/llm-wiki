---
title: Prompt Engineering Techniques
type: concept
created: 2026-04-12
updated: 2026-04-12
tags: [prompt-engineering, llm-techniques, ai-evals, ai-security, product-development]
sources: [lenny-podcast/sander-schulhoff.md, lenny-podcast/kevin-weil.md, lenny-podcast/logan-kilpatrick.md, lenny-podcast/aparna-chennapragada.md]
---

# Prompt Engineering Techniques

Prompt engineering is the discipline of crafting inputs to large language models to reliably produce desired outputs. Despite recurring predictions of its demise ("just talk to the AI naturally"), research shows that bad prompts can yield 0% accuracy while good prompts boost performance to 90% on the same task. The field divides into two distinct practices: *conversational* prompt engineering (everyday chatbot use by individuals) and *product-focused* prompt engineering (optimizing a single prompt that runs millions of inputs through an API). The latter is where the highest-stakes optimization occurs and where the techniques below have the most impact.

## Canonical methodology: the five techniques that work

[[source-sander-schulhoff|Sander Schulhoff]] -- creator of the first prompt engineering guide on the internet and lead author of The Prompt Report (analyzing 1,500+ papers and 200+ techniques) -- identifies five high-value prompting techniques with strong empirical support:

### 1. Few-shot prompting

Giving the LLM examples of desired input-output pairs before the actual task. Identified as the single most impactful technique across the literature. Even 2--3 examples can dramatically shift model behavior, especially for formatting, tone, and classification tasks.

### 2. Additional context / information

Providing the model with relevant background information it would not otherwise have. This aligns with [[source-logan-kilpatrick|Logan Kilpatrick]]'s maxim: "Context is all you need." Models are eager to answer but lack context; better inputs yield dramatically better outputs. At OpenAI, Kilpatrick argued that if they printed t-shirts, they should say "Context is the only thing that matters."

### 3. Decomposition

Asking the LLM to break a complex problem into subproblems before attempting to solve the whole. This is the prompting analog of divide-and-conquer algorithms -- it enables better reasoning on multi-step problems by reducing the cognitive load on any single generation step.

### 4. Self-criticism

Having the LLM critique its own output and then implement its own suggestions. This yields a "free performance boost" in many situations because the model can catch errors in review that it made during generation -- similar to how human proofreading catches mistakes the writer missed.

### 5. Ensembling

Running the same problem through multiple prompts (or the same prompt multiple times) and taking the most common answer as the final response. Trades compute cost for reliability. Particularly valuable in production systems where a single wrong answer has high cost.

## What does NOT work (debunked techniques)

Schulhoff's research also identifies two popular techniques that have **no measurable effect** on accuracy:

### Role prompting

Prefacing a prompt with "You are a world-class expert in X" or "Act as a senior software engineer." Despite being widely recommended, controlled studies show no measurable accuracy improvement from role prompting. It may affect tone and style, but it does not make the model smarter at the task.

### Emotional threats / rewards

Prompts like "This is very important to my career" or "Someone will die if you get this wrong." These likely do not improve performance. While some papers have shown marginal effects, Schulhoff considers the evidence unconvincing and the mechanism implausible.

## Contrasting views

| Guest | Role / Company | Core framing | Key insight | Emphasis |
|---|---|---|---|---|
| [[source-sander-schulhoff\|Sander Schulhoff]] | Lead author, The Prompt Report | Empirical science -- 1,500 papers, 200+ techniques, controlled experiments | 5 techniques work, 2 are debunked; prompt engineering is evolving, not dying | Product-focused prompt engineering (millions of API calls) |
| [[source-kevin-weil\|Kevin Weil]] | CPO, [[openai\|OpenAI]] | Evals as the meta-skill -- prompting is half the battle, measuring is the other | Writing evals is a core PM skill; product design depends on accuracy level (60% vs 99.5%) | [[ai-evals\|Evals]] as inseparable from prompting |
| [[source-logan-kilpatrick\|Logan Kilpatrick]] | DevRel, [[openai\|OpenAI]] | Human communication skill -- the same principles that help people communicate help with LLMs | "Context is all you need" -- models are eager but lack background; provide context, goals, examples | Accessibility -- prompting as a skill everyone already has |
| [[source-aparna-chennapragada\|Aparna Chennapragada]] | CPO, [[microsoft\|Microsoft]] | Product development tool -- "prompt sets are the new PRDs" | The fastest path from idea to validation is a prototype, not a document; demos before memos | Prototyping and organizational transformation |

## Consensus

Despite coming from different vantage points (researcher, platform provider, enterprise CPO), the four sources agree on several points:

1. **Prompt engineering is not dead.** Every source pushes back on the "just talk naturally" narrative. Schulhoff shows the 0%-to-90% accuracy gap. Kilpatrick emphasizes context as a learnable, improvable skill. Weil frames evals as the feedback loop that makes prompting iterative.

2. **Context is the highest-leverage input.** Whether called "few-shot prompting" (Schulhoff), "context is all you need" (Kilpatrick), or "prompt sets" (Chennapragada), all sources agree that giving the model more relevant information is the single most effective intervention.

3. **The discipline is bifurcating.** Casual chatbot prompting is becoming easier as models improve. But product-focused prompt engineering -- optimizing a single prompt running millions of inputs through an API -- is becoming *more* important and more specialized.

4. **Prompting and evaluation are inseparable.** Weil explicitly argues you cannot do one without the other: the prompt determines the output, but only evals tell you whether the output is good enough. This connects prompt engineering directly to [[ai-evals]].

## Open disagreements

### Will prompt engineering eventually disappear?

Schulhoff argues it will remain important indefinitely, coining "artificial social intelligence" as the permanent human skill of communicating with AI systems. Kilpatrick takes a softer position -- context provision will always matter, but the specific techniques may simplify as models improve. Neither Weil nor Chennapragada addresses the long-term directly, but Weil's emphasis on evals suggests the *measurement* side will persist even if the *crafting* side becomes easier.

### Product-focused vs. conversational

Schulhoff draws a sharp line between the two. Kilpatrick blurs it, arguing the same human communication principles apply in both cases. Chennapragada largely ignores the product-focused side, framing prompting as a prototyping and communication tool for PMs and leaders.

### Prompting as science vs. art

Schulhoff approaches it as empirical science (controlled studies, reproducible results). Kilpatrick frames it as an interpersonal art ("the most eager person in the world to answer your question"). Chennapragada treats it as a product development craft. This tension between rigor and intuition remains unresolved.

## Relationship to [[ai-evals]]

[[source-kevin-weil|Kevin Weil]] makes the strongest case for treating prompt engineering and [[ai-evals]] as a single discipline: the product you build at 60% model accuracy is fundamentally different from one at 99.5%, and evals are the mechanism for tracking improvement. This means every prompt change should be paired with an eval measuring its impact -- a workflow that mirrors test-driven development in traditional software engineering.

The B1 batch's [[source-hamel-husain-shreya-shankar|Hamel Husain and Shreya Shankar]] episode provides the canonical evals methodology (error analysis, axial coding, LLM-as-judge), which directly complements Schulhoff's prompting techniques.

## See also

- [[ai-evals]] -- the measurement discipline inseparable from prompting
- [[ai-coding-tools]] -- where prompt engineering meets code generation
- [[taste-as-differentiator]] -- judgment about what to prompt for matters as much as how
- [[ai-agents]] -- prompt injection becomes an existential risk as agents gain real-world agency
- [[openai]] / [[microsoft]] / [[anthropic]] -- the platform providers shaping the discipline
