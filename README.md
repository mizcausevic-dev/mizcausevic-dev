# Miz Causevic — `// kineticgain`

```
[ Director of Web Engineering & Platform Architecture ]
[ Boston, MA · 30 yrs of platform & web engineering ]
[ IBM · CyberArk · Alteryx · Digital.ai · Gryphon.ai ]
```

I build **AI Platform Engineering** infrastructure — the layer that sits between agents/models and the SRE, SecOps, FinOps, and platform teams who have to keep them running in production.

---

## The Doctrine

Most enterprises ship AI features by stitching together notebooks, vendor consoles, and Slack channels. That works at demo scale. It does not work when you have 8 MCP servers, 12 agent fleets, 6 RAG collections, three model providers, a $50K monthly LLM bill, a CISO asking "are we OK right now," and a CFO asking "are we on budget."

This portfolio is a **deliberate platform**, not a pile of side projects. Nine repos. Nine surfaces. One doctrine: **every layer of the AI stack needs the same governance discipline that database, network, and identity surfaces already have.**

---

## The Nine Repos

| # | Repo | Surface | Question it answers | CI |
|---|---|---|---|---|
| 1 | [`mcp-sentinel`](https://github.com/mizcausevic-dev/mcp-sentinel) | Tool calls | What MCP tools are exposed and how risky? | ![CI](https://github.com/mizcausevic-dev/mcp-sentinel/actions/workflows/ci.yml/badge.svg) |
| 2 | [`rag-sentinel`](https://github.com/mizcausevic-dev/rag-sentinel) | Retrieval | What is in the vector store and how trustworthy? | ![CI](https://github.com/mizcausevic-dev/rag-sentinel/actions/workflows/ci.yml/badge.svg) |
| 3 | [`agent-codex`](https://github.com/mizcausevic-dev/agent-codex) | Decisions | Under what policies are decisions allowed? | ![CI](https://github.com/mizcausevic-dev/agent-codex/actions/workflows/ci.yml/badge.svg) |
| 4 | [`agent-eval-arena`](https://github.com/mizcausevic-dev/agent-eval-arena) | Pre-prod | Should this model promotion ship? | ![CI](https://github.com/mizcausevic-dev/agent-eval-arena/actions/workflows/ci.yml/badge.svg) |
| 5 | [`agent-router`](https://github.com/mizcausevic-dev/agent-router) | Runtime routing | Which model does this request actually hit? | ![CI](https://github.com/mizcausevic-dev/agent-router/actions/workflows/ci.yml/badge.svg) |
| 6 | [`agentobserve`](https://github.com/mizcausevic-dev/agentobserve) | Runtime telemetry | What did agents actually do? | ![CI](https://github.com/mizcausevic-dev/agentobserve/actions/workflows/ci.yml/badge.svg) |
| 7 | [`shadow-ai-detector`](https://github.com/mizcausevic-dev/shadow-ai-detector) | Egress | Who is leaking what to whom? | ![CI](https://github.com/mizcausevic-dev/shadow-ai-detector/actions/workflows/ci.yml/badge.svg) |
| 8 | [`ai-finops-radar`](https://github.com/mizcausevic-dev/ai-finops-radar) | Finance | Are we on budget — and why not? | ![CI](https://github.com/mizcausevic-dev/ai-finops-radar/actions/workflows/ci.yml/badge.svg) |
| 9 | [`kinetic-flightdeck`](https://github.com/mizcausevic-dev/kinetic-flightdeck) | Operator | Are we OK right now? Who do I call? | ![CI](https://github.com/mizcausevic-dev/kinetic-flightdeck/actions/workflows/ci.yml/badge.svg) |

---

## Architectural View

```
                       +-------------------------------------------------+
                       |             kinetic-flightdeck                  |
                       |    (operator surface - single pane of glass)    |
                       +-------------------------------------------------+
                                            ^
        +---------------+--------------+----+----+----------------+----------------+
        |               |              |         |                |                |
        v               v              v         v                v                v
+--------------+ +--------------+ +--------+ +--------+ +-------------+ +-----------------+
| GOVERNANCE    | | PRE-PROD    | |RUNTIME | |EGRESS  | | FINANCE     | | RUNTIME OBS     |
|               | |             | |        | |        | |             | |                 |
| mcp-sentinel  | | agent-eval- | | agent- | | shadow-| | ai-finops-  | | agentobserve    |
| rag-sentinel  | | arena       | | router | | ai-    | | radar       | | (runs, traces,  |
| agent-codex   | | (gates,     | | (live  | | detect | | (cost,      | |  cost, SLA)     |
|               | |  reg)       | | route) | | egress)| |  forecast)  | |                 |
+--------------+  +--------------+ +--------+ +--------+ +-------------+ +-----------------+
                                          |
                                          v
                       +-------------------------------------------------+
                       |          AGENTS - LLMs - MCP SERVERS            |
                       +-------------------------------------------------+
```

---

## Common Patterns Across All Nine

Every repo in this portfolio follows the same engineering discipline:

| Pattern | Why |
|---|---|
| **TypeScript strict mode + Node.js 20+** | Type safety + LTS runtime; same as enterprise platform teams |
| **Express 5 + Zod schema validation** | Versioned, validated, swagger-able APIs |
| **Composite scoring with override logic** | A 90 composite + one critical signal still blocks. "Platform thinking." |
| **Heuristic-first analysis, LLM-judges optional** | Deterministic, testable, cheap - no judge LLM in the hot path |
| **CI on Node 20 + 22 matrix** | Forward-compatibility before LTS deprecation |
| **Local validation before push** | Sandbox build, npm test green, push only when green. Zero broken pushes since adopted. |
| **BERT dark theme + JetBrains Mono / Space Grotesk** | Operator dashboards that do not look like SaaS demos |
| **Composite + per-signal + recommended-action output shape** | What an SRE pager-rotation actually needs to read at 3am |

---

## What This Portfolio Demonstrates

For platform-engineering / director-level hiring managers:

- **Range across the AI stack** - tool calls, retrieval, decisions, eval, routing, runtime observability, egress, finance, operator surface. **Nine perspectives, one doctrine.**
- **Three buyer profiles** - CTO/Platform (mcp-sentinel, agent-codex, agent-router, agentobserve, kinetic-flightdeck), CISO (shadow-ai-detector, mcp-sentinel), CFO (ai-finops-radar). One coherent platform thesis.
- **Production-minded backend design** - strict TypeScript, schema validation, full test coverage, CI matrix, dashboards as deliverables.
- **Enterprise-ready domain modeling** - auth posture, OAuth scopes, SOC 2 / EU AI Act mapping, PII patterns, compliance frameworks, accountability rollups, anomaly detection, forecasting with confidence intervals.
- **Refusal of demo-quality engineering** - none of these projects has placeholder logic. Every aggregator is testable, every override rule is justified, every composite score has weights chosen for a reason. Circuit breakers have correct half-open semantics.
- **Platform-thinking doctrine** - no project ships without a governance loop, an operator output, and override logic that respects single-signal escalation. The same discipline applied across nine different problem domains.

---

## Selected Background

| | |
|---|---|
| **IBM** | Web engineering & platform architecture |
| **CyberArk** | Cybersecurity platform; identity & access |
| **Alteryx** | Web platform optimization; documented **1,712x network performance improvement** as flagship technical proof point |
| **Digital.ai** | Application security & DevOps |
| **Gryphon.ai** | Conversational AI platform engineering |

30 years of platform & web engineering · Sarajevo roots · Boston-based · ~30 hardware synthesizers and a music project running since 1999 (because the work does not stop at 5pm).

---

## Connect

- [LinkedIn](https://www.linkedin.com/in/mizcausevic/)
- [Skills Page](https://mizcausevic.com/skills)
- [Medium](https://medium.com/@mizcausevic)
- [Email](mailto:miz@kineticgain.dev)

```
"The pessimist complains about the wind. The optimist expects it to change.
 The realist adjusts the sails."
                                                    -- William Arthur Ward
```
