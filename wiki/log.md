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

## [2026-04-11] ingest-batch | B1 — AI products & LLMs 2025+ (29 sources)

Deep-ingested the full **B1** batch: 29 Lenny's Podcast transcripts on AI products from 2025 onward. Tier-B depth (executive summary + 3-5 key ideas + entities + concepts + quote + B1-angle, with wikilinks to shared cross-source pages rather than creating a standalone page for every single-source mention).

**Pipeline**: 6 parallel subagents read 4-5 transcripts each and wrote structured JSON summaries to `/tmp/b1/*.json`. One agent (group 3) refused the first pass; re-dispatched as two smaller groups (2+3). All 29 JSON files validated against a strict schema (exec_summary, key_ideas, entities, concepts, quote, tags, b1_angle). A Python generator then batch-produced the 29 source pages with consistent structure and canonicalized wikilinks.

**Pages created (55 total)**:
- **29 source pages** replacing the B1 stubs: [[source-aishwarya-naresh-reganti-kiriti-badam]], [[source-jason-m-lemkin]], [[source-sander-schulhoff-20]], [[source-elena-verna-40]], [[source-edwin-chen]], [[source-tomer-cohen]], [[source-dr-fei-fei-li]], [[source-grant-lee]], [[source-dhanji-r-prasanna]], [[source-chip-huyen]], [[source-nicole-forsgren]], [[source-dylan-field]], [[source-robby-stein]], [[source-jason-droege]], [[source-hamel-husain-shreya-shankar]], [[source-julian-shapiro]], [[source-julie-zhuo]], [[source-brendan-foody]], [[source-ethan-smith]], [[source-howie-liu]], [[source-asha-sharma]], [[source-garrett-lord]], [[source-eoghan-mccabe]], [[source-brian-balfour]], [[source-nick-turley]], [[source-bret-taylor]], [[source-madhavan-ramanujam]], [[source-dan-shipper]], [[source-brandon-chu]].
- **15 entity pages**:
  - Cross-source (≥2 sources, 10): [[openai]], [[anthropic]], [[chatgpt]], [[scale-ai]], [[figma]], [[sierra-ai]], [[salesforce]], [[meta]], [[google]], [[webflow]].
  - Single-source B1 hubs (5): [[linkedin]], [[gamma]], [[block]], [[mercor]], [[world-labs]].
- **9 concept pages**:
  - Cross-source clusters (6): [[ai-evals]], [[ai-agents]], [[outcomes-based-pricing]], [[ai-native-organization]], [[post-training-data-moat]], [[product-velocity-ai-era]].
  - Named single-source (3): [[answer-engine-optimization]], [[spatial-intelligence]], [[developer-experience]].
- **1 comparison + 1 synthesis**: [[comparison-b1-ai-product-approaches]] (groups the 29 guests into 10 schools of thought with explicit disagreements) and [[synthesis-b1-ai-product-patterns]] (9 convergent cross-source patterns + anti-signals).

**Cross-source stats**: OpenAI is the most-referenced entity (10/29 sources). The evals-first, post-training-data, and AI-native-org patterns each span 6-7 sources. The deepest disagreement is between Hamel Husain (evals-first) and Chip Huyen (users-first).

**Index updates**: [[index]] now lists 34 deep source pages (5 PMF + 29 B1). [[index-stubs]] drops from 287 → 258. [[index-by-theme]] marks B1 as ✅ done. B2 (32 older AI transcripts) is next, pending user review.

## [2026-04-12] ingest-batch | B2 — AI products & LLMs 2024 & earlier (32 sources)

Deep-ingested the full **B2** batch: 32 Lenny's Podcast transcripts on AI products spanning 2022–2025. Tier-B depth (same pipeline as B1).

**Pipeline**: 6 parallel subagents read 5-6 transcripts each and wrote structured JSON summaries to `/tmp/b2/*.json`. All 32 validated against schema. Python generator batch-produced source pages with canonicalized wikilinks. Entity, concept, comparison, and synthesis pages written in parallel.

