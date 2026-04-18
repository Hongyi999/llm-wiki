---
title: Growth Model
type: concept
created: 2026-04-15
updated: 2026-04-15
tags: [concept, growth, dan-hockenmaier, spreadsheet, saas, marketplace, analytical]
sources: [lenny-podcast/dan-hockenmaier.md]
---

# Growth Model

A **spreadsheet-based analytical representation of a business** used to quantify how all growth levers compound into top-line numbers. Canonical treatment from [[source-dan-hockenmaier|Dan Hockenmaier]] (ex-Thumbtack, Faire).

## The thesis

"50% of the value you get from it is simply building the model. It forces you to understand it."

The output number is almost secondary. The act of building the model — specifying inputs, surfacing invisible dependencies, quantifying assumptions — is where the insight lives.

## Three building blocks (SaaS)

1. **Acquisition** — New users per period; decomposed by channel.
2. **Retention** — Cohort curves; churn/resurrection.
3. **Monetization** — Revenue per user, expansion, AOV.

## Additional layers

- **Transactional businesses**: AOV, frequency, take rate.
- **Marketplaces**: supply-side model, liquidity, cross-side matching.
- **Consumer subscription**: [[source-casey-winters_|Casey Winters's]] retention math — need >60-70% annual retention to sustain.

## Sensitivity analysis reveals priorities

Run scenarios: +10% to acquisition, +10% to retention, +10% to monetization. [[source-dan-hockenmaier|Hockenmaier's]] observation: models repeatedly show growth is "exceptionally sensitive" to retention because it compounds into virality, content, payback period.

## Two-metric north star framework

[[source-sri-batchu|Sri Batchu / Ramp]]: pair a **volume metric** (SQL pipeline $) with an **efficiency metric**. Every team's local metric has a translation factor to the company north star, updated every 6 months. Enables cross-team prioritization in a common currency.

## Marketplace-specific: dual-sided ROI

[[source-dan-hockenmaier|Hockenmaier]]: supplier acquisition cost + customer acquisition cost vs. LTV (supplier GMV × take rate × retention). Replaces naive "marketplace balance" ratios.

## Related

- **[[growth-loops]]** — The loop view; complementary to the model view.
- **[[marketplace-liquidity]]** — Core marketplace growth-model input.
- **[[product-led-growth]]** — The DLG foundation.
- **[[source-naomi-gleit|Growth accounting]]** — New − stale + resurrected (Facebook origin).

## Canonical quote

> "If you think about running a marketplace, you're basically a gardener. You have to have a very light touch. If you're building a SaaS business, you're a construction worker."

## Sources

- [[source-dan-hockenmaier]]
- [[source-sri-batchu]]
