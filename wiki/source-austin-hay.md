---
title: "Source: The Ultimate Guide to MarTech ft. Austin Hay"
type: source
created: 2026-04-10
updated: 2026-04-19
tags: [martech, growth, marketing-technology, tools, attribution, data-infrastructure, B2B, B2C]
sources: [lenny-podcast/austin-hay.md]
---

# Source: The Ultimate Guide to MarTech ft. Austin Hay

**Guest**: Austin Hay (Head of Marketing Technology, Ramp; formerly VP Growth at mParticle, 4th employee at Branch Metrics; Reforge instructor)
**Published**: 2023-08-13
**Duration**: ~1h 25m
**YouTube**: https://www.youtube.com/watch?v=B79p85DHLkU

## Executive summary

Austin Hay demystifies Marketing Technology (MarTech) as a discipline that sits at the intersection of product, engineering, growth, and marketing. His core thesis is that tools are meant to solve problems, not create them — and the best MarTech practitioners think backwards from problems and people before touching systems. He provides deeply tactical guidance on tool stacks, attribution architecture, and when companies need a dedicated MarTech hire.

## Key ideas

1. **Tools are meant to solve problems** — Austin's mantra and the organizing principle of his work. Most people jump straight to buying or building tools; the right approach is to start with the problem, understand the people involved, and only then design the system (his PPS framework: Problem, People, System).

2. **Build AND buy, not build vs. buy** — The false binary of building in-house versus purchasing a third-party tool misses the optimal path: buy a tool that gets you 90% of the way there, then build the remaining 10% on top of it. This saves engineering time, creates vendor alignment, and produces solutions uniquely tailored to your business.

3. **When to hire a MarTech person** — Companies typically hit a critical mass around 100-150 employees where the "village approach" to managing tools breaks down. The signal is pain: nobody knows how data flows, tools are too complex for one person, and the business can't move forward because changing a tool might break something. The best MarTech hires combine intellectual curiosity with scrappy engineering skills — they don't need to be software engineers, but they need to read API docs and write basic code.

4. **The end of deterministic attribution** — From 2010-2020, marketers enjoyed "golden years" of deterministic matching (IDFA, cookies). Post-iOS 14 and cookie deprecation, attribution is increasingly probabilistic. Austin recommends designing your tracking infrastructure for multi-touch attribution from day one — collecting first and last UTMs on both user profiles and events — even if you start with simple first-touch or last-touch models, so you have the data when you need it.

5. **B2C vs. B2B stack architecture** — B2C stacks center on a CDP (Segment, Amplitude) connecting to ad networks, email tools, and analytics. The modern evolution uses a data warehouse (Snowflake) with reverse ETLs (Census, Hightouch) to activate data. B2B stacks revolve around Salesforce with everything else orbiting it. B2B2C (e.g., Notion, Ramp) is the hardest because you must merge top-of-funnel user acquisition data with bottom-of-funnel CRM data.

6. **Thinking gray** — From Steven B. Sample's *The Contrarian's Guide to Leadership*: resist the pressure to make decisions quickly. Delay deciding for as long as you possibly can before you must. This applies to tool selection, people evaluation, and life decisions. Patience opens the possibility that you'll make a better decision with more information.

## Entities mentioned

- **Companies/products**: [[Ramp]], Branch Metrics, mParticle, Runway, Segment, Amplitude, Snowflake, Braze, Salesforce, HubSpot, Hightouch, Census, Rudder Stack, Snowplow, Split.io, Facebook/Meta, Reddit, Threads, Recast, Mixpanel
- **People**: Sri Batchu (Ramp), Siqi Chen (Runway CEO), Mike Molinet (Branch COO), Dmitri (Airbnb MarTech), Cody Morgan (Ramp UA)
- **Frameworks/books**: PPS (Problem, People, System), Build AND Buy, *The Contrarian's Guide to Leadership* (Steven B. Sample), *The Art and Adventure of Leadership* (Warren Bennis), Thinking Gray, Reforge MarTech course

## Concepts that deserve their own wiki page

- **[[MarTech]]** — The discipline of using technology and tools to drive growth, sitting at the crossroads of product, engineering, and marketing
- **[[Attribution]]** — Methods for measuring which marketing channels drive conversions (first-touch, last-touch, MTA, MMM)
- **[[Reverse ETL]]** — Moving data from a warehouse back out to operational tools, enabling a "composable CDP" architecture

## Notable quote

> "Tools are just meant to solve problems. You don't have to buy a tool to solve the problem. You also don't have to buy a specific tool to solve the problem."

## B10 angle

Austin's "tools solve problems" philosophy is a pragmatic counterweight to the tool-obsessed culture common in growth teams. His PPS framework (Problem, People, System) echoes product thinking seen across many Lenny episodes — understand the user and the problem before jumping to solutions. The attribution discussion connects to the broader [[data-informed vs. data-driven]] debate, and his advice on hiring MarTech talent complements discussions of [[growth team]] structure.
