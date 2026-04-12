---
title: "Comparison: B2 AI Product Approaches"
type: comparison
created: 2026-04-12
updated: 2026-04-12
tags: [ai-products, comparison, b2]
sources: [lenny-podcast/sander-schulhoff.md, lenny-podcast/hilary-gridley.md, lenny-podcast/mike-krieger.md, lenny-podcast/krithika-shankarraman.md, lenny-podcast/aparna-chennapragada.md, lenny-podcast/nabeel-s-qureshi.md, lenny-podcast/kim-scott.md, lenny-podcast/scott-wu.md, lenny-podcast/michael-truell.md, lenny-podcast/varun-mohan.md, lenny-podcast/guillermo-rauch.md, lenny-podcast/kevin-weil.md, lenny-podcast/eric-simons.md, lenny-podcast/anton-osika.md, lenny-podcast/karina-nguyen.md, lenny-podcast/shaun-clowes.md, lenny-podcast/amjad-masad.md, lenny-podcast/tamar-yehoshua.md, lenny-podcast/eli-schwartz.md, lenny-podcast/cam-adams.md, lenny-podcast/claire-vo.md, lenny-podcast/jackie-bavaro.md, lenny-podcast/logan-kilpatrick.md, lenny-podcast/inbal-s.md, lenny-podcast/paul-adams.md, lenny-podcast/christopher-miller.md, lenny-podcast/noah-weiss.md, lenny-podcast/jiaona-zhang.md, lenny-podcast/gustav-s#U00f6derstr#U00f6m.md, lenny-podcast/scott-belsky.md, lenny-podcast/marily-nika.md, lenny-podcast/ryan-j-salva.md]
---

# Comparison: B2 AI Product Approaches

How 32 Lenny's Podcast guests approach AI products — grouped into 10 schools of thought. B2 spans 2022–2025 and covers the full arc from pre-ChatGPT experimentation to the AI coding tools explosion.

## 1. Human-in-the-loop code editors

**Thesis**: AI augments developers inside the IDE; the human stays in the driver's seat.

- [[source-michael-truell|Michael Truell]] ([[cursor]]) — "After code": programming evolves toward pseudocode; custom models for every interaction layer.
- [[source-varun-mohan|Varun Mohan]] ([[windsurf]]) — "Dehydrated organization": AI lets a lean team compete with giants. Enterprise-first via FedRAMP.
- [[source-inbal-s|Inbal Shani]] ([[github-copilot]]) — "Copilot is a copilot, not a pilot." 92% developer adoption, 55% speed gains.
- [[source-ryan-j-salva|Ryan J. Salva]] ([[github-copilot]]) — Copilot origin story: accidental discovery from mass-cloning repos. Latency and ethics as first-order constraints.

**Key differentiation**: Cursor bets on custom models; Windsurf bets on enterprise compliance; Copilot bets on distribution (100M+ GitHub users).

## 2. AI app builders (no-code creation)

**Thesis**: AI lets non-engineers build production apps. The addressable market expands from 20M developers to 100M+ builders.

- [[source-eric-simons|Eric Simons]] ([[bolt]]) — Claude Sonnet crossed the quality threshold → Bolt went from near-death to $40M ARR in 5 months.
- [[source-anton-osika|Anton Osika]] ([[lovable]]) — $10M ARR in 60 days with 15 people. AI reliability scaling laws determine product quality.
- [[source-guillermo-rauch|Guillermo Rauch]] ([[v0]]) — "100 million builders." Inverted Git commit; exposure hours develop taste.
- [[source-amjad-masad|Amjad Masad]] ([[replit]]) — "The last piece of software." Amjad's Law: every app that can exist will exist. Society of models architecture.

**Key differentiation**: Bolt/Lovable target zero-code users; v0 targets designers/PMs; Replit targets the full spectrum including existing developers.

## 3. Autonomous AI agents

**Thesis**: AI doesn't just assist — it independently writes, tests, and deploys code. Humans shift from bricklayer to architect.

- [[source-scott-wu|Scott Wu]] ([[devin]]) — Fully autonomous, Slack-native coding agent. [[jevons-paradox-software|Jevons Paradox]]: more AI → more software → more engineering demand.

**Key differentiation**: Only one B2 guest takes the fully autonomous position. This is the most controversial school — directly challenged by the human-in-the-loop editors.

## 4. Model providers (the supply side)

**Thesis**: Build the best models and let the ecosystem build products on top.

- [[source-kevin-weil|Kevin Weil]] ([[openai]]) — Every company will need fine-tuned model ensembles; evals are the core PM skill.
- [[source-karina-nguyen|Karina Nguyen]] ([[openai]]) — Canvas and Tasks built via synthetic data training. Creative thinking threshold in Opus 4.
- [[source-logan-kilpatrick|Logan Kilpatrick]] ([[openai]]) — Vertical AI apps are the opportunity; don't compete with the platform.
- [[source-mike-krieger|Mike Krieger]] ([[anthropic]]) — 90%+ of code is AI-written at Anthropic. The bottleneck migrates from engineering to decision-making.

**Key differentiation**: Kevin Weil emphasizes model maximalism (use everything); Mike Krieger emphasizes the organizational transformation that AI-written code forces.

## 5. Enterprise AI transformation

**Thesis**: The hard part isn't the model — it's integrating AI into existing enterprise workflows, data, and culture.

- [[source-aparna-chennapragada|Aparna Chennapragada]] ([[microsoft]]) — NLX (natural language experience) as the new UX. "Prompt sets are the new PRDs."
- [[source-paul-adams|Paul Adams]] ([[intercom]]) — Ripped up product strategy post-ChatGPT. Fin chatbot handles 50–70% of support volume.
- [[source-shaun-clowes|Shaun Clowes]] (Confluent) — Data is 90% of AI quality. SaaS incumbents are protected by business rules, not UI.
- [[source-tamar-yehoshua|Tamar Yehoshua]] ([[glean]]) — Design for LLM improvement, not around LLM limitations. Non-deterministic products require new PM skills.
- [[source-nabeel-s-qureshi|Nabeel S. Qureshi]] ([[palantir]]) — Forward-deployed engineers + LLMs collapse the cost of customer-embedded engineering 5–10×.

**Key differentiation**: Paul Adams and Shaun Clowes argue incumbents are defensible (moat = data + business rules); Aparna says incumbents must fundamentally redesign interfaces.

## 6. AI and growth/marketing

**Thesis**: AI changes not just products but how products are discovered and marketed.

- [[source-krithika-shankarraman|Krithika Shankarraman]] ([[openai]]) — Even ChatGPT needed marketing: the challenge shifted from awareness to "use case epiphany."
- [[source-eli-schwartz|Eli Schwartz]] — AI Overviews are swallowing top-of-funnel SEO. Product-led SEO survives; editorial SEO is at risk.
- [[source-christopher-miller|Christopher Miller]] (HubSpot) — ChatSpot and microapps as AI-native distribution channels alongside traditional PLG.

## 7. AI-era product craft and taste

**Thesis**: As AI commoditizes execution, taste and product sense become the primary differentiator.

- [[source-scott-belsky|Scott Belsky]] (Adobe) — "Golden gut" intuition + first mile experience. AI collapses the organizational stack.
- [[source-gustav-s#U00f6derstr#U00f6m|Gustav Söderström]] ([[spotify]]) — Curation → recommendation → generation framework. Fault-tolerant UIs for non-deterministic AI.
- [[source-cam-adams|Cameron Adams]] ([[canva]]) — 800 coaches replacing managers. Three-pillar AI strategy (build/partner/ecosystem).
- [[source-jiaona-zhang|Jiaona Zhang]] (Webflow) — [[minimum-lovable-product|Minimum lovable products]]; roadmap storytelling; Airbnb Plus post-mortem.

**Key differentiation**: Belsky focuses on individual intuition; Gustav focuses on UI paradigm shifts; Cam focuses on organizational culture.

## 8. AI for PM augmentation

**Thesis**: AI tools make individual PMs more effective — not by replacing them, but by compressing learning and extending capabilities.

- [[source-claire-vo|Claire Vo]] (ChatPRD) — Built a commercially successful AI PM tool. "One click faster" pace framework. CPTO role.
- [[source-marily-nika|Marily Nika]] (Meta) — Every PM becomes an AI PM. Practical AI product lifecycle. Warning against the "shiny object trap."
- [[source-hilary-gridley|Hilary Gridley]] (Whoop) — Custom GPTs for simulating feedback, practicing conversations, and accelerating learning.

## 9. Prompt engineering and security

**Thesis**: How to actually use LLMs effectively — and what breaks when you try.

- [[source-sander-schulhoff|Sander Schulhoff]] — [[prompt-engineering-techniques|5 techniques that work, 2 debunked]]. Prompt injection remains unsolvable.

## 10. Management and leadership in the AI era

**Thesis**: Human management skills become more critical, not less, as AI multiplies the surfaces leaders must navigate.

- [[source-kim-scott|Kim Scott]] — Radical Candor framework. Ruinous empathy is the most common failure mode.
- [[source-noah-weiss|Noah Weiss]] ([[slack]]) — Complaint Storms and Customer Love Sprints. "Successful teams" as activation metric.
- [[source-jackie-bavaro|Jackie Bavaro]] — Three pillars of strategy (vision, framework, roadmap). PEARL interview framework.

## Key disagreements at a glance

| Tension | Position A | Position B |
|---|---|---|
| Human-in-loop vs. autonomous | [[source-michael-truell\|Truell]], [[source-varun-mohan\|Mohan]]: Humans stay in driver's seat | [[source-scott-wu\|Wu]]: Fully autonomous agents are the future |
| Developers survive vs. transform | [[source-inbal-s\|Shani]]: AI augments, developers are irreplaceable | [[source-guillermo-rauch\|Rauch]]: Non-developers become the primary builders |
| Incumbents defensible vs. vulnerable | [[source-shaun-clowes\|Clowes]]: Data + business rules protect incumbents | [[source-paul-adams\|Adams]]: Must rip up strategy or die |
| Ship fast vs. ship carefully | [[source-eric-simons\|Simons]], [[source-anton-osika\|Osika]]: Daily shipping, speed is everything | [[source-noah-weiss\|Weiss]]: AI confidence must match actual capability |
| Taste can be learned vs. innate | [[source-guillermo-rauch\|Rauch]]: Exposure hours develop taste | [[source-scott-belsky\|Belsky]]: Golden gut is partly innate intuition |
| Evals vs. user research | [[source-kevin-weil\|Weil]]: Evals are the core PM skill | [[source-marily-nika\|Nika]]: Talk to users first, AI tools second |

## See also

- [[comparison-b1-ai-product-approaches]] — the B1 comparison (2025+ sources)
- [[synthesis-b2-ai-product-patterns]] — convergent patterns across B2
- [[ai-coding-tools]] — the biggest single theme in B2
- [[taste-as-differentiator]] — the cross-cutting concept
