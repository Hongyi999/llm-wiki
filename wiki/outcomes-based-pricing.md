---
title: Outcomes-Based Pricing
type: concept
created: 2026-04-11
updated: 2026-04-11
tags: [pricing, ai-products, gtm, monetization]
sources: [lenny-podcast/bret-taylor.md, lenny-podcast/madhavan-ramanujam.md]
---

# Outcomes-Based Pricing

Charging customers for the *result* delivered — a resolved ticket, a closed deal, a recovered invoice — rather than for seats, API calls, or features. In B1 this is the **dominant pricing thesis for AI agents** and the deliberate counter-model to per-seat SaaS.

## Canonical case: Sierra AI

[[source-bret-taylor|Bret Taylor]] built [[sierra-ai|Sierra]] entirely around this model. Customers pay per successfully resolved customer-service interaction, not per user account. The alignment is direct: Sierra only makes money when its agent actually completes the job. Bret argues this is the only way to capture the real value of AI — per-seat pricing artificially caps the revenue at software-budget levels when the work being replaced is labor-budget scale.

## The framework: Madhavan Ramanujam's 2×2

[[source-madhavan-ramanujam|Madhavan Ramanujam]] (author of *Monetizing Innovation*) gives the B1 canonical pricing framework for AI companies. His **outcome-pricing 2×2** sorts AI products by:

|                     | **Outcomes measurable?**              | **Outcomes not measurable?**    |
|---------------------|---------------------------------------|----------------------------------|
| **Labor replaced?** | Pure outcomes pricing (Sierra model)  | Hybrid / usage-based             |
| **Augmentation?**   | Outcomes + seat floor                 | Seat-based (legacy SaaS)         |

The key insight from 250+ pricing engagements: **most AI startups undermonetize on day one** because they instinctively default to seat-based thinking when they should be charging labor-budget prices for labor-budget work.

## Labor budget vs software budget arbitrage

Both Bret and Madhavan hammer this:

- **Software budget** per seat per month: $50–500
- **Labor budget** per role per month: $5,000–20,000

An AI product that replaces 10% of a role's work is worth 10% of the labor budget — roughly 10x what the same product could charge as traditional software. Per-seat pricing structurally forfeits this.

## Why B1 AI startups are converging here

1. **Agents complete jobs**, not just "assist" with them. Completing jobs is a billable outcome. See [[ai-agents]].
2. **Evals make outcomes measurable.** If you can [[ai-evals|eval]] whether an agent resolved a ticket, you can bill for it.
3. **Enterprise buyers prefer it.** Committing to labor-budget-scale spend is easier for a CFO when the vendor only earns on delivered work.
4. **Per-seat pricing collapses under agents.** If one agent does the work of 10 seats, per-seat pricing drops revenue 10x instead of rising.

## Open questions

- What happens when the customer disputes whether the outcome was actually delivered? (Bret acknowledges this requires clear definitions and audit trails.)
- How do you bootstrap a pricing conversation when the customer has no baseline for what an outcome is worth?
- Does outcomes-based pricing work for AI products that **augment** humans rather than replace them? (Madhavan's 2×2 says: only partially.)

## See also

- [[sierra-ai]] — the canonical example.
- [[ai-agents]] — why agents make outcomes-based pricing possible.
- [[ai-evals]] — how you measure the outcomes you bill for.
- [[source-madhavan-ramanujam]] — the pricing framework.
- [[source-bret-taylor]] — the agent-era pricing thesis.
