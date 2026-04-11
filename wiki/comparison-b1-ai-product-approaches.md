---
title: "Comparison: B1 AI Product Approaches"
type: comparison
created: 2026-04-11
updated: 2026-04-11
tags: [ai-products, comparison, b1]
sources: [lenny-podcast/aishwarya-naresh-reganti-kiriti-badam.md, lenny-podcast/asha-sharma.md, lenny-podcast/brandon-chu.md, lenny-podcast/brendan-foody.md, lenny-podcast/bret-taylor.md, lenny-podcast/brian-balfour.md, lenny-podcast/chip-huyen.md, lenny-podcast/dan-shipper.md, lenny-podcast/dhanji-r-prasanna.md, lenny-podcast/dr-fei-fei-li.md, lenny-podcast/dylan-field.md, lenny-podcast/edwin-chen.md, lenny-podcast/elena-verna-40.md, lenny-podcast/eoghan-mccabe.md, lenny-podcast/ethan-smith.md, lenny-podcast/garrett-lord.md, lenny-podcast/grant-lee.md, lenny-podcast/hamel-husain-shreya-shankar.md, lenny-podcast/howie-liu.md, lenny-podcast/jason-droege.md, lenny-podcast/jason-m-lemkin.md, lenny-podcast/julian-shapiro.md, lenny-podcast/julie-zhuo.md, lenny-podcast/madhavan-ramanujam.md, lenny-podcast/nick-turley.md, lenny-podcast/nicole-forsgren.md, lenny-podcast/robby-stein.md, lenny-podcast/sander-schulhoff-20.md, lenny-podcast/tomer-cohen.md]
---

# Comparison: B1 AI Product Approaches

Side-by-side mapping of how the 29 guests in [[index-by-theme|B1 (AI products 2025+)]] think about building AI products. Guests are grouped by their primary angle, with disagreements flagged explicitly.

## Grouping by angle

### 1. The evals-first school

| Guest | Company | Core claim |
|---|---|---|
| [[source-hamel-husain-shreya-shankar\|Hamel Husain & Shreya Shankar]] | Parlance Labs / Berkeley | Evals are the new PRD; error analysis → axial coding → LLM-as-judge |
| [[source-brendan-foody\|Brendan Foody]] | [[mercor\|Mercor]] | Evals are the product bottleneck; frontier labs pay PhDs to write them |
| [[source-chip-huyen\|Chip Huyen]] | NVIDIA NeMo | Evals are necessary but not sufficient — users > evals |
| [[source-edwin-chen\|Edwin Chen]] | Surge AI | Evals teach values; different labs produce different model personalities |

**Convergence**: evals are the core AI engineering skill. **Disagreement**: whether evals *drive* the process (Hamel) or *follow* user research (Chip). See [[ai-evals]].

### 2. The agents-as-new-app school

| Guest | Company | Core claim |
|---|---|---|
| [[source-bret-taylor\|Bret Taylor]] | [[sierra-ai\|Sierra AI]] | Every SaaS category will be re-built around agents, priced per outcome |
| [[source-eoghan-mccabe\|Eoghan McCabe]] | Intercom | Fin agent + 40% workforce reset = survival bet |
| [[source-asha-sharma\|Asha Sharma]] | [[meta\|Microsoft AI]] | Agentic society reshapes the org chart |
| [[source-nick-turley\|Nick Turley]] | [[chatgpt\|ChatGPT]]/[[openai\|OpenAI]] | Agents with human oversight, always |

**Convergence**: agents replace apps, not features. **Disagreement**: how much autonomy ([[source-bret-taylor\|Bret]]: a lot; [[source-nick-turley\|Nick]]: always with a human checkpoint). See [[ai-agents]].

### 3. The AI-native organization school

| Guest | Company | Core claim |
|---|---|---|
| [[source-tomer-cohen\|Tomer Cohen]] | [[linkedin\|LinkedIn]] | AI-first product development since 2016; Full Stack Builder program |
| [[source-dhanji-r-prasanna\|Dhanji R. Prasanna]] | [[block\|Block]] | Functional org + internal Goose agent; Conway's Law applied |
| [[source-julie-zhuo\|Julie Zhuo]] | ex-Facebook | Management as AI orchestration; builders not roles |
| [[source-dan-shipper\|Dan Shipper]] | Every | 15-person team, 5 products, Head of AI Ops role |
| [[source-howie-liu\|Howie Liu]] | Airtable | IC CEO + fast/slow team split |
| [[source-eoghan-mccabe\|Eoghan McCabe]] | Intercom | Founder-mode decisiveness; AI bet or death |

**Convergence**: top-down restructuring required; grassroots alone fails. **Disagreement**: how violent the disruption must be ([[source-eoghan-mccabe\|Eoghan]]: total; [[source-tomer-cohen\|Tomer]]: gradual re-orientation possible at LinkedIn scale). See [[ai-native-organization]].

### 4. The post-training data school

| Guest | Company | Core claim |
|---|---|---|
| [[source-brendan-foody\|Brendan Foody]] | [[mercor\|Mercor]] | PhDs are the new labelers; $1M → $500M in 17 months |
| [[source-garrett-lord\|Garrett Lord]] | Handshake | 18M-student network as audience moat |
| [[source-jason-droege\|Jason Droege]] | ex-Scale AI / Handshake | Domain-specific evals; agentic environments |
| [[source-edwin-chen\|Edwin Chen]] | Surge AI | Data teaches values; bootstrapped research |
| [[source-chip-huyen\|Chip Huyen]] | NVIDIA NeMo | Pre-training saturated; post-training is the frontier |
| [[source-asha-sharma\|Asha Sharma]] | Microsoft AI | Post-training economics reshape supplier relationships |

