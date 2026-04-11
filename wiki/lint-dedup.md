---
title: Lint Report — Raw Transcript Deduplication
type: lint
created: 2026-04-11
updated: 2026-04-11
tags: [lint, dedup, raw-maintenance]
---

# Lint Report — Raw Transcript Deduplication

**Date**: 2026-04-11  
**Trigger**: Pre-B1 dedup check before deep-ingesting 298 stub Lenny's Podcast transcripts.

## Summary

- Scanned: 303 raw files in `raw/lenny-podcast/`
- Duplicate pairs found: **11**
- Files deleted: **11**
- Unique transcripts remaining: **292**

Detection method: SHA-256 over whitespace-normalized body (post-frontmatter). For non-matching hashes, cross-check publish_date + title → flag same-episode variants, then compute sequence similarity over first 5000 chars to decide.

## Decisions

| # | Category | Sim | Keep | Delete | Reason |
|---:|---|---:|---|---|---|
| 1 | 🟢 Exact duplicate | 100.0% | `andy-raskin.md` | `andy-raskin_.md` | Content bytes identical — safe auto-delete; picked cleaner filename. |
| 2 | 🟢 Exact duplicate | 100.0% | `dr-fei-fei-li.md` | `fei-fei.md` | Content bytes identical — safe auto-delete; picked cleaner filename. |
| 3 | 🟢 Exact duplicate | 100.0% | `ethan-evans.md` | `ethan-evans-20.md` | Content bytes identical — safe auto-delete; picked cleaner filename. |
| 4 | 🟢 Exact duplicate | 100.0% | `nicole-forsgren.md` | `nicole-forsgren-20.md` | Content bytes identical — safe auto-delete; picked cleaner filename. |
| 5 | 🟢 Exact duplicate | 100.0% | `wes-kao.md` | `wes-kao-20.md` | Content bytes identical — safe auto-delete; picked cleaner filename. |
| 6 | 🟢 Exact duplicate | 100.0% | `yuhki-yamashata.md` | `yamashata.md` | Content bytes identical — safe auto-delete; picked cleaner filename. |
| 7 | 🟡 Same-episode variant | 15.4% | `tomer-cohen.md` | `tomer-cohen-20.md` | Same episode (title + publish_date match) but different transcription versions. Kept the longer, more complete body. |
| 8 | 🟡 Same-episode variant | 17.6% | `uri-levine.md` | `uri-levine-20.md` | Same episode (title + publish_date match) but different transcription versions. Kept the longer, more complete body. |
| 9 | 🟠 Mislabeled filename | 16.9% | `melissa-tan.md` | `melissa.md` | Filename does not match content or another pair has the canonical version; kept the one where filename/title/content are consistent. |
| 10 | 🟠 Mislabeled filename | 15.6% | `ryan-singer.md` | `ryan-hoover.md` | Filename does not match content or another pair has the canonical version; kept the one where filename/title/content are consistent. |
| 11 | 🟢 Near-exact duplicate | 97.1% | `hamel-husain-shreya-shankar.md` | `hamelshreya.md` | 97%+ body similarity over first 5KB; kept the full-proper-name filename. |

## Per-pair detail

### 1. andy-raskin ← andy-raskin_ (🟢 Exact duplicate)

- **Similarity**: 100.0%
- **Publish date**: 2023-05-28 (both files match)
- **Title**: `The power of strategic narrative | Andy Raskin`
- **Kept** `andy-raskin.md` — 61852 body chars
- **Deleted** `andy-raskin_.md` — 61852 body chars
- **Reason**: Content bytes identical — safe auto-delete; picked cleaner filename.

### 2. dr-fei-fei-li ← fei-fei (🟢 Exact duplicate)

- **Similarity**: 100.0%
- **Publish date**: 2025-11-16 (both files match)
- **Title**: `The Godmother of AI on jobs, robots & why world models are next | Dr. Fei-Fei Li`
- **Kept** `dr-fei-fei-li.md` — 66536 body chars
- **Deleted** `fei-fei.md` — 66536 body chars
- **Reason**: Content bytes identical — safe auto-delete; picked cleaner filename.

### 3. ethan-evans ← ethan-evans-20 (🟢 Exact duplicate)

- **Similarity**: 100.0%
- **Publish date**: 2024-01-14 (both files match)
- **Title**: `Taking control of your career | Ethan Evans (Amazon)`
- **Kept** `ethan-evans.md` — 81420 body chars
- **Deleted** `ethan-evans-20.md` — 81420 body chars
- **Reason**: Content bytes identical — safe auto-delete; picked cleaner filename.

