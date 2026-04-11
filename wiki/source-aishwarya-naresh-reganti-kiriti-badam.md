---
title: "Source: Why most AI products fail: Lessons from 50+ AI deployments at OpenAI, Google & Amazon"
type: source
created: 2026-04-11
updated: 2026-04-11
tags: [ai-agents, ai-products, customer-trust, deployment-failure, evals, operational-ai]
guest: "Aishwarya Naresh Reganti, Kiriti Badam"
publish_date: 2026-01-11
duration: "1:26:22"
sources: [lenny-podcast/aishwarya-naresh-reganti-kiriti-badam.md]
---

# Source: Why most AI products fail: Lessons from 50+ AI deployments at OpenAI, Google & Amazon

**Guest**: Aishwarya Naresh Reganti, Kiriti Badam
**Published**: 2026-01-11
**Duration**: 1:26:22  
**YouTube**: https://www.youtube.com/watch?v=z7T1pCxgvlA  

## Executive summary

Two AI product leads who built 50+ deployments across OpenAI, Google, Amazon and Databricks break down why most AI products fail. The core insight: AI products differ fundamentally from traditional software in non-determinism (you cannot predict user or LLM behavior) and agency control trade-offs (handing decision-making to agents means losing control). Their framework—Continuous Calibration/Continuous Development (CC/CD)—emphasizes building small, iterating fast, measuring customer trust obsessively, and understanding that evals are necessary but insufficient for production quality.

## Key ideas

1. Non-determinism and agency control trade-off are the two defining characteristics that change how you build AI products: you cannot predict user behavior or LLM outputs, and when you give agents decision-making power, you relinquish control proportionally.
2. Start small and resist complexity creep: the biggest mistake is racing to build agents before solving the foundational problem. Most AI products fail because they start with a solution (an agentic system) rather than a problem.
3. Evals alone don't guarantee production quality—guardrails fail, and what matters is continuous calibration against real customer feedback and deployed-system performance, not synthetic benchmarks.
4. Customer trust is the underrated driver of AI product success: reliability, transparency, and 'explainability under pressure' matter more than raw capability. Companies like Booking.com built 50+ AI systems that actually moved revenue because they obsessed over user control and trust.
5. The CC/CD framework (not SDLC) is the operational model: continuous calibration of models against real-world data, continuous development in tight loops, constant measurement of reliability gaps.

## Entities

- **Aishwarya Naresh Reganti** — guest, applied AI lead at OpenAI and Google, co-author of Awesome Generative AI Guide
- **Kiriti Badam** — guest, AI engineer, worked at OpenAI Codex team
- [[openai|OpenAI]] — employer where guests built AI products at scale
- [[google|Google]] — employer where guests worked on AI deployments
- **Amazon** — employer, involved in 50+ AI product deployments
- **Booking.com** — cited example of AI product success through trust-first approach

## Concepts & frameworks

- **Non-determinism in AI** — AI systems produce different outputs for the same input; you cannot predict user behavior or model responses, fundamentally changing product design.
- **Agency Control Trade-off** — Handing decision-making to agents requires accepting loss of control; the more autonomous the system, the less oversight you have.
- **Continuous Calibration/Continuous Development** — Iterative model refinement against real-world data and user feedback; replaces traditional SDLC for AI products.
- **Customer Trust as Metric** — Reliability, transparency, and controlled autonomy matter more than benchmark scores for production AI success.
- [[ai-evals|Evals Limitations]] — Synthetic evaluations are necessary but insufficient; guardrails provide false confidence and real production monitoring is critical.

## Memorable quote

> It's not about being the first company to have an agent among your competitors. It's about have you built the right flywheels in place so that you can improve over time. — Aishwarya Naresh Reganti

## B1 angle

One of the most practical, hard-won guides to why most AI products fail and the CC/CD framework that actually works—directly from engineers who shipped 50+ systems.

## See also

- [[index-by-theme]] — batch plan (this source is in **B1: AI products 2025+**)
- [[synthesis-b1-ai-product-patterns]] — cross-source patterns from B1
- [[comparison-b1-ai-product-approaches]] — how B1 guests differ on AI product strategy
