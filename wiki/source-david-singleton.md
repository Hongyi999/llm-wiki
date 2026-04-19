---
title: "Source: Building a Culture of Excellence ft. David Singleton"
type: source
created: 2026-04-10
updated: 2026-04-19
tags: [engineering-culture, craft, stripe, hiring, developer-productivity, friction-logging, reliability, co-creation]
sources: [lenny-podcast/david-singleton.md]
---

# Source: Building a Culture of Excellence ft. David Singleton

**Guest**: David Singleton (CTO, Stripe; formerly VP Engineering, Google)
**Published**: 2023-05-04
**Duration**: ~1h 30m
**YouTube**: https://www.youtube.com/watch?v=F0_IKKY3HCk

## Executive summary

David Singleton explains how Stripe operationalizes its "be meticulous in your craft" operating principle through concrete practices: friction logging, walking the store, engineer-cations, and co-creating products with early users. He argues that craft isn't just aesthetics — Stripe's obsessive attention to detail in checkout flows has measurably increased user revenue by 10.5%, and their error messages that link to documentation became a competitive moat for developer adoption.

## Key ideas

1. **Co-create with users** — Stripe's product development model centers on finding the right set of early users and building alongside them. For Stripe Billing, they partnered with companies like Figma and Slack via shared Slack channels, showing them product regularly and only going to a broader audience when the alpha group was "super, super happy." This approach means every engineer exercises PM-like attributes, which is why Stripe waited until roughly 200 employees to hire its first PM.

2. **Friction logging** — A widely used practice where someone puts themselves in a specific user's shoes, walks through the product end-to-end, and writes stream-of-consciousness notes on every point of friction. Done monthly by senior leaders (David personally friction-logs the onboarding flow once a month) and recursively across teams. Critically, it also praises what's working well — a chance to recognize great work.

3. **Be meticulous in your craft** — One of Stripe's operating principles, operationalized not as perfectionism everywhere, but as intentional investment where it matters most for users. The canonical example: Stripe's API error messages link directly to the relevant documentation page. There is more code handling edge cases in the API than in the main flow. This attention to high-stakes moments compounds — their payment element and Checkout product increased average user revenue by 10.5% through accumulated small improvements.

4. **Engineer-cations** — David clears 3-4 days, joins a team, picks up a small feature, and ships it end-to-end to production — experiencing the full developer workflow. He keeps a friction log throughout, then shares findings with the team. He recommends engineering managers do this within their first quarter at Stripe and annually thereafter. The name comes from treating it like vacation: decline all meetings and let the world go on without you.

5. **Walking the store** — Periodic company-wide sessions where the entire company looks at critical product flows together during Friday Fireside (a weekly all-hands). This creates shared language, aligns craft standards, and helps maintain cohesion as thousands of engineers work in parallel.

6. **Reliability through continuous deployment** — Stripe deploys to production automatically in ~45 minutes after code merge, averaging 16.4 deploys/day to the core API with 99.999% uptime. They achieve this through comprehensive automated test suites (no manual testers), progressive rollout to staging then small production percentages, auto-merge on PRs, selective test execution, and chaos testing. Incident remediations are prioritized ahead of the roadmap.

7. **Hiring through patience and references** — Stripe takes a very patient, personal approach to hiring. For critical roles, they'll meet tens or hundreds of candidates and sometimes wait years for the right person. They take reference checks unusually seriously — "If you've spent eight hours with someone in interviews, but you talk to people who have thousands of hours of direct experience working with them, references are often where you get the best conviction on the hire."

## Entities mentioned

- **Companies/products**: [[Stripe]], [[Google]], Figma, Slack, Atlassian, CloudFlare, OpenAI, Lyft, Shopify, Amazon, Nest
- **People**: John and Patrick Collison (Stripe co-founders), Claire Hughes Johnson, Shreyas Doshi, Jeff Weinstein (Atlas PM), Charlie Bell (Amazon), Tony Fadell, Andy Grove, Andrej Karpathy
- **Frameworks/books**: *High Output Management* (Andy Grove), *Build* (Tony Fadell), *Scaling People* (Claire Hughes Johnson), Stripe Operating Principles, Friction Logging template

## Concepts that deserve their own wiki page

- **[[Friction logging]]** — Structured practice of experiencing a product as a specific user and documenting every point of friction and delight
- **[[Meticulous craft]]** — The philosophy that sweating details at high-stakes user moments compounds into massive business impact
- **[[Co-creation with users]]** — Building products in partnership with carefully chosen early users via shared channels and rapid feedback loops
- **[[Engineer-cation]]** — Leaders temporarily joining engineering teams to ship code and experience the developer workflow firsthand

## Notable quote

> "There's actually more code in the jobs that serve the Stripe API to handle those edge cases than in the actual main flow. And I think that's quite remarkable. Most people wouldn't do that, but when I talk to Stripe users, this is very frequently something they tell me delights them about the product."

## B10 angle

David's friction logging practice and engineer-cations are the engineering equivalent of Maya Prohovnik's [[dogfooding|maya-prohovnik]] — leaders who insist on firsthand product experience rather than delegating understanding. The compound effect of meticulous craft (10.5% revenue uplift from small changes) mirrors the [[compound startup]] philosophy at [[Rippling|jeremy-henrickson]], where platform investment creates compounding returns. Stripe's patient, reference-heavy hiring approach and operating principles offer a concrete model for the "culture of excellence" that many companies aspire to but few operationalize.
