---
title: Product Velocity in the AI Era
type: concept
created: 2026-04-11
updated: 2026-04-11
tags: [product-velocity, ai-products, iteration, shipping-cadence]
sources: [lenny-podcast/nick-turley.md, lenny-podcast/dan-shipper.md, lenny-podcast/asha-sharma.md, lenny-podcast/brian-balfour.md, lenny-podcast/robby-stein.md, lenny-podcast/grant-lee.md, lenny-podcast/howie-liu.md, lenny-podcast/elena-verna-40.md]
---

# Product Velocity in the AI Era

The observation — shared across 8+ B1 guests — that AI products are built and scaled on fundamentally faster iteration cycles than traditional software, and that this speed is itself a durable advantage.

## Convergent practices

### 1. Ship daily, discover the product empirically

- [[source-nick-turley|Nick Turley]]: [[chatgpt|ChatGPT]] is built by shipping and measuring, not by writing strategy docs. "Product as empirical discovery."
- [[source-robby-stein|Robby Stein]]: Google Search culture of "relentless improvement" — small changes every day compound into quality.
- [[source-howie-liu|Howie Liu]]: "Timely over ritual" meetings — meetings happen when a decision is needed, not on a calendar.

### 2. Vibe over benchmarks

- [[source-nick-turley|Nick Turley]]: the ChatGPT team trusts subjective vibe checks over leaderboard metrics. A model that feels better usually *is* better.
- [[source-dan-shipper|Dan Shipper]]: "vibe checks" are how a 15-person team evaluates 5 shipped products — there isn't time for formal eval suites on every release.

### 3. Seasons over semesters

- [[source-asha-sharma|Asha Sharma]]: plan in **seasons** (6 weeks), not semesters (6 months). Products are organisms, not artifacts.
- [[source-brian-balfour|Brian Balfour]]: **cycle compression** — the time from idea → ship → customer feedback → next iteration keeps shrinking, and companies that can't compress fall behind.

### 4. Fast/slow team splits

- [[source-howie-liu|Howie Liu]]: [[figma|Airtable]] restructured into **fast teams** (ship daily) and **slow teams** (deep refactors and infra), because mixing them ruins both. Copying Figma's structure.
- [[source-asha-sharma|Asha Sharma]]: similar split at Microsoft AI — composable building blocks shipped fast, underlying platform moves slower.

### 5. Continuous PMF recalibration

- [[source-elena-verna-40|Elena Verna]]: [[product-market-fit|PMF]] is a **3-month treadmill**, not a destination. Every 90 days, market conditions shift and you must re-prove you still have PMF. 95% innovation / 5% optimization.
- [[source-grant-lee|Grant Lee]] ([[gamma|Gamma]]): four months rebuilding onboarding was the inflection point for $100M ARR. Willingness to redo core UX at velocity is what separated Gamma.

## Why AI makes this possible

- **Models improve weekly.** What was impossible in April is table-stakes in June; you can't plan on a 6-month horizon when your building material keeps changing.
- **AI coding tools compress dev cycles.** [[source-dan-shipper|Dan Shipper]]'s team ships products with Claude Code as primary interface; what took 6 engineers a month now takes 1 engineer a week.
- **[[ai-evals|Evals]] automate the QA bottleneck.** Fast evals → fast iteration → fast product.
- **Users tolerate rough edges.** AI products are in a "fascination honeymoon" where users forgive rough UX that would kill a traditional SaaS product.

## Why AI makes this *necessary*

- **Platform cycle velocity** ([[source-brian-balfour|Balfour]]): every few years a new platform lets you rebuild a product category; whoever ships first defines defaults. Missing a cycle kills you.
- **AI bet or death** ([[source-eoghan-mccabe|Eoghan McCabe]]): gradual change doesn't work; disruption is violent. Speed is survival.
- **Pioneer-to-majority gap** ([[source-elena-verna-40|Elena Verna]]): the window between early adopters and mainstream is compressing, and you must race through it.

## Anti-patterns from B1

- Quarterly roadmaps (too slow).
- Large eval suites that block ship (use [[ai-evals|LLM-as-judge]] evals that run on PR).
- Formal strategy docs (ship and discover).
- Code quality optimization ([[source-dhanji-r-prasanna|Dhanji]]: unrelated to product success).

## Open questions

- Is this velocity sustainable without burning out teams?
- Does it scale past ~50 engineers, or is there a size where process must reassert itself?
- How do you balance velocity with the safety concerns raised in [[ai-agents]]?

## See also

- [[ai-native-organization]] — the org design that enables this speed.
- [[ai-evals]] — the QA mechanism that unblocks it.
- [[chatgpt]], [[gamma]] — canonical velocity case studies.
