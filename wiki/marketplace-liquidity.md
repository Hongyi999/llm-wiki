---
title: Marketplace Liquidity
type: concept
created: 2026-04-10
updated: 2026-04-10
tags: [marketplaces, liquidity, product-market-fit]
sources: [benjamin-lauzier.md]
---

# Marketplace Liquidity

The operational definition of [[product-market-fit|PMF]] for a two-sided marketplace. Defined by [[benjamin-lauzier|Benjamin Lauzier]] as the **Venn-diagram overlap** between what supply offers and what demand wants, transacted quickly enough that both sides feel the market is alive.

## Two PMFs, not one

A marketplace has **two products**:
- **Supply-side product** — what providers experience.
- **Demand-side product** — what buyers experience.

Each side has its own PMF. You cannot reach "marketplace PMF" by reaching PMF on only one side — the other side's experience will break first.

## Pick the hard side

- The **hard side** is whichever side is harder to acquire or retain.
- Usually (not always) it's **supply**: drivers at [[lyft|Lyft]], quality pros at [[thumbtack|Thumbtack]], hosts at Airbnb.
- Your early strategy should be obsessed with the hard side. The easy side will follow.

### Single-player mode

Give the hard side value **even without the other side present**. Examples:
- Lyft's driver tooling usable before riders showed up.
- Thumbtack's pro-side CRM-like features.
- Hosts' Airbnb calendar tools that were valuable even without bookings.

If the hard side gets no value from being on the platform alone, you can't bootstrap liquidity.

## Measuring liquidity

Two operational proxies dominate the podcast:

### Market Health Metric (Lyft)
- At Lyft, ETA was the health metric.
- Below **~2 minutes** in a dense market, the experience felt magical; above it, riders churned.
- The specific number is less important than the principle: pick one metric that is a **customer-facing proxy** for "the market is alive," and ruthlessly optimize it.

### Fill rate (Thumbtack)
- % of requests that result in a match.
- The north-star metric for home-services marketplaces.
- Low fill rate → the buyer side experiences the marketplace as broken → demand churns → supply churns → death spiral.

## Signs of a good marketplace idea

From Benjamin's checklist:
1. **Fragmentation on both sides** — neither buyers nor sellers have market power.
2. **Uniform needs** — buyers want roughly the same thing, so matching is computable.
3. **High matchmaking barrier** without the platform.

If the two sides can easily find each other without you, you'll be disintermediated.

## Jumpstart tactics

- **Craigslist jumpstart**: both Airbnb and [[thumbtack|Thumbtack]] seeded supply from Craigslist.
- **Concierge supply**: manually recruit the first providers.
- **Geographic focus**: one neighborhood, one zip code, one city. Liquidity is local.
- **Supply subsidies**: Lyft's GM rental-car partnership put cars in the hands of drivers who couldn't afford one.
- **Peer recruiting**: Lyft's mentor/ambassador program paid existing drivers to onboard new ones ($35/session + $20/recruit).

## Failure modes

- **Over-control** (Sidecar): taking too much agency away from supply kills supply motivation.
- **Cognitive load** ([[thumbtack|Thumbtack]] smoke-machine example): demanding too much information from supply before matching them with demand kills response rates.
- **Thin local density** dressed up as "national launch": better to own one zip code than have 1 match per city.

## PMF before marketplace mechanics

Benjamin is explicit that marketplace dynamics only matter **after** single-sided PMF exists. His Reforge course explicitly asks students to wait until they have PMF before enrolling.

## See also

- [[benjamin-lauzier]], [[lyft]], [[thumbtack]]
- [[product-market-fit]]
- [[source-benjamin-lauzier-marketplaces]]