### 4. nicole-forsgren ← nicole-forsgren-20 (🟢 Exact duplicate)

- **Similarity**: 100.0%
- **Publish date**: 2025-10-19 (both files match)
- **Title**: `How to measure AI developer productivity in 2025 | Nicole Forsgren`
- **Kept** `nicole-forsgren.md` — 74529 body chars
- **Deleted** `nicole-forsgren-20.md` — 74529 body chars
- **Reason**: Content bytes identical — safe auto-delete; picked cleaner filename.

### 5. wes-kao ← wes-kao-20 (🟢 Exact duplicate)

- **Similarity**: 100.0%
- **Publish date**: 2022-08-28 (both files match)
- **Title**: `Persuasive communication and managing up | Wes Kao (Maven, altMBA, Section4)`
- **Kept** `wes-kao.md` — 98893 body chars
- **Deleted** `wes-kao-20.md` — 98893 body chars
- **Reason**: Content bytes identical — safe auto-delete; picked cleaner filename.

### 6. yuhki-yamashata ← yamashata (🟢 Exact duplicate)

- **Similarity**: 100.0%
- **Publish date**: 2023-01-08 (both files match)
- **Title**: `An inside look at how Figma builds product | Yuhki Yamashita (CPO of Figma)`
- **Kept** `yuhki-yamashata.md` — 72973 body chars
- **Deleted** `yamashata.md` — 72973 body chars
- **Reason**: Content bytes identical — safe auto-delete; picked cleaner filename.

### 7. tomer-cohen ← tomer-cohen-20 (🟡 Same-episode variant)

- **Similarity**: 15.4%
- **Publish date**: 2025-12-04 (both files match)
- **Title**: `Why AI is disrupting traditional product management | Tomer Cohen (LinkedIn CPO)`
- **Kept** `tomer-cohen.md` — 74847 body chars
- **Deleted** `tomer-cohen-20.md` — 74210 body chars
- **Reason**: Same episode (title + publish_date match) but different transcription versions. Kept the longer, more complete body.

### 8. uri-levine ← uri-levine-20 (🟡 Same-episode variant)

- **Similarity**: 17.6%
- **Publish date**: 2025-02-16 (both files match)
- **Title**: `A founder’s guide to crisis management | Uri Levine (Waze co-founder, serial entrepreneur)`
- **Kept** `uri-levine.md` — 81345 body chars
- **Deleted** `uri-levine-20.md` — 75933 body chars
- **Reason**: Same episode (title + publish_date match) but different transcription versions. Kept the longer, more complete body.

### 9. melissa-tan ← melissa (🟠 Mislabeled filename)

- **Similarity**: 16.9%
- **Publish date**: 2023-06-18 (both files match)
- **Title**: `Building high-performing teams | Melissa Tan (Webflow, Dropbox, Canva)`
- **Kept** `melissa-tan.md` — 82919 body chars
- **Deleted** `melissa.md` — 59713 body chars
- **Reason**: Filename does not match content or another pair has the canonical version; kept the one where filename/title/content are consistent.

### 10. ryan-singer ← ryan-hoover (🟠 Mislabeled filename)

- **Similarity**: 15.6%
- **Publish date**: 2025-03-30 (both files match)
- **Title**: `A better way to plan, build, and ship products | Ryan Singer (creator of “Shape Up")`
- **Kept** `ryan-singer.md` — 107992 body chars
- **Deleted** `ryan-hoover.md` — 83395 body chars
- **Reason**: Filename does not match content or another pair has the canonical version; kept the one where filename/title/content are consistent.

### 11. hamel-husain-shreya-shankar ← hamelshreya (🟢 Near-exact duplicate)

- **Similarity**: 97.1%
- **Publish date**: 2025-09-25 (both files match)
- **Title**: `Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shanka`
- **Kept** `hamel-husain-shreya-shankar.md` — 108488 body chars
- **Deleted** `hamelshreya.md` — 108483 body chars
- **Reason**: 97%+ body similarity over first 5KB; kept the full-proper-name filename.

## See also

- [[index]] — main wiki catalog
- [[index-stubs]] — stub source catalog (updated to remove deleted entries)
- [[index-by-theme]] — batch plan (updated to remove deleted entries)
- [[log]] — operation log