**Pages created/updated (57 total)**:
- **32 source pages** replacing B2 stubs.
- **16 new entity pages**:
  - Cross-source (6): [[cursor]] (7 sources, most-referenced), [[github-copilot]], [[microsoft]], [[github]], [[slack]], [[glean]].
  - Single-source hubs (10): [[bolt]], [[lovable]], [[devin]], [[windsurf]], [[replit]], [[v0]], [[intercom]], [[canva]], [[palantir]], [[spotify]].
- **4 existing entity pages updated**: [[openai]] (+11 B2 sources), [[anthropic]] (+5), [[chatgpt]] (+6), [[google]] (+6).
- **5 concept pages**: [[ai-coding-tools]] (12 sources, the defining B2 theme), [[taste-as-differentiator]] (6 sources), [[prompt-engineering-techniques]] (Sander Schulhoff's definitive treatment), [[jevons-paradox-software]] (2 sources), [[minimum-lovable-product]] (2 sources).
- **1 comparison + 1 synthesis**: [[comparison-b2-ai-product-approaches]] (10 schools of thought, 6 key disagreements) and [[synthesis-b2-ai-product-patterns]] (9 convergent patterns + anti-signals).

**Cross-source stats**: OpenAI again most-referenced (11/32). Cursor is the most-referenced new entity (7/32). Claude Sonnet identified as a step-function moment by 5 independent founders. The deepest disagreement: human-in-loop (Cursor/Windsurf) vs. fully autonomous (Devin).

**Data issues found**: `kim-scott.md` had Scott Wu's YAML frontmatter (transcript content is Kim Scott); `jackie-bavaro.md` had Claire Vo's YAML frontmatter. Both handled at generation time — correct guest names used, titles overridden.

**Index updates**: [[index]] now lists 66 deep source pages (5 PMF + 29 B1 + 32 B2). [[index-stubs]] drops from 258 → 226. [[index-by-theme]] marks B2 as ✅ done. B3 (product strategy & PM craft, newer) is next.

## [2026-04-12] ingest-batch | B3 — Product strategy & PM craft, Part 1 (30 sources)

Deep-ingested the full **B3** batch: 30 Lenny's Podcast transcripts on product strategy and PM craft (newer episodes). Tier-B depth (same pipeline as B1/B2).

**Pipeline**: 6 parallel subagents read 5 transcripts each and wrote structured JSON summaries to `/tmp/b3/*.json`. All 30 validated against schema. Python generator batch-produced source pages with canonicalized wikilinks. Entity, concept, comparison, and synthesis pages written in parallel.

**Pages created/updated (48 total)**:
- **30 source pages** replacing B3 stubs.
- **8 new entity pages**:
  - Cross-source (2): [[atlassian]] (2 guests: Tanguy Crusson + Megan Cook), [[uber]] (4 sources).
  - Single-source hubs (6): [[y-combinator]], [[tiktok]], [[opendoor]], [[rippling]], [[gojek]], [[basecamp]].
- **1 existing entity page updated**: [[figma]] (+1 B3 source: Dylan Field's second episode).
- **6 concept pages**: [[jobs-to-be-done]] (2 sources), [[product-operating-model]] (5 sources, the defining B3 concept), [[counter-positioning]] (2 sources), [[seven-powers]] (Hamilton Helmer), [[strategy-choice-cascade]] (Roger Martin + Rumelt + Janakiraman), [[shape-up]] (Ryan Singer).
- **1 comparison + 1 synthesis**: [[comparison-b3-product-strategy-approaches]] (8 schools of thought, 6 key disagreements) and [[synthesis-b3-product-strategy-patterns]] (9 convergent patterns + anti-signals).

**Cross-source stats**: Uber is the most-referenced entity (4/30 sources). The product-operating-model / PM-reform cluster spans 5 sources (the batch's strongest theme). Three canonical strategy thinkers (Helmer, Martin, Rumelt) provide complementary frameworks. The deepest disagreement: whether strategy matters early (Helmer yes, Kamat/Caldwell no).

**Data issues found**: `matt-mullenweg.md` had YAML duplicated from `matt-lemay.md`; `ray-cao.md` had Marty Cagan's YAML frontmatter. Both handled at generation time with title overrides.

**Index updates**: [[index]] now lists 96 deep source pages (5 PMF + 29 B1 + 32 B2 + 30 B3). [[index-stubs]] drops from 226 → 196. [[index-by-theme]] marks B3 as ✅ done. B4 (product strategy & PM craft, older) is next.

## [2026-04-13] ingest-batch | B4 — Product strategy & PM craft, Part 2 (29 sources)

Deep-ingested the full **B4** batch: 29 Lenny's Podcast transcripts on product strategy and PM craft (older 2022–2023 episodes). Tier-B depth, but written incrementally one page at a time to avoid API stream-idle timeouts that hit on large parallel batches.

**Pipeline change**: Switched away from the Python-generator batch approach used for B1/B2/B3. After two successive `API Error: Stream idle timeout` events on large parallel writes, split the work into per-page Read → Write cycles with no parallelism on page writing. 6 parallel subagents did the initial transcript-reading pass. Subsequent page generation was serial: 29 source pages plus supporting entity/concept/comparison/synthesis pages, each written as its own `Write` tool call.

**Pages created/updated (40 total)**:
- **29 source pages** replacing B4 stubs: [[source-chip-conley]], [[source-maggie-crowley]], [[source-bob-moesta-20]], [[source-hari-srinivasan]], [[source-casey-winters]], [[source-shweta-shriva]], [[source-nikita-bier]], [[source-nikita-miller]], [[source-claire-hughes-johnson]], [[source-annie-pearl]], [[source-upasna-gautam]], [[source-marty-cagan-20]], [[source-zoelle-egner]], [[source-ravi-mehta]], [[source-john-cutler]], [[source-yuhki-yamashata]], [[source-chris-hutchins]], [[source-petra-wille]], [[source-ian-mcallister]], [[source-lauren-ipsen]], [[source-fareed-mosavat]], [[source-adriel-frederick]], [[source-janna-bastow]], [[source-teresa-torres]], [[source-jason-shah]], [[source-shreyas-doshi]], [[source-shreyas-doshi-live]], [[source-shishir-mehrotra]], [[source-nickey-skarstad]].
- **2 new entity pages**: [[amazon]] (cross-source; 3+ guests), [[reforge]] (Fareed Mosavat + Casey Winters + others).
- **7 new concept pages**: [[working-backwards]] (Amazon PR/FAQ), [[lno-framework]] (Shreyas Doshi's L/N/O task taxonomy), [[opportunity-solution-tree]] (Teresa Torres), [[now-next-later-roadmap]] (Janna Bastow), [[continuous-discovery]] (Teresa Torres), [[product-strategy-stack]] (Ravi Mehta), [[rituals-of-great-teams]] (Shishir Mehrotra), [[product-leader-canyon]] (Fareed Mosavat), [[pre-mortem]] (Shreyas Doshi).
- **1 comparison + 1 synthesis**: [[comparison-b4-product-strategy-approaches]] (7 schools of thought, 6 key disagreements) and [[synthesis-b4-product-strategy-patterns]] (8 convergent patterns).

**Cross-source stats**: The strongest B4 theme is the **PM career as skill reset, not extension** — spanning Mosavat, McAllister, Doshi, Shah, and Ipsen. The modern-product-operating-system artifact trio (Product Strategy Stack + Now/Next/Later + Opportunity Solution Tree) converges cleanly across three independent guests (Mehta, Bastow, Torres). Shishir Mehrotra's rituals concept is the operating-rhythm anchor.

**Data issues found**: `chip-conley.md` raw file YAML carried Maggie Crowley's title/description; `nikita-bier.md` raw file YAML carried Nikita Miller's title. Both corrected in the source pages with explanatory notes. `shreyas-doshi-live.md` and `shreyas-doshi.md` share an (incorrect) YouTube URL but have distinct transcript content — treated as two episodes.

**Index updates**: [[index]] now lists 125 deep source pages (5 PMF + 29 B1 + 32 B2 + 30 B3 + 29 B4). [[index-stubs]] drops from 196 → 167. [[index-by-theme]] marks B4 as ✅ done. B5 (hiring, management & leadership, Part 1) is next.
