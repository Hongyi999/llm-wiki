---
title: "Source: Building a world-class data org ft. Jessica Lachs"
type: source
created: 2026-04-10
updated: 2026-04-19
tags: [analytics, data-science, metrics, org-design, doordash, marketplace, hiring]
sources: [lenny-podcast/jess-lachs.md]
---

# Source: Building a world-class data org ft. Jessica Lachs

**Guest**: Jessica Lachs (VP of Analytics and Data Science, DoorDash)
**Published**: 2024-07-14
**Duration**: ~1h 20m
**YouTube**: https://www.youtube.com/watch?v=D4PDb_C8Dww

## Executive summary

Jessica Lachs shares how she built one of tech's largest and most respected data organizations at DoorDash over 10+ years — starting as a self-taught data scientist who learned SQL and Python out of necessity. She makes a strong case for a centralized analytics org that earns its seat at the table by proactively finding opportunities (not just answering questions), and offers deeply practical advice on picking metrics that actually drive behavior.

## Key ideas

1. **Centralized analytics org with embedded pods** — Analytics should report through a single central org (center of excellence), not be embedded in business units. But the team is organized into pods that map to product/engineering/ops, sharing the same goals as partner teams. This preserves talent consistency, career mobility, methodology standards, and team culture while solving for the "ownership" concern of embedded models.

2. **Analytics as business impact, not service** — The team's job is not just answering "why" but answering "so what do we do now?" Analysts should have a point of view on decisions, proactively find opportunities through deep dives and hackathons, and earn their seat at the table by driving roadmaps — not processing Jira tickets.

3. **Short-term proxy metrics for long-term outcomes** — "Retention is a terrible thing to goal on" because it is nearly impossible to move in the short term. Instead, find input metrics that you can experiment on quickly and validate that they drive the long-term output. Keep metrics simple: composite scores with coefficients become meaningless. Even if imperfect, a metric everyone understands outperforms a "perfect" one nobody can interpret.

4. **Common currency across the business** — Quantify every lever (price reduction, delivery time improvement, new restaurant) in terms of a shared unit (GOV/volume). This lets you compare a dollar spent on marketing versus logistics versus merchant acquisition and make faster, better trade-off decisions across a complex multi-sided marketplace.

5. **Goal on fail states, not just averages** — DoorDash tracks "Never Delivered" orders — extremely rare but devastatingly expensive and churn-inducing. These edge cases hide inside averages. Similarly, login failures are invisible because affected users never enter the data set. Dedicated teams goal on eradicating these fail states.

6. **Hiring for curiosity over credentials** — Technical skills are table stakes. The differentiator is curiosity: people who notice something odd in the data and pull the thread without being asked. Lachs herself is self-taught (art portfolio, investment banking background) and explicitly hires people smarter than her technically, then keeps them grounded in business impact.

7. **Extreme ownership culture** — From DoorDash's earliest days (handing out promo codes at 5 AM in Boston, the entire company jumping on customer support during outages), the culture expected everyone to do whatever was needed. Lachs extends this to data scientists: "If that means you pick up the phone and call customers, that is what you're going to do."

## Entities mentioned

- **Companies/products**: [[DoorDash]], Volt (DoorDash international), Airbnb, Lehman Brothers
- **People**: Jessica Lachs, [[Lenny Rachitsky]], Tony Xu, Elizabeth Stone, Riley Newman, Keith Yandell
- **Frameworks/books**: WeDash program, Office Hours, Gross Order Value (GOV)

## Concepts that deserve their own wiki page

- **[[Centralized Analytics Org]]** — Center-of-excellence model for data teams with embedded pods and shared goals
- **[[Proxy Metrics]]** — Short-term measurable inputs that drive long-term outputs like retention
- **[[Fail State Metrics]]** — Goaling on rare but catastrophic edge cases that hide inside averages

## Notable quote

> "Retention is a terrible thing to goal on. It's almost impossible to drive in a meaningful way in the short term. Ultimately, you want to find a short-term metric you can measure that drives a long-term output."

## B11 angle

Lachs's emphasis on extreme ownership and "do whatever it takes" culture echoes [[jeff-weinstein]]'s customer obsession at Stripe. Her proxy metrics framework connects to broader [[metrics]] discussions across the wiki. The centralized-but-embedded org model offers a counterpoint to fully embedded structures, relevant for anyone building [[data teams]] or [[analytics orgs]] at scale.
