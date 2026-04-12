---
title: Taste as Differentiator
type: concept
created: 2026-04-12
updated: 2026-04-12
tags: [taste, product-sense, craft, ai-era-skills, design, judgment]
sources: [lenny-podcast/michael-truell.md, lenny-podcast/guillermo-rauch.md, lenny-podcast/scott-belsky.md, lenny-podcast/kevin-weil.md, lenny-podcast/krithika-shankarraman.md, lenny-podcast/karina-nguyen.md]
---

# Taste as Differentiator

As AI rapidly commoditizes the *execution* of building software -- writing code, generating designs, producing content -- "taste" emerges as the critical human bottleneck: the ability to discern what is good, what should be built, and how it should feel. Across six B2 sources (and echoing B1's [[figma|Figma]]/[[source-dylan-field|Dylan Field]] "craft-is-moat" thesis), guests converge on the claim that taste -- encompassing product judgment, aesthetic sensibility, and the intuition for what users actually need -- is the skill that compounds in value as AI makes implementation nearly free. The word "taste" appears in nearly every AI coding interview in B2, making it the meta-skill of the entire batch.

## Core thesis: taste as the new bottleneck

[[source-michael-truell|Michael Truell]] articulates the thesis most directly: as AI reduces the "translation labor" of turning ideas into working software, the dominant differentiator becomes *having the right idea* for what should be built and how it should work. This applies to both visual design and the underlying logic of software. In a world where anyone can build anything, the person who knows *what is worth building* becomes the most valuable contributor.

This echoes [[source-anton-osika|Anton Osika]]'s framing from the [[ai-coding-tools]] interviews: the bottleneck has "permanently shifted from engineering capacity to product taste and user understanding."

## How taste develops

The sources offer three distinct models for how taste is cultivated:

### 1. Exposure hours (Rauch)

[[source-guillermo-rauch|Guillermo Rauch]] rejects taste as an innate gift. He frames it as a trainable skill developed through quantifiable "exposure hours" -- time spent watching how people use products, trying many products yourself, and showing your work to others for feedback. At Vercel, this is an explicit internal operating principle: teams are expected to log time observing real users. The mechanism is pattern recognition -- you develop intuition by accumulating a large library of product experiences to draw from.

### 2. Golden gut (Belsky)

[[source-scott-belsky|Scott Belsky]] introduces the "golden gut" -- an experienced product intuition for the thousands of micro-decisions in design. When should a presumptuous default beat an explicit choice? When should you trade 10% confusion for 90% speed? The golden gut develops not through abstract theory but through empathy and shoulder-to-shoulder customer observation. Belsky emphasizes that this intuition is specifically about the "**first mile experience**" -- the first 30 seconds where users are "lazy, vain, and selfish."

### 3. Creative threshold (Nguyen)

[[source-karina-nguyen|Karina Nguyen]] approaches taste from the AI research side. She argues that it is "really, really hard to teach the model how to be aesthetic or really good visual design or how to be extremely creative." This suggests taste sits above a capability threshold that current models cannot reliably cross -- making it one of the few human skills that remains genuinely scarce even as models master coding, writing, and analysis.

## Contrasting views

| Guest | Role / Company | Definition of taste | How it develops | Why it matters now |
|---|---|---|---|---|
| [[source-michael-truell\|Michael Truell]] | CEO, [[cursor\|Cursor]] | Having the right idea for what should be built -- both visual design and software logic | Practice: iterative prototyping and dogfooding | AI eliminates translation labor; taste is all that remains |
| [[source-guillermo-rauch\|Guillermo Rauch]] | CEO, Vercel/[[v0\|v0]] | Pattern recognition for what makes products great | Quantified "exposure hours" watching users, trying products, showing work | 100M builders need taste to stand out; tools are democratized |
| [[source-scott-belsky\|Scott Belsky]] | CSO, Adobe | Micro-decision intuition ("golden gut") for product craft | Empathy, shoulder-to-shoulder observation, radical reductionism | AI "collapses the stack" -- individuals do more, taste guides what |
| [[source-kevin-weil\|Kevin Weil]] | CPO, [[openai\|OpenAI]] | Judgment about which capabilities to ship and how | Human reasoning as design heuristic; thinking about what a human would do | Models improve every 2 months; product vision outpaces model capability |
| [[source-krithika-shankarraman\|Krithika Shankarraman]] | First marketer, [[openai\|OpenAI]] & Stripe | Craft and authenticity that differentiates in a sea of AI-generated content | Deep product understanding, customer connection, the DATE diagnostic | AI floods the market with content; being "cheaper" is a race to the bottom |
| [[source-karina-nguyen\|Karina Nguyen]] | Researcher, [[openai\|OpenAI]] | Aesthetic judgment and creative originality that models cannot reliably produce | Unclear -- may be the hardest skill to systematize | Models master hard skills; creativity and aesthetic judgment are the remaining human edge |

## Why taste matters more now than before

The sources converge on a causal chain:

1. **AI makes execution cheap.** Code that took days now takes minutes ([[source-amjad-masad|Masad]]: full-stack app in 10 minutes for 15 cents). Content that required specialists is now generated by anyone with a prompt.

2. **Supply explodes.** More software, more content, more products flood every market. Rauch predicts 100 million builders; Masad invokes [[jevons-paradox-software|Jevons Paradox]].

3. **Differentiation shifts upstream.** When everyone can build, the scarce resource is knowing *what to build and how it should feel*. Shankarraman frames this as: being cheaper is a race to the bottom; being different and tasteful is durable.

4. **Taste compounds.** Unlike technical skills that depreciate as models improve, taste compounds with experience. Rauch's "exposure hours" model suggests taste gets better the more products you observe and ship. Belsky's "golden gut" sharpens with every customer observation.

The implication for product teams is stark: hiring for taste, design sensibility, and user empathy may matter more than hiring for raw engineering ability -- a reversal of decades of tech industry orthodoxy.

## Relationship to adjacent concepts

Taste intersects with several related ideas in the wiki:

- **[[product-market-fit]]**: Taste helps you identify *what* to build; PMF confirms you were right. The [[superhuman-pmf-engine]] explicitly involves taste-driven iteration on the "main benefit."
- **[[ai-coding-tools]]**: Every AI coding guest identifies taste as the skill that remains after AI handles implementation.
- **[[ai-evals]]**: Weil argues that writing evals is itself an exercise in taste -- knowing what "good" looks like for a model's output is a judgment call, not a mechanical one.
- **First mile experience**: Belsky's "golden gut" is most critical in the first 30 seconds of a product experience, where micro-decisions about defaults, copy, and flow determine whether users stay or leave.

## See also

- [[ai-coding-tools]] -- the category where taste becomes the bottleneck
- [[prompt-engineering-techniques]] -- communicating taste to AI systems effectively
- [[product-market-fit]] -- taste helps find it; PMF confirms it
- **first mile experience** -- where taste has the highest leverage
- [[cursor]] / [[v0]] / [[lovable]] -- products whose founders explicitly center taste
- [[figma]] -- Dylan Field's B1 thesis that craft is the moat
