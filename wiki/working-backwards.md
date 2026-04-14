---
title: Working Backwards (PR/FAQ)
type: concept
created: 2026-04-13
updated: 2026-04-13
tags: [amazon, working-backwards, pr-faq, mechanism, problem-first-thinking]
sources: [lenny-podcast/ian-mcallister.md, lenny-podcast/bill-carr.md, lenny-podcast/jason-shah.md]
---

# Working Backwards (PR/FAQ)

**Working Backwards** is [[amazon|Amazon]]'s process for defining new products by writing a mock press release and FAQ *before* any engineering work starts. It forces the team to articulate the customer problem, the customer experience, and the hardest objections — in the customer's language — before committing resources.

## The artifact: PR + FAQ

- **Press Release (1 page)**: Dated for the launch. Written for a news audience. Includes headline, subhead, summary, problem statement, solution, quote from customer, quote from executive, and call to action.
- **FAQ (several pages)**: The hardest questions a customer, journalist, or internal skeptic would ask. Forces the team to do the hard thinking upfront — what would we need to be true about this market, this tech, this economics?

## The mechanism, not the artifact

The most common failure mode is treating the PR/FAQ as a document format to retrofit onto existing solutions. [[source-ian-mcallister]]'s B4 episode is the clearest articulation of the right mental model:

> "Working Backwards is about the problem, not the press release. The PR/FAQ is a mechanism to enforce problem-first thinking. The spirit of it can live in any document format."

Teams that cargo-cult the template without the problem-first intent produce the ceremony and none of the clarity. Teams that internalize the intent can produce the same rigor in a Google doc.

## When to use Working Backwards

- **New product definition** — Before investment, before engineering scope, before design.
- **Pivots and major feature bets** — When the direction of the work is unclear.
- **Cross-org alignment** — When multiple teams need a shared understanding of the target state.

## When not to

- **Known-problem incremental features** — PR/FAQs for minor tweaks is bureaucracy.
- **Early discovery** — Before you know the problem, you can't write a coherent press release. Use [[opportunity-solution-tree]]-style discovery first.
- **Pure 0→1 with no framing** — [[source-adriel-frederick]] warns that mature-Amazon governance kills incubation inside a mature org.

## Variants and descendants

- **Jeff Bezos's three investment tests** (via [[source-ian-mcallister]]):
  1. Is it a big idea?
  2. Is it something we should be doing?
  3. Is there a legitimate plan to succeed?
  All three must pass.
- **Bill Carr's *Working Backwards* book** — The canonical written reference. See [[source-bill-carr]].
- **Jason Shah's six-pager adaptation** — Amazon's six-pager narrative memo is the older cousin; PR/FAQ is the product-specific variant. See [[source-jason-shah]].

## Related sources

- [[source-ian-mcallister]] — Top-1%-PM episode; most nuanced B4 articulation.
- [[source-bill-carr]] — Co-author of the book *Working Backwards*.
- [[source-jason-shah]] — Writing-culture perspective from Amazon alum.

## Related concepts

- [[amazon]] — Home org.
- [[opportunity-solution-tree]] — Complementary discovery artifact.
- [[rituals-of-great-teams]] — PR/FAQ as one ritual among many.
