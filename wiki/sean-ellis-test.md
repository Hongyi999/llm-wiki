---
title: Sean Ellis Test
type: concept
created: 2026-04-10
updated: 2026-04-10
tags: [product-market-fit, survey, measurement]
sources: [sean-ellis.md, rahul-vohra.md]
---

# Sean Ellis Test

A single-question survey used to measure [[product-market-fit|product-market fit]], invented by [[sean-ellis|Sean Ellis]] at [[xobni|Xobni]].

## The question

> **"How would you feel if you could no longer use this product?"**
>
> - Very disappointed
> - Somewhat disappointed
> - Not disappointed (I'd just move on)

## The 40% threshold

If **≥40%** of engaged users answer "very disappointed," you have sufficient PMF for sustainable growth. Below that, growth efforts tend to leak out the bottom of the funnel faster than they can be replaced.

The threshold is empirical — it came from Sean's observation of which products in his portfolio could scale profitably and which couldn't. It is a benchmark, not a law.

## How to run it

- **Survey engaged users only**, not all signups. Definition of "engaged" varies by product (e.g., used the product ≥3 times in the last 2 weeks).
- Don't show the options when asking — the labels are a forced choice.
- Ask **follow-up drill-downs** immediately:
  1. What type of person would most benefit from this product?
  2. What is the **main benefit** you receive?
  3. How can we improve it for you?

The "main benefit" answer from the "very disappointed" segment is usually the most important output — it tells you the real value prop, which is often different from what the founder thinks they're selling.

## Case studies

- **[[lookout|Lookout]]**: moved from **7% → 40%+** by repositioning from antivirus to lost-phone recovery based on the drill-down answers.
- **[[logmein|LogMeIn]]**: the survey was healthy but **activation was 5%**. After fixing onboarding, activation rose to ~50% and growth followed. Lesson: satisfaction PMF requires activation to convert into business outcomes.
- **Nubank**: ~50% "very disappointed." Growth nearly mechanical at that level.
- **TikTok** (anecdotally): so strong that there was nothing to fix at the PMF layer — pour fuel on the fire.

## Tooling

[[sean-ellis|Sean Ellis]] made the survey freely available at **PMFsurvey.com**.

## Extension

[[rahul-vohra|Rahul Vohra]] extended this test into the [[superhuman-pmf-engine|Superhuman PMF Engine]], which adds a segmentation step to create an actionable roadmap rather than just a score.

## Caveats and criticisms

- The 40% number is a benchmark, not a guarantee. Some products (two-sided marketplaces, enterprise) don't fit cleanly.
- A high score on a narrow user base is not the same as a high score at scale.
- The test measures **satisfaction** (one of [[four-levels-of-pmf|Todd Jackson's three dimensions]]). A product with 40% "very disappointed" but broken unit economics is not in PMF in the business sense.

## See also

- [[sean-ellis]], [[superhuman-pmf-engine]], [[product-market-fit]]
- [[comparison-pmf-measurement-approaches]]
