---
title: AI Agents
type: concept
created: 2026-04-11
updated: 2026-04-11
tags: [ai-agents, ai-products, enterprise-ai, autonomous-ai]
sources: [lenny-podcast/bret-taylor.md, lenny-podcast/eoghan-mccabe.md, lenny-podcast/nick-turley.md, lenny-podcast/asha-sharma.md, lenny-podcast/jason-droege.md, lenny-podcast/sander-schulhoff-20.md, lenny-podcast/dhanji-r-prasanna.md]
---

# AI Agents

Software systems that take autonomous actions on a user's behalf — as opposed to chat interfaces that only produce text. In B1, agents are the emerging *primary* form factor for AI products, with consensus across 7+ guests that the shift is inevitable but dangerous.

## Core claims in B1

### Agents as the new app (Bret Taylor, Sierra AI)

[[source-bret-taylor|Bret Taylor]] ([[sierra-ai|Sierra AI]]) argues every SaaS category will be re-built around an agent that does the job, not a tool that helps humans do the job. This reframes pricing ([[outcomes-based-pricing|per outcome, not per seat]]) and GTM (sell to line-of-business, not IT). See [[sierra-ai]].

### Agentic society (Asha Sharma, Microsoft AI)

[[source-asha-sharma|Asha Sharma]] frames the shift as an **org-chart redesign**: agents become teammates with their own "roles," managers orchestrate mixed human-agent teams, and [[ai-native-organization|composable building blocks replace monolithic apps]].

### ChatGPT is heading to agents with oversight (Nick Turley)

[[source-nick-turley|Nick Turley]]'s roadmap for [[chatgpt|ChatGPT]] puts agentic workflows at the center, **always with a human checkpoint**. He emphasizes "agents and human oversight" as a design constraint, not a transitional phase.

### Customer service is the first full-stack agent deployment (Eoghan McCabe, Intercom)

[[source-eoghan-mccabe|Eoghan McCabe]] bet [[source-eoghan-mccabe|Intercom]]'s survival on **Fin**, an AI customer support agent, and reset 40% of the workforce to reorganize around agents. He frames it as "AI bet or death" for legacy SaaS.

### Enterprise agents need domain-specific evals (Jason Droege)

[[source-jason-droege]] stresses that agents in enterprise settings fail because generic evals miss domain-specific failure modes. The data-labeling market is pivoting toward supplying **agent behavior evaluations**, not just static Q&A labels.

### Agents productivity at Block (Dhanji Prasanna)

At [[block|Block]], Goose (internal agent) saves engineers 8–10 hours/week and is generating pull requests from Slack discussions. See [[source-dhanji-r-prasanna]].

## Security warning

[[source-sander-schulhoff-20|Sander Schulhoff]] warns that agentic systems dramatically **scale the blast radius** of prompt injection and jailbreaks. An agent with tool use can read, write, send, and transact — adversaries can weaponize a single successful injection into real-world damage. Guardrails fail; evals fail; the problem is fundamentally unsolved.

## Cross-source patterns

- **Outcomes-based pricing follows agents** — if the agent does the job, charge for the job done. See [[outcomes-based-pricing]].
- **Human-in-the-loop is universal** — every B1 guest building agents insists on a human checkpoint somewhere.
- **Disruption is violent** — Eoghan McCabe: the shift is not gradual; incumbents either bet fully or die.
- **Evals are the bottleneck** — agents need behavioral evals, not just accuracy benchmarks. See [[ai-evals]].

## See also

- [[outcomes-based-pricing]] — the pricing model agents unlock.
- [[sierra-ai]], [[chatgpt]] — canonical B1 agent products.
- [[ai-evals]] — the bottleneck for safe deployment.
- [[ai-native-organization]] — org-design implications.
