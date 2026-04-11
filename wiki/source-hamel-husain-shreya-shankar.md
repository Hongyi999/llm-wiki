---
title: "Source: Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar"
type: source
created: 2026-04-11
updated: 2026-04-11
tags: [ai-engineering, ai-evals, ai-products, error-analysis, evaluation-frameworks, llm-as-judge, product-building]
guest: "Hamel Husain & Shreya Shankar"
publish_date: 2025-09-25
duration: "1:46:33"
sources: [lenny-podcast/hamel-husain-shreya-shankar.md]
---

# Source: Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar

**Guest**: Hamel Husain & Shreya Shankar
**Published**: 2025-09-25
**Duration**: 1:46:33  
**YouTube**: https://www.youtube.com/watch?v=BsWxPI9UM4c  

## Executive summary

Hamel Husain and Shreya Shankar present the definitive framework for AI product builders: start with error analysis by manually reviewing 20-100 production traces to identify failure modes, group them into axial codes (failure categories), then build evals—either code-based checks or LLM-as-judge evaluators. Their Field Guide distills techniques from machine learning theory (open coding, theoretical saturation) into a practical workflow that replaces guesswork with measurable signals, avoiding the common pitfall of automating error detection with LLMs too early.

## Key ideas

1. Error analysis via open coding — manually review production traces and write one-sentence notes on the first upstream error, sampling until theoretical saturation (20-100 traces)
2. Benevolent dictator approach — appoint one domain expert (often the product manager) to make judgment calls in error analysis rather than committee review, reducing cost and keeping the process tractable
3. Axial coding and pivot tables — use Claude or ChatGPT to synthesize open codes into failure categories, then count occurrences to identify the top 3-5 problems worth fixing
4. LLM-as-judge with binary decisions — for subjective failure modes like 'should we hand off to a human?', build narrowly-scoped evaluators that output true/false, not 1-5 scores
5. Validate judges against humans — measure agreement between your LLM judge and manual labels before shipping, ensuring the eval doesn't drift from ground truth

## Entities

- **Hamel Husain** — Co-instructor of Maven's #1 AI evals course, trained 2,000+ PMs and engineers at OpenAI and Anthropic
- **Shreya Shankar** — Berkeley PhD researcher, co-instructor and curriculum designer for AI evals course
- **Nurture Boss** — Property management AI assistant used as real-world case study for error analysis
- [[anthropic|Anthropic]] — AI lab that trained teams in evals; CPO cited evals as critical skill
- [[openai|OpenAI]] — AI lab that trained teams in evals; CPO cited evals as critical skill

## Concepts & frameworks

- [[ai-evals|Error Analysis]] — Manually examining production traces to identify failure modes before building automated tests; grounded in decades of ML theory

## Memorable quote

> Everyone that does this immediately gets addicted to it. When you're building an AI application, you just learn a lot. — Hamel Husain

## B1 angle

Error analysis is the systematic foundation that separates successful AI products from failed pilots; it's the skill that turns guesswork into measured iteration.

## See also

- [[index-by-theme]] — batch plan (this source is in **B1: AI products 2025+**)
- [[synthesis-b1-ai-product-patterns]] — cross-source patterns from B1
- [[comparison-b1-ai-product-approaches]] — how B1 guests differ on AI product strategy
