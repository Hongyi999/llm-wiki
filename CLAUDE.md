# LLM Wiki — Schema

This is a personal knowledge base maintained by an LLM agent. Obsidian is the viewer; you (the LLM) are the maintainer.

## Directory Structure

```
raw/            ← Immutable source documents. NEVER modify files here.
raw/assets/     ← Downloaded images referenced by raw sources.
wiki/           ← LLM-maintained wiki pages. You own this directory entirely.
wiki/index.md   ← Content catalog of all wiki pages.
wiki/log.md     ← Chronological append-only operation log.
CLAUDE.md       ← This file. The schema and operating instructions.
```

## Page Conventions

- All wiki pages are markdown files in `wiki/`.
- Use `[[wikilinks]]` for cross-references between pages.
- Every page must have YAML frontmatter:

```yaml
---
title: Page Title
type: source | entity | concept | comparison | synthesis
created: YYYY-MM-DD
updated: YYYY-MM-DD
tags: [tag1, tag2]
sources: [source-filename.md]
---
```

- Page types:
  - **source**: Summary of a single raw source document.
  - **entity**: A person, organization, product, or project.
  - **concept**: An idea, technique, framework, or theory.
  - **comparison**: Side-by-side analysis of two or more entities/concepts.
  - **synthesis**: Higher-order analysis combining multiple sources/concepts.

## Workflows

### Ingest

When told to process a new source in `raw/`:

1. Read the source document fully.
2. Discuss key takeaways with the user (if interactive).
3. Create a **source** page in `wiki/` summarizing the document.
4. Create or update **entity** pages for people, orgs, products mentioned.
5. Create or update **concept** pages for key ideas covered.
6. Add `[[wikilinks]]` in all new/updated pages to connect them.
7. Update `wiki/index.md` — add new pages with one-line summaries.
8. Append an entry to `wiki/log.md` in the format:
   `## [YYYY-MM-DD] ingest | Source Title`

### Query

When the user asks a question:

1. Read `wiki/index.md` to identify relevant pages.
2. Read those pages for context.
3. Synthesize an answer with citations to specific wiki pages.
4. If the answer is substantial and reusable, offer to save it as a new wiki page (type: synthesis or comparison).

### Lint

When told to lint or health-check the wiki:

1. Check for orphan pages (no inbound links from other wiki pages).
2. Check for contradictions between pages.
3. Check for stale claims that newer sources may have superseded.
4. Check for concepts mentioned but lacking their own page.
5. Check for missing cross-references.
6. Suggest new questions to investigate or sources to look for.
7. Append a lint entry to `wiki/log.md`:
   `## [YYYY-MM-DD] lint | Summary of findings`

## Guidelines

- Write clearly and concisely. Prefer short paragraphs over long blocks.
- When in doubt, create a new page rather than overloading an existing one.
- Always preserve source attribution — every claim should trace back to a raw source.
- Use consistent terminology. If a concept has multiple names, pick one canonical name and note aliases.
- The user reads the wiki in Obsidian. Make liberal use of `[[wikilinks]]` so the graph view is rich and navigable.
