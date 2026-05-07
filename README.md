# Miz Causevic — `// kineticgain`

```
[ Director of Web Engineering & Platform Architecture ]
[ Boston, MA · 30 yrs of platform & web engineering ]
[ IBM · CyberArk · Alteryx · Digital.ai · Gryphon.ai ]
```

I build **AI Platform Engineering** infrastructure — the layer that sits between agents/models and the SRE, SecOps, and platform teams who have to keep them running in production.

---

## The Doctrine

Most enterprises ship AI features by stitching together notebooks, vendor consoles, and Slack channels. That works at demo scale. It does not work when you have 8 MCP servers, 12 agent fleets, 6 RAG collections, three model providers, and a CISO asking "are we OK right now?"

This portfolio is a **deliberate platform**, not a pile of side projects. Six repos. Six layers. One doctrine: **every surface in the AI stack needs the same governance discipline that database, network, and identity surfaces already have.**

---

## The Six Repos

| # | Repo | Surface | Question it answers | CI |
|---|---|---|---|---|
| 1 | [`mcp-sentinel`](https://github.com/mizcausevic-dev/mcp-sentinel) | Tool calls | What MCP tools are exposed and how risky? | ![CI](https://github.com/mizcausevic-dev/mcp-sentinel/actions/workflows/ci.yml/badge.svg) |
| 2 | [`rag-sentinel`](https://github.com/mizcausevic-dev/rag-sentinel) | Retrieval | What's in the vector store and how trustworthy? | ![CI](https://github.com/mizcausevic-dev/rag-sentinel/actions/workflows/ci.yml/badge.svg) |
| 3 | [`agent-codex`](https://github.com/mizcausevic-dev/agent-codex) | Decisions | Under what policies are decisions allowed? | ![CI](https://github.com/mizcausevic-dev/agent-codex/actions/workflows/ci.yml/badge.svg) |
| 4 | [`agent-eval-arena`](https://github.com/mizcausevic-dev/agent-eval-arena) | Pre-prod | Should this model promotion ship? | ![CI](https://github.com/mizcausevic-dev/agent-eval-arena/actions/workflows/ci.yml/badge.svg) |
| 5 | [`agentobserve`](https://github.com/mizcausevic-dev/agentobserve) | Runtime | What did agents actually do? | ![CI](https://github.com/mizcausevic-dev/agentobserve/actions/workflows/ci.yml/badge.svg) |
| 6 | [`kinetic-flightdeck`](https://github.com/mizcausevic-dev/kinetic-flightdeck) | Operator | Are we OK right now? Who do I call? | ![CI](https://github.com/mizcausevic-dev/kinetic-flightdeck/actions/workflows/ci.yml/badge.svg) |

---

## Architectural View

```
                     +-------------------------------------------------+
                     |           kinetic-flightdeck                    |
                     |   (operator surface - single pane of glass)     |
                     +-------------------------------------------------+
                                          ^
                +-------------------------+--------------------------+
                |                         |                          |
                v                         v                          v
   +------------------+    +------------------+         +-------------------+
   |   GOVERNANCE     |    |   PRE-PROD       |         |   RUNTIME         |
   |                  |    |                  |         |                   |
   | mcp-sentinel     |    | agent-eval-arena |         | agentobserve      |
   | rag-sentinel     |    | (gates, reg)     |         | (runs, traces,    |
   | agent-codex      |    |                  |         |  cost, SLA)       |
   +------------------+    +------------------+         +-------------------+
                                          |
                                          v
                     +-------------------------------------------------+
                     |         AGENTS - LLMs - MCP SERVERS             |
                     +-------------------------------------------------+
```

---

## Common Patterns Across All Six

Every repo in this portfolio follows the same engineering discipline:

| Pattern | Why |
|---|---|
| **TypeScript strict mode + Node.js 20+** | Type safety + LTS runtime; same as enterprise platform teams |
| **Express 5 + Zod schema validation** | Versioned, validated, swagger-able APIs |
| **Composite scoring with override logic** | A 90 composite + one critical signal still blocks. "Platform thinking." |
| **Heuristic-first analysis, LLM-judges optional** | Deterministic, testable, cheap - no judge LLM in the hot path |
| **CI on Node 20 + 22 matrix** | Forward-compatibility before LTS deprecation |
| **Local validation before push (the doctrine)** | Sandbox build, npm test green, push only when green. Zero broken pushes since adopted. |
| **BERT dark theme + JetBrains Mono / Space Grotesk** | Operator dashboards that do not look like SaaS demos |
| **Composite + per-signal + recommended-action output shape** | What an SRE pager-rotation actually needs to read at 3am |

---

## What This Portfolio Demonstrates

For platform-engineering / director-level hiring managers:

- **Range across the AI stack** - tool surface, retrieval surface, decision surface, eval surface, runtime surface, operator surface. Six perspectives, one doctrine.
- **Production-minded backend design** - strict TypeScript, schema validation, full test coverage, CI matrix, dashboards as deliverables.
- **Enterprise-ready domain modeling** - auth posture, OAuth scopes, SOC 2 / EU AI Act mapping, PII patterns, compliance frameworks, accountability rollups.
- **Refusal of demo-quality engineering** - none of these projects has placeholder logic. Every aggregator is testable, every override rule is justified, every composite score has weights chosen for a reason.
- **Platform-thinking doctrine** - no project ships without a governance loop, an operator output, and override logic that respects single-signal escalation. The same discipline applied across six different problem domains.

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
