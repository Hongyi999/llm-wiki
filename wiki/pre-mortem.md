---
title: Pre-mortem
type: concept
created: 2026-04-13
updated: 2026-04-13
tags: [shreyas-doshi, pre-mortem, decision-hygiene, risk-management]
sources: [lenny-podcast/shreyas-doshi.md]
---

# Pre-mortem

A **pre-mortem** is a decision-hygiene ritual — popularized for PMs by [[source-shreyas-doshi|Shreyas Doshi]] — where the team imagines a future failure *before* starting work and reverse-engineers the causes. It's the mirror of a postmortem: same question ("why did this fail?"), but asked while risks are still mitigable.

## The mechanic

1. **Set the scene**: "It's six months from now. This launch has failed. What happened?"
2. **Silent individual brainstorm** (5–10 min): Each attendee writes failure stories.
3. **Round-robin share**: Each person reads one. Repeat until exhausted.
4. **Cluster and rank**: Group similar failures. Rank by plausibility × impact.
5. **Owner and mitigation**: Top risks get a named owner and a mitigation plan.

## Why it works

- **Imagination beats analysis** for surfacing risks. "List all risks" produces optimistic lists. "Imagine the failure" produces honest ones.
- **Permission to be negative**: Pre-mortems legalize pessimism in a room where dissent is usually costly.
- **Loss aversion activation**: Humans are better at avoiding losses than capturing gains; pre-mortems harness that asymmetry.

## When to run a pre-mortem

- **Before major bets** — Product launches, strategy shifts, large hires, org redesigns.
- **Before irreversible decisions** — One-way doors in Bezos's framing.
- **When the team is too aligned** — Uncritical consensus is a signal that risks are hidden, not absent.

## Postmortem vs pre-mortem

| Postmortem | Pre-mortem |
|---|---|
| After failure | Before launch |
| Forensic | Predictive |
| Fixes next time | Fixes this time |
| Backward-looking | Forward-looking |

Both are valuable; pre-mortems are underused because they require admitting doubt before success is visible.

## Common failure modes

- **Cheap ceremony** — Running the ritual without actually changing plans based on what it surfaces.
- **Political filtering** — Attendees self-censor to avoid calling out the boss's favored bet.
- **No owners** — Risks surfaced without owners become ambient worry, not mitigation.
- **Single-pass** — Pre-mortem once at project start, never revisit. Better: pre-mortem at each major stage gate.

## Related sources

- [[source-shreyas-doshi]] — Primary B4 articulation.
- [[source-annie-duke]] — *Thinking in Bets* intellectual predecessor.

## Related concepts

- [[lno-framework]] — Pre-mortems are L-tasks (high leverage) that often get classified as O.
- [[working-backwards]] — PR/FAQ is a complementary decision-hygiene mechanism.
- [[rituals-of-great-teams]] — Pre-mortems can be institutionalized as a ritual.
