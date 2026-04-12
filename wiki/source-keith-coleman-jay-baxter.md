---
title: "An inside look at X's Community Notes | Keith Coleman & Jay Baxter"
type: source
created: 2026-04-12
updated: 2026-04-12
tags: [community-notes, misinformation, crowdsourcing, machine-learning, small-teams, x-twitter, product-leadership, trust-and-safety]
sources: [lenny-podcast/keith-coleman-jay-baxter.md]
---

# An inside look at X's Community Notes | Keith Coleman & Jay Baxter

**Guest**: Keith Coleman & Jay Baxter  
**Published**: 2025-02-27  
**Duration**: 1:47:58  
**YouTube**: [https://www.youtube.com/watch?v=8dgyqYHLcCI](https://www.youtube.com/watch?v=8dgyqYHLcCI)

## Executive summary

Keith Coleman (VP of Product) and Jay Baxter (founding ML engineer) tell the origin story and inner workings of Community Notes, the crowdsourced fact-checking system on X/Twitter that has become the industry standard for combating misinformation at scale. The product works by surfacing context notes only when people who historically disagree with each other find a note helpful — a bridging-based algorithm that emerged from an internal bake-off over earlier PageRank approaches. The team operated as a 'Thermal' project inside Twitter: a small, fully dedicated squad with one clear decision-maker, no OKRs, and goals set dynamically from a single long-running Google Doc. With nearly a million volunteer contributors, Community Notes now shows hundreds of notes per day seen billions of times, causing 50-60% drops in reposts of noted misinformation — all without the ranking algorithm demoting posts.

## Key ideas

1. **Bridging-based consensus algorithm**: Community Notes does not use majority-rules voting. Instead, it surfaces notes only when people who have historically disagreed with each other agree a note is helpful. This approach emerged from an internal competition and replaced an earlier PageRank-based anti-manipulation model that could amplify partisan bias.

2. **Thermal team model for zero-to-one products**: The team operated as a 'Thermal' project — a small, fully dedicated squad with one clear founder-like owner (Keith), one senior decision-maker (first Kayvon, then Elon), 100% focus from every member, no OKRs, and dynamically set milestones. They ran off a single Google Doc and had no Jira or formal task management.

3. **Quality over coverage as a trust strategy**: Only about 8% of proposed notes are shown. The team deliberately sets a conservative threshold (0.4 on their scoring scale) because a single bad note undermines trust more than a missing good note hurts coverage. This quality-first approach is why Community Notes is broadly trusted.

4. **Massive behavioral impact without algorithmic demotion**: Noted posts see 50-60% drops in reposts and authors become 80% more likely to delete their post — all from organic user behavior, not from the ranking algorithm penalizing the content. External research confirms that people's agreement with core claims actually changes when they see the note.

5. **Open-source transparency as anti-manipulation defense**: The algorithm, data, and code are all publicly available. Contrary to the expectation that open-sourcing would invite manipulation, the bridging-based design makes gaming extremely difficult because attackers would need agreement from people who usually disagree with them.

## Entities discussed

- **Keith Coleman** — VP of Product at X and founder of the Community Notes (originally Birdwatch) project.
- **Jay Baxter** — Founding ML engineer and researcher for Community Notes who designed the bridging-based consensus algorithm.
- **Kayvon Beykpour** — Former Twitter executive who created the Thermal program and sponsored the Birdwatch project.
- **Elon Musk** — Owner of X who championed Community Notes and served as the team's senior decision-maker after the acquisition.
- **[[meta|X (Twitter)]]** — Social media platform where Community Notes operates, reaching billions of note impressions.
- **[[meta]]** — Adopted Community Notes as its primary fact-checking approach, replacing tens of thousands of fact checkers.

## Concepts covered

- **Bridging-based algorithm** — An ML approach that identifies consensus by finding agreement among people who historically disagree, using matrix factorization.
- **Thermal team** — An organizational model inside Twitter for small, fully dedicated teams with clear ownership and autonomy from standard corporate processes.
- **Community Notes** — A crowdsourced system on X where volunteer contributors add context to potentially misleading posts, surfaced via bridging-based consensus.
- **Matrix factorization** — The ML technique underlying the Community Notes scoring algorithm, fitted with gradient descent to identify bridging agreement.
- **Sawtooth career path** — Coleman's pattern of growing a team into a large organization, then jumping back to a small zero-to-one effort for higher impact.

## Notable quote

> Keith Coleman (00:39:37): 'If I had stayed running a large consumer PM team, what would I have produced? 16 more pages of OKRs? Building Community Notes has had way bigger impact on the world.'

## B3 angle

Reveals how a tiny autonomous team inside a large platform built the industry-standard crowdsourced fact-checking product by combining a novel bridging algorithm with radical operational simplicity.
