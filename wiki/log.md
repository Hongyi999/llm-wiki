---
title: Wiki Log
type: log
created: 2026-04-10
updated: 2026-04-10
---

# Wiki Log

Chronological record of all wiki operations.

## [2026-04-10] init | Wiki initialized

Wiki starter kit created with CLAUDE.md schema, index.md, and log.md.

## [2026-04-10] ingest | Sean Ellis — The Original Growth Hacker Reveals His Secrets

Ingested `raw/sean-ellis.md`. Created source page [[source-sean-ellis-growth-hacker]]; entity pages [[sean-ellis]], [[dropbox]], [[xobni]], [[lookout]], [[logmein]]; concept pages [[sean-ellis-test]], [[growth-hacking]], and root [[product-market-fit]].

## [2026-04-10] ingest | Rahul Vohra — Superhuman's Secret to Success

Ingested `raw/rahul-vohra.md`. Created source page [[source-rahul-vohra-superhuman]]; entity pages [[rahul-vohra]], [[superhuman]]; concept pages [[superhuman-pmf-engine]], [[solution-deepening-vs-market-widening]].

## [2026-04-10] ingest | Todd Jackson — A Framework for Finding Product-Market Fit

Ingested `raw/todd-jackson.md`. Created source page [[source-todd-jackson-pmf-framework]]; entity pages [[todd-jackson]], [[first-round-capital]], [[vanta]]; concept pages [[four-levels-of-pmf]], [[four-ps-framework]], [[dollar-driven-discovery]].

## [2026-04-10] ingest | Benjamin Lauzier — How Marketplaces Win

Ingested `raw/benjamin-lauzier.md`. Created source page [[source-benjamin-lauzier-marketplaces]]; entity pages [[benjamin-lauzier]], [[lyft]], [[thumbtack]]; concept page [[marketplace-liquidity]].

## [2026-04-10] ingest | Jen Abel — The Ultimate Guide to Founder-Led Sales

Ingested `raw/jen-abel.md`. Created source page [[source-jen-abel-founder-led-sales]]; entity pages [[jen-abel]], [[jjellyfish]]; concept page [[founder-led-sales]].

## [2026-04-10] synthesis | PMF batch synthesis across 5 sources

After ingesting all 5 PMF-focused transcripts, created comparison page [[comparison-pmf-measurement-approaches]] (Sean Ellis Test vs. Superhuman PMF Engine vs. Four Levels of PMF vs. Marketplace Liquidity) and synthesis page [[synthesis-pmf-signals]] (cross-source signals and anti-signals of real PMF).

## [2026-04-10] restructure | raw/ reorganized into per-source subdirectories

Moved all 303 Lenny's Podcast transcripts from `raw/*.md` to `raw/lenny-podcast/*.md` via `git mv` (preserves history). Updated CLAUDE.md schema to clarify that raw file **contents** are immutable but **directory structure** may be reorganized on explicit user request. Updated `raw/README.md` to document the new convention. Updated `sources:` frontmatter in all 32 existing wiki pages to use the new `lenny-podcast/` path prefix.

## [2026-04-10] ingest-bulk | 298 stub source pages auto-generated

Generated stub source pages for every Lenny's Podcast transcript not yet deeply ingested (298 of 303 total). Each stub is auto-extracted from the transcript's YAML frontmatter (title, guest, publish_date, duration, description, keywords) and tagged with `status: stub` for easy filtering. Stubs live at `wiki/source-<stem>.md`. Created [[index-stubs]] as an auto-generated index grouped by publish year. Deep analysis (entity / concept / synthesis pages) is done on-demand per topic or per guest — see [[index-stubs]] for the full catalog.

## [2026-04-11] plan | 11-batch thematic deep-ingest plan

Clustered all 298 stub sources by theme via regex over `title + description`, producing a batch plan for on-demand deep ingest. Final distribution: AI products (65), product discovery & PM craft (61), hiring & management (52), growth (31), positioning & narrative (22), sales+GTM+pricing (22), design+founder (24), data+career+misc (21). AI products and product discovery and hiring are split into two parts each to keep batch sizes 20–35 sources. See [[index-by-theme]] for the full ordered batch plan. No source pages changed in this step — only the plan doc and index update. Deep ingest begins with B1 on user confirmation.

## [2026-04-11] lint | Pre-B1 dedup — 11 duplicate raw transcripts removed

Ran SHA-256-based content dedup on 303 raw transcripts. Found 11 duplicate pairs across 4 categories: 6 exact-byte duplicates (e.g. `andy-raskin_` vs `andy-raskin`, `fei-fei` vs `dr-fei-fei-li`, `wes-kao-20` vs `wes-kao`), 2 same-episode transcription variants (kept longer body: `tomer-cohen`, `uri-levine`), 2 mislabeled filename cases (`melissa.md` had Melissa Perri content under Melissa Tan frontmatter; `ryan-hoover.md` was misnamed Shape Up transcript — kept `melissa-tan.md` and `ryan-singer.md`), and 1 near-duplicate with 97% similarity (`hamelshreya` vs `hamel-husain-shreya-shankar`, kept full-name file). Removed 22 files total (11 raw + 11 stub wiki pages). Updated [[index-stubs]], [[index-by-theme]], and [[index]] to reflect 287 unique stubs (down from 298). Batch-size impact: B1 dropped from 33 → 29. Full report at [[lint-dedup]].
