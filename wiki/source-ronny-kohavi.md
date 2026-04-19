---
title: "Source: The Ultimate Guide to A/B Testing ft. Ronny Kohavi"
type: source
created: 2026-04-10
updated: 2026-04-19
tags: [a-b-testing, experimentation, data-driven, metrics, product-management, growth, trust]
sources: [lenny-podcast/ronny-kohavi.md]
---

# Source: The Ultimate Guide to A/B Testing ft. Ronny Kohavi

**Guest**: Ronny Kohavi (Former VP & Technical Fellow at Airbnb; former Corporate VP at Microsoft leading Microsoft Experimentation Platform; former Director of Data Mining & Personalization at Amazon)
**Published**: 2023-07-27
**Duration**: ~1h 23m
**YouTube**: https://www.youtube.com/watch?v=hEzpiDuYFoE

## Executive summary

Ronny Kohavi, widely regarded as the world's leading expert on A/B testing, shares hard-won lessons from running tens of thousands of experiments at Microsoft, Amazon, and Airbnb. His central message: most ideas fail (66-92% depending on maturity), and organizations that do not rigorously test every code change are unknowingly shipping degradations. Trust in the experimentation platform, not speed, is the most critical factor for building an experiment-driven culture.

## Key ideas

1. **Most ideas fail -- and that is normal** — At Microsoft, ~66% of experiments failed. At Bing (a more optimized product), ~85% failed. At Airbnb search, 92% failed. Google, Booking.com, and others report 80-90% failure rates. This is not a sign of bad PMs; it is the baseline reality of product development. Yet every new team believes they will be different.

2. **Test everything** — Every code change, even small bug fixes, should be in an experiment. A trivial change at Bing (promoting the second ad-title line to the first) generated $100M/year in revenue -- the biggest win in Bing's history. It had languished in the backlog for months because nobody rated it highly.

3. **The Overall Evaluation Criterion (OEC)** — Teams must define what they are optimizing for as a composite metric causally predictive of long-term user lifetime value. Revenue alone is insufficient because you can always increase short-term revenue by degrading user experience (e.g., more ads). The OEC must include countervailing/guardrail metrics (time-to-task-completion, churn, session success rate). If the team cannot agree on the directionality of a metric, that metric should not be in the OEC.

4. **Twyman's Law** — "Any figure that looks interesting or different is usually wrong." When an experiment shows a surprisingly large positive result, the first reaction should be investigation, not celebration. Nine out of ten times, there is a flaw. Replicate before shipping.

5. **Sample Ratio Mismatch (SRM)** — The single most common validity threat. If you design a 50/50 split and observe 50.2/49.8 with a million users, that is statistically implausible and signals a corrupted experiment. At Microsoft, ~8% of experiments suffered from SRM. Common causes: bots, data pipeline issues, skewed campaign traffic.

6. **Big redesigns usually fail** — Full product redesigns almost always produce negative or flat results. The better approach is OFAT (One Factor At a Time): decompose redesigns into incremental changes, test each, and ship only the winners. Allocate ~20% of effort to high-risk/high-reward bets, but expect 80% of those to fail.

7. **P-values are widely misunderstood** — A P-value of 0.05 does not mean there is a 95% chance the treatment is better. At Airbnb (where only 8% of ideas succeed), a statistically significant result at p<0.05 still carries a 26% false positive risk. Kohavi recommends replicating experiments and combining P-values via Fisher's or Stouffer's method.

8. **Building an experimentation culture** — Start with a beachhead team that ships frequently. Share surprising results (both wins and losses) in quarterly reviews to build institutional learning. Invest in the platform to drive marginal experiment cost toward zero. When leadership resistance exists, let the data from the beachhead team create the pull.

## Entities mentioned

- **Companies/products**: Microsoft (Bing, Office, MSN), Amazon, Airbnb, Optimizely, Booking.com, Google, Eppo, Mixpanel, goodui.org
- **People**: Ronny Kohavi, Qi Lu, Satya Nadella, Greg Greeley, Brian Chesky, Ramesh Johari, Shreyas Doshi, Ricardo (Airbnb)
- **Frameworks/books**: *Trustworthy Online Controlled Experiments* (Kohavi, Tang, Xu), *Calling Bullshit* (Bergstrom & West), *Hard Facts, Dangerous Half-Truths And Total Nonsense* (Pfeffer & Sutton), *Mistakes Were Made (But Not by Me)* (Tavris & Aronson)

## Concepts that deserve their own wiki page

- **[[A/B testing]]** — Controlled online experiments comparing treatment vs. control to measure causal impact of product changes
- **[[Overall Evaluation Criterion (OEC)]]** — Composite metric designed to be causally predictive of long-term user lifetime value, balancing business goals with user experience guardrails
- **[[Twyman's Law]]** — Heuristic that any statistical figure that looks surprisingly interesting or different is probably wrong
- **[[Sample Ratio Mismatch]]** — Validity check comparing observed vs. expected user allocation in an experiment; the most common indicator of a corrupted test

## Notable quote

> "I'm very clear that I'm a big fan of test everything. Any code change that you make, any feature that you introduce has to be in some experiment. Because I've observed this surprising result that even small bug fixes, even small changes can sometimes have surprising, unexpected impact."

## B11 angle

Kohavi's data on experiment failure rates (66-92%) provides strong empirical backing for the humility that other Lenny Podcast guests advocate around product intuition. His OEC concept connects to discussions of [[metrics]] and [[North Star metrics]] across the wiki. The tension between Kohavi's "test everything" philosophy and Airbnb's shift toward top-down design-driven leadership under Brian Chesky offers a fascinating case study in experimentation culture vs. visionary leadership.