**Convergence**: expert human data is the new moat. **Disagreement**: whether synthetic data will eventually catch up. See [[post-training-data-moat]].

### 5. The product-velocity school

| Guest | Company | Core claim |
|---|---|---|
| [[source-nick-turley\|Nick Turley]] | [[chatgpt\|ChatGPT]] | Empirical discovery > strategy; vibe over benchmarks |
| [[source-dan-shipper\|Dan Shipper]] | Every | Founder experiment comfort = success predictor |
| [[source-grant-lee\|Grant Lee]] | [[gamma\|Gamma]] | Four months rebuilding onboarding = $100M ARR |
| [[source-elena-verna-40\|Elena Verna]] | Indie growth | PMF is a 3-month treadmill; 95% innovation |
| [[source-robby-stein\|Robby Stein]] | [[google\|Google]] | Relentless improvement culture |
| [[source-brian-balfour\|Brian Balfour]] | Reforge | Platform cycle theory; cycle compression |
| [[source-howie-liu\|Howie Liu]] | Airtable | Timely over ritual meetings |

**Convergence**: daily shipping is non-negotiable; AI both enables and demands it. **Disagreement**: whether this velocity scales past ~50 engineers. See [[product-velocity-ai-era]].

### 6. The AI pricing school

| Guest | Company | Core claim |
|---|---|---|
| [[source-bret-taylor\|Bret Taylor]] | Sierra | Outcomes-based pricing is the only way to capture AI value |
| [[source-madhavan-ramanujam\|Madhavan Ramanujam]] | Simon-Kucher | 2×2 framework; most AI startups undermonetize day one |
| [[source-elena-verna-40\|Elena Verna]] | Indie | Aggressive free-tier giveaways while market forms |

**Convergence**: per-seat pricing is structurally wrong for AI. **Disagreement**: timing — charge outcomes now (Bret) or give away free first (Elena). See [[outcomes-based-pricing]].

### 7. The AI security school

| Guest | Company | Core claim |
|---|---|---|
| [[source-sander-schulhoff-20\|Sander Schulhoff]] | LearnPrompting | Guardrails fail; prompt injection is unsolved; agents scale blast radius |

**Note**: Sander is the only B1 guest focused on security. All the other agent-enthusiasts should probably read his episode.

### 8. The research / frontier school

| Guest | Company | Core claim |
|---|---|---|
| [[source-dr-fei-fei-li\|Dr. Fei-Fei Li]] | [[world-labs\|World Labs]] | Language is not enough; spatial intelligence is next |
| [[source-chip-huyen\|Chip Huyen]] | NVIDIA NeMo | Practical AI engineering; post-training asymmetry |
| [[source-edwin-chen\|Edwin Chen]] | Surge AI | Bootstrapped research enables deeper work |

### 9. The growth & distribution school

| Guest | Company | Core claim |
|---|---|---|
| [[source-grant-lee\|Grant Lee]] | Gamma | Word-of-mouth > ads; viral onboarding |
| [[source-ethan-smith\|Ethan Smith]] | Graphite | AEO: get cited across tiers (Reddit, YouTube, blogs) |
| [[source-julian-shapiro\|Julian Shapiro]] | Demand Curve | PLA: product-led acquisition via building state |
| [[source-elena-verna-40\|Elena Verna]] | Indie growth | PMF treadmill; building in public |
| [[source-brian-balfour\|Brian Balfour]] | Reforge | Platform cycle + context/memory moat |
| [[source-jason-m-lemkin\|Jason Lemkin]] | SaaStr | Don't ideologically reject sales; hire 2, not 1 |

### 10. The design & craft school

| Guest | Company | Core claim |
|---|---|---|
| [[source-dylan-field\|Dylan Field]] | [[figma\|Figma]] | Taste and craft become the moat when AI commoditizes features |
| [[source-nicole-forsgren\|Nicole Forsgren]] | DX | [[developer-experience\|DevEx]] metrics shift in the AI era |
| [[source-brandon-chu\|Brandon Chu]] | ex-Shopify | Writing as strategic leverage; trust battery |

## Key disagreements at a glance

- **Evals-first (Hamel) vs. users-first (Chip)** — order of operations in AI product development.
- **Agents with full autonomy (Bret) vs. always human-in-loop (Nick)** — how much control to give agents.
- **Violent disruption (Eoghan) vs. gradual re-orientation (Tomer)** — pace of org change.
- **Outcomes pricing now (Bret/Madhavan) vs. free tier first (Elena)** — monetization timing.
- **Ship daily (most guests) vs. Sander's warning** — velocity vs. security.

## See also

- [[synthesis-b1-ai-product-patterns]] — what cuts across these schools.
- [[index-by-theme]] — the full B1 ordered list.
- [[ai-evals]], [[ai-agents]], [[ai-native-organization]], [[post-training-data-moat]], [[product-velocity-ai-era]], [[outcomes-based-pricing]] — the underlying concept pages.
