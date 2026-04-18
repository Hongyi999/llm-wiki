---
title: Value-Metric Pricing
type: concept
created: 2026-04-14
updated: 2026-04-14
tags: [concept, pricing, patrick-campbell, profitwell, saas, expansion-revenue, churn]
sources: [lenny-podcast/patrick-campbell.md]
---

# Value-Metric Pricing

**Value-metric pricing** is the practice of choosing a pricing dimension that scales with the *value the customer captures from the product* — per-seat, per-API-call, per-1K-events, per-GB, per-unit-processed — rather than by feature-tier.

[[source-patrick-campbell|Patrick Campbell]] (ProfitWell) calls choosing the right value metric the **single highest-leverage pricing move** available to most SaaS companies.

## The core claim

- **Churn drops 20-25%** on value-metric pricing vs. feature-tiering.
- **Expansion revenue roughly doubles** — because customers grow into higher prices naturally, without renegotiation or upsell friction.
- **Pricing becomes self-aligning**: Disney pays Disney prices; Johnny's startup pays Johnny's prices — the same product, with the same list price, at different effective rates.

## Why it works

- **Aligned incentives** — The customer only pays more when they are capturing more value.
- **Self-serve expansion** — No quarterly negotiation.
- **Market-segmentation without discounting** — Different-sized customers naturally end up at different price points.

## Canonical examples

- **AWS / Stripe / Twilio** — Pay per unit consumed.
- **Slack** — Per active user (a value metric proxy for team size).
- **Datadog** — Per host / per container / per event.

## Anti-examples

- **Fixed-tier SaaS** (Basic / Pro / Enterprise) — Customer-size distribution breaks because a small customer and a whale both fit "Pro."

## Operational discipline

Campbell's rule of thumb:
- **One pricing change per quarter maximum**.
- **One price raise per year** if NPS > 20.

## Related

- [[source-madhavan-ramanujam|Madhavan Ramanujam]] — B1 pricing 2×2; outcomes-based pricing for AI.
- [[outcomes-based-pricing]] — AI-era extension of value-metric thinking.
- [[source-brian-balfour|Brian Balfour]] — Pricing in the context of retention curves.

## Sources

- [[source-patrick-campbell]]
