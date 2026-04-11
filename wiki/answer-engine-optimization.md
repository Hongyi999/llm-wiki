---
title: Answer Engine Optimization (AEO)
type: concept
created: 2026-04-11
updated: 2026-04-11
tags: [growth, seo, ai-products, search]
sources: [lenny-podcast/ethan-smith.md, lenny-podcast/robby-stein.md]
---

# Answer Engine Optimization (AEO)

The successor discipline to SEO: the practice of structuring and distributing content so that large language models surface it as a **cited source** in their generated answers. In B1, [[source-ethan-smith|Ethan Smith]] is the definitive episode; [[source-robby-stein|Robby Stein]]'s episode on Google Search provides the complementary view from the platform side.

## Core claims ([[source-ethan-smith|Ethan Smith]])

- **Rankings don't matter the way they used to.** When a user asks ChatGPT or Google AI Mode a question, the answer is synthesized from a small number of sources — typically 3 to 10 — and those sources don't appear in the order that traditional SEO would predict.
- **Citations across tiers win.** The best AEO strategy is to be cited across multiple content types: Reddit threads, YouTube transcripts, long-form blogs, Wikipedia, authoritative news. Diversity of citations > pure PageRank.
- **The RAG layer is controllable, the model layer is not.** You can't influence how [[openai|OpenAI]] trains Claude, but you *can* influence what a RAG retrieval system surfaces today.
- **Topic coverage > backlinks.** Comprehensive coverage of a topic (every sub-question answered on one page) beats narrow, backlink-optimized pages.

## Complementary view from Google ([[source-robby-stein|Robby Stein]])

- **Query fan-out.** [[google|Google's]] AI Mode internally decomposes one user query into many parallel sub-queries against the index. This means the "retrieval target" is not a single keyword but a mesh of sub-intents.
- **AI search is expansionary.** Users who use AI Mode ask *more* questions in total, not fewer. Total demand for searchable content is growing, even if the interface changes.
- **Natural-language search is the new interface.** The content that wins in AEO is written in natural-language Q&A form, not keyword-stuffed headers.

## Tactics referenced in B1

1. Seed content on Reddit and other high-trust community sources.
2. Build YouTube presence — transcripts are read by LLMs.
3. Write FAQ and Q&A pages with natural-language sub-questions.
4. Get cited in Wikipedia where legitimate.
5. Topic-cluster content to maximize overlap with decomposed queries.

## See also

- [[source-ethan-smith]] — the B1 AEO playbook.
- [[source-robby-stein]] — how Google sees it from the platform side.
- [[google]], [[chatgpt]] — the answer engines.
