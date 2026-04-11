---
title: "Source: Why securing AI is harder than anyone expected and guardrails are failing"
type: source
created: 2026-04-11
updated: 2026-04-11
tags: [adversarial-robustness, agentic-ai, ai-products, ai-security, guardrails, jailbreaking, prompt-injection]
guest: "Sander Schulhoff"
publish_date: 2025-12-21
duration: "1:32:41"
sources: [lenny-podcast/sander-schulhoff-20.md]
---

# Source: Why securing AI is harder than anyone expected and guardrails are failing

**Guest**: Sander Schulhoff
**Published**: 2025-12-21
**Duration**: 1:32:41  
**YouTube**: https://www.youtube.com/watch?v=J9982NLmTXg  

## Executive summary

Sander Schulhoff, an AI security researcher who runs HackAPrompt and the largest AI red-teaming competition, delivers a stark warning: all guardrails are failing and there is no technical solution to prompt injection and jailbreaking today. Guardrails marketed as the defense against adversarial attacks are 'terribly, terribly insecure'—a determined attacker will bypass them. The only reason we haven't seen massive attacks yet is because AI systems lack sufficient autonomy and aren't widely deployed enough to cause real harm. But with agents, robotics, and agentic AI systems expanding rapidly, this will change. The conversation isn't meant to halt progress but to force the industry to think harder about mitigating risks before giving AI agents control over critical systems.

## Key ideas

1. Guardrails do not work—period. Any guardrail claiming to 'catch everything' is lying. A determined attacker will defeat guardrails; they're just speed bumps that create false confidence in security.
2. Jailbreaking vs prompt injection: jailbreaking is a user attacking a model directly (no system prompt); prompt injection is an attacker exploiting a developer's system prompt within an application. Both are unsolved.
3. You can patch a bug, but you can't patch a brain. Software bugs are deterministic and fixable; adversarial attacks on neural networks are fundamentally different—a 'fix' still leaves the underlying vulnerability.
4. The real risk comes when agents can take real actions: modify databases, send emails, control robotics. Chatbots are mostly safe because they can only output text. Agentic systems will cause financial loss and eventually physical harm.
5. Technical solutions (human-in-the-loop, sandboxing, CaMeL) are incomplete and will limit AI usefulness. The market will eventually demand fully autonomous AI, which cannot be defended against adversarial input.

## Entities

- **Sander Schulhoff** — guest, AI security researcher, runs HackAPrompt and red-teaming competitions, co-author of Learn Prompting
- **HackAPrompt** — first and largest generative AI red-teaming competition, produced first dataset of prompt injections
- [[openai|OpenAI]] — frontier lab sponsoring and using Schulhoff's red-teaming research
- **Hugging Face** — sponsor of red-teaming competitions, uses prompt injection dataset
- **EMNLP 2023** — conference where Schulhoff's prompt injection paper won best theme paper award

## Concepts & frameworks

- **Prompt Injection** — Attacker manipulates system prompt or input to make LLM ignore its original instructions and perform malicious actions.
- **Jailbreaking** — User tricks a model directly (without system prompt) into breaking its safety guidelines through clever prompting.
- **Guardrails Fallacy** — LLM-based guardrails claiming to catch adversarial attacks are ineffective and create false confidence in security posture.
- **Adversarial Robustness** — Unlike software bugs, neural network vulnerabilities are fundamentally unsolvable—you can't patch an adversarial input without introducing new weaknesses.
- [[ai-agents|Agentic Risk Scaling]] — Risk increases exponentially as AI gains autonomy to take real-world actions (database modification, email, robotics) rather than just generating text.

## Memorable quote

> You can patch a bug, but you can't patch a brain. If you find some bug in your software and you go and patch it, you can be maybe 99.99% sure that bug is solved. Try to do that in your AI system. You can be 99.99% sure that the problem is still there. — Sander Schulhoff

## B1 angle

The most direct warning on AI security: guardrails fail, and agents will be vulnerable. Only researcher with real-world red-teaming data to back this claim.

## See also

- [[index-by-theme]] — batch plan (this source is in **B1: AI products 2025+**)
- [[synthesis-b1-ai-product-patterns]] — cross-source patterns from B1
- [[comparison-b1-ai-product-approaches]] — how B1 guests differ on AI product strategy
