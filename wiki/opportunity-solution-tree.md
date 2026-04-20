---
title: Opportunity Solution Tree (OST)
type: concept
created: 2026-04-13
updated: 2026-04-13
tags: [teresa-torres, continuous-discovery, opportunity-solution-tree, discovery-habits, product-trio]
sources: [lenny-podcast/teresa-torres.md]
---

# Opportunity Solution Tree (OST)

The **Opportunity Solution Tree** is the canonical artifact of modern product discovery, popularized by [[source-teresa-torres|Teresa Torres]] in *Continuous Discovery Habits*. It structures the relationship between a desired outcome and the set of experiments that might drive it.

## The tree structure

```
                  Desired Outcome
                         │
      ┌──────────────────┼──────────────────┐
      │                  │                  │
 Opportunity 1      Opportunity 2      Opportunity 3
      │                  │                  │
  ┌───┴───┐          ┌───┴───┐          ┌───┴───┐
Solution Solution  Solution Solution  Solution Solution
  │        │         │        │         │        │
 Tests    Tests     Tests    Tests     Tests    Tests
```

- **Outcome (top)**: A measurable business outcome (activation rate, weekly active users, conversion to paid). One per tree.
- **Opportunities (middle)**: Customer needs, pain points, or desires — phrased in customer language. Multiple per outcome.
- **Solutions (middle-bottom)**: Specific interventions that might address an opportunity. Multiple per opportunity.
- **Assumption Tests (bottom)**: The cheapest experiment to learn whether the solution works. Multiple per solution.

## Why the tree structure matters

Most PMs jump from outcome directly to a single solution. The tree forces:

1. **Multiple opportunities per outcome** — Which customer need is actually blocking this outcome?
2. **Multiple solutions per opportunity** — Is the first idea really the best? Brainstorming three or more solutions surfaces trade-offs.
3. **Explicit assumption testing** — Every solution embeds assumptions (desirability, viability, usability, feasibility, ethics). Name the riskiest one; test the cheapest.

## Continuous, not one-shot

The tree is a living artifact, updated weekly. New interviews add opportunities. Failed tests prune solutions. The tree represents the team's current map of the problem space, not a final plan.

## The Product Trio as owner

The tree is owned by the **Product Trio**: PM, designer, engineer. Each brings a different lens:

- **PM** — viability (business)
- **Designer** — desirability and usability (customer)
- **Engineer** — feasibility (technical)

Solo-PM trees tend to be thin; trio-built trees surface assumptions that a single role would miss.

## Relation to other artifacts

- **Now/Next/Later roadmap** ([[source-janna-bastow]]): The roadmap is what the OST's winning solutions become once validated.
- **Product Strategy Stack** ([[source-ravi-mehta]]): The outcome at the top of the OST is derived from the strategy layer above it.
- **Working Backwards PR/FAQ** ([[working-backwards]]): Complementary artifact — OST maps the discovery space; PR/FAQ locks the solution once a direction is chosen.

## Common failure modes

- **Solution-first trees** — Starting with solutions and retrofitting opportunities. A smell test: can every opportunity stand alone as a customer pain point?
- **Too many outcomes** — One tree, one outcome. Multi-outcome trees become unusable.
- **Dead tree** — If the tree isn't updated weekly, it's stale decoration. Cadence matters.

## Related sources

- [[source-teresa-torres]] — Primary source; canonical articulation.
- [[source-marty-cagan]] — Discovery precursor; intellectual lineage.
- [[source-petra-wille]] — PMwheel competency coaching that complements OST practice.

## Related concepts

- [[continuous-discovery]] — The habit OST structures.
- [[jobs-to-be-done]] — Adjacent school for framing opportunities.
