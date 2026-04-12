---
title: Shape Up
type: concept
created: 2026-04-12
updated: 2026-04-12
tags: [product-methodology, project-management, shaping, appetite, basecamp, agile-alternative]
sources: [lenny-podcast/ryan-singer.md]
---

# Shape Up

Shape Up is a product development methodology created by [[source-ryan-singer|Ryan Singer]] at [[basecamp|Basecamp/37signals]]. It is a radical alternative to Scrum and agile sprints, replacing estimates with **appetites** (fixed time budgets), backlogs with **shaping** (collaborative problem definition), and open-ended iteration with **circuit breakers** (hard stops that kill work that doesn't converge). The methodology is documented in Singer's free online book and has been adopted by teams at Shopify, Freshworks, and hundreds of other companies.

## Core mechanics

### Appetites, not estimates

Instead of asking "how long will this take?" (an estimate), Shape Up asks "how much time is this worth?" (an appetite). Appetites are top-down bets: leadership decides a problem is worth 2 weeks or 6 weeks of a small team's time. If the team can't ship within the appetite, the project is killed — not extended.

### Shaping

Before any work is committed, a small group (typically a senior designer and engineer) shapes the work in a collaborative session. The output is a **pitch** — not a spec — that defines:
- The problem and why it matters
- The solution at the right level of abstraction (a "fat marker sketch" — rough enough to leave room for the team, detailed enough to show the approach is viable)
- **Rabbit holes** — known risks flagged upfront
- **No-gos** — explicitly excluded scope

Singer uses **breadboarding** (text-based flow diagrams) and **fat marker sketches** (deliberately low-fidelity visuals) to communicate shape without over-specifying.

### Circuit breakers

Every bet has a hard time limit (the appetite). If the team hasn't converged by the deadline, the project is killed — no extensions, no "just one more sprint." This prevents runaway projects and forces honest scope negotiation upfront during shaping.

### Cool-down

Between cycles, teams get 2 weeks of unstructured cool-down time for bug fixes, exploration, and recovery. This is not slack — it's a deliberate structural element that prevents burnout and enables serendipitous discovery.

## Singer's candid caveats

Singer is unusually honest about Shape Up's limitations. He acknowledges that Basecamp's specific conditions — a bootstrapped company with a small team, a CEO who is the primary shaper, and a culture of extreme autonomy — don't transfer automatically. The methodology works best when leadership is deeply involved in shaping and when teams have genuine autonomy to make trade-offs within the appetite.

## Relationship to adjacent concepts

- **[[jobs-to-be-done]]**: Singer collaborated with Bob Moesta and the Shape Up methodology draws on JTBD's insight that scope should be shaped by the struggling moment, not by feature lists. Singer's shaping sessions often begin with "what's the struggling moment?"
- **[[product-operating-model]]**: Shape Up is one answer to "how should empowered teams work?" It's compatible with Cagan's empowered-team model but incompatible with feature-team/Scrum backlogs.
- **[[product-market-fit]]**: Shape Up's appetite-and-circuit-breaker approach is a mechanism for rapid PMF exploration — you can run many cheap bets rather than one expensive project.

## See also

- [[source-ryan-singer]] — the canonical Shape Up episode
- [[basecamp]] — where Shape Up was created
- [[jobs-to-be-done]] — the customer research framework that influenced shaping
- [[product-operating-model]] — the broader question of how product teams should operate
