# Miz Causevic

> **Director of Web Engineering Â· Platform Architecture Â· B2B SaaS Technologist**
> Boston, MA Â· ~30 years across IBM, CyberArk, Alteryx, Digital.ai, Gryphon.ai

I ship platform infrastructure for production AI: the layer between agent fleets and the people who run them. Reliability, identity, governance, decision intelligence. Python reliability primitives, FastAPI intelligence engines, React operator surfaces. Audit trails on everything.

---

## ðŸš¦ Platform Reliability Stack for AI Agents Â· Python

A four-piece set. Each independent. All designed to compose:

| Repo | Surface | Buyer |
|---|---|---|
| [`rate-limit-shield`](https://github.com/mizcausevic-dev/rate-limit-shield) | Token bucket + circuit breaker + jittered retry, HTTP 429 / Retry-After awareness | **SRE** |
| [`identity-mesh`](https://github.com/mizcausevic-dev/identity-mesh) | SPIFFE-style JWT-SVID broker â€” short-lived tokens, audience binding, zero long-lived API keys | **CISO** |
| [`agent-canary`](https://github.com/mizcausevic-dev/agent-canary) | Progressive rollout, shadow mode, sticky-percent routing, auto-rollback | **Platform / SRE** |
| [`model-registry-pro`](https://github.com/mizcausevic-dev/model-registry-pro) | Model lifecycle catalog with lineage, stage promotion, approval gates | **Platform / MLOps** |

Identity at the edge â†’ rate limits at the model â†’ canary at deploy â†’ registry as source of truth. **Defense-in-depth for the agent era.**

---

## ðŸ§  Decision Intelligence Engines Â· Python + FastAPI

| Repo | What it does |
|---|---|
| [`briefing-intelligence-engine`](https://github.com/mizcausevic-dev/briefing-intelligence-engine) | Executive briefing scoring, narrative generation, risk ranking, action sequencing |
| [`signal-orchestration-lab`](https://github.com/mizcausevic-dev/signal-orchestration-lab) | Dependency-aware signal routing, escalation sequencing, cross-functional response planning |

These pair with the React + TypeScript executive surfaces below into full-stack decision products.

---

## ðŸ§° AI Platform & Governance Â· TypeScript

Production-shaped governance and observability for AI / LLM workloads:

- [`mcp-sentinel`](https://github.com/mizcausevic-dev/mcp-sentinel) â€” MCP server observability + security audit
- [`rag-sentinel`](https://github.com/mizcausevic-dev/rag-sentinel) â€” RAG quality / drift / hallucination signals
- [`agent-codex`](https://github.com/mizcausevic-dev/agent-codex) â€” governance-as-code with SOC 2 / EU AI Act / ISO 27001 / NIST mappings
- [`agent-eval-arena`](https://github.com/mizcausevic-dev/agent-eval-arena) â€” eval harness with regression detection + CI gates
- [`agent-router`](https://github.com/mizcausevic-dev/agent-router) â€” LLM router with provider-aware routing and breakers
- [`agentobserve`](https://github.com/mizcausevic-dev/agentobserve) â€” Datadog-shaped operator surface for agent fleets
- [`llm-redaction-gateway`](https://github.com/mizcausevic-dev/llm-redaction-gateway) â€” PII + secret redaction for LLM API calls
- [`shadow-ai-detector`](https://github.com/mizcausevic-dev/shadow-ai-detector) â€” unauthorized LLM usage detection across enterprise networks
- [`ai-finops-radar`](https://github.com/mizcausevic-dev/ai-finops-radar) â€” token-level cost attribution + anomaly detection
- [`kinetic-flightdeck`](https://github.com/mizcausevic-dev/kinetic-flightdeck) â€” unified AI Platform Engineering ops console

---

## ðŸ“Š Operator Surfaces Â· React + TypeScript

Executive dashboards, control planes, decision studios:

**Executive & Portfolio**
[`executive-briefing-studio`](https://github.com/mizcausevic-dev/executive-briefing-studio) Â· [`portfolio-command-center`](https://github.com/mizcausevic-dev/portfolio-command-center) Â· [`executive_operations_dashboard`](https://github.com/mizcausevic-dev/executive_operations_dashboard)

**Revenue & Growth**
[`customer-intelligence-graph`](https://github.com/mizcausevic-dev/customer-intelligence-graph) Â· [`growth-systems-control-room`](https://github.com/mizcausevic-dev/growth-systems-control-room) Â· [`revenue-forecasting-workbench`](https://github.com/mizcausevic-dev/revenue-forecasting-workbench) Â· [`attribution-intelligence-studio`](https://github.com/mizcausevic-dev/attribution-intelligence-studio) Â· [`pricing-experiment-studio`](https://github.com/mizcausevic-dev/pricing-experiment-studio) Â· [`conversion-funnel-intelligence-hub`](https://github.com/mizcausevic-dev/conversion-funnel-intelligence-hub) Â· [`deal-desk-workspace`](https://github.com/mizcausevic-dev/deal-desk-workspace)

**AI Governance & Risk**
[`ai-governance-review-studio`](https://github.com/mizcausevic-dev/ai-governance-review-studio) Â· [`model-risk-oversight-hub`](https://github.com/mizcausevic-dev/model-risk-oversight-hub) Â· [`vendor-risk-operations-center`](https://github.com/mizcausevic-dev/vendor-risk-operations-center) Â· [`compliance-workflow-hub`](https://github.com/mizcausevic-dev/compliance-workflow-hub) Â· [`ai-operations-console`](https://github.com/mizcausevic-dev/ai-operations-console)

**Identity & Security**
[`identity-command-center`](https://github.com/mizcausevic-dev/identity-command-center) Â· [`identity-lifecycle-workbench`](https://github.com/mizcausevic-dev/identity-lifecycle-workbench) Â· [`security-posture-control-room`](https://github.com/mizcausevic-dev/security-posture-control-room)

**Workflow & Operations**
[`workflow-orchestration-studio`](https://github.com/mizcausevic-dev/workflow-orchestration-studio) Â· [`feature-flag-rollout-studio`](https://github.com/mizcausevic-dev/feature-flag-rollout-studio) Â· [`ab-testing-command-center`](https://github.com/mizcausevic-dev/ab-testing-command-center) Â· [`customer-journey-control-plane`](https://github.com/mizcausevic-dev/customer-journey-control-plane)

---

## ðŸ”Œ Backend APIs Â· TypeScript + Node

Spec-first OpenAPI services:

[`Identity-Access-Audit-API`](https://github.com/mizcausevic-dev/Identity-Access-Audit-API) Â· [`observability-incident-command-api`](https://github.com/mizcausevic-dev/observability-incident-command-api) Â· [`customer-health-churn-api`](https://github.com/mizcausevic-dev/customer-health-churn-api) Â· [`partner-lead-distribution-engine`](https://github.com/mizcausevic-dev/partner-lead-distribution-engine) Â· [`content-workflow-intelligence-platform`](https://github.com/mizcausevic-dev/content-workflow-intelligence-platform) Â· [`experimentation_insights_kpi`](https://github.com/mizcausevic-dev/experimentation_insights_kpi) Â· [`seo-governance-platform`](https://github.com/mizcausevic-dev/seo-governance-platform) Â· [`webhook-ingestion-pipeline`](https://github.com/mizcausevic-dev/webhook-ingestion-pipeline) Â· [`kinetic-api-gateway`](https://github.com/mizcausevic-dev/kinetic-api-gateway) Â· [`revenue-ops-ai-assistant`](https://github.com/mizcausevic-dev/revenue-ops-ai-assistant)

---

## ðŸ—ƒï¸ Data & Analytics

[`revops-database-lab`](https://github.com/mizcausevic-dev/revops-database-lab) Â· [`revenue-intelligence-db`](https://github.com/mizcausevic-dev/revenue-intelligence-db) Â· [`cloud-cost-intelligence-dashboard`](https://github.com/mizcausevic-dev/cloud-cost-intelligence-dashboard)

PostgreSQL revenue modeling, attribution analysis, forecast and renewal risk reporting, cloud cost intelligence.

---

## ðŸ› ï¸ Stack

| Layer | Tools |
|---|---|
| **Languages** | Python Â· TypeScript Â· SQL (PostgreSQL) Â· Bash |
| **Backend** | FastAPI Â· Express Â· Hatchling packaging Â· GitHub Actions CI |
| **Frontend** | React Â· TypeScript Â· Vite Â· Tailwind Â· Recharts |
| **Data** | PostgreSQL Â· Pandas Â· OpenAPI / Swagger / Pydantic |
| **Reliability** | SRE primitives (buckets Â· breakers Â· retries Â· canaries) Â· SPIFFE zero-trust identity Â· governance-as-code |
| **Process** | Spec-first APIs Â· TDD Â· MIT-licensed Â· documented architectures Â· audit-ready |

---

## ðŸ¤ Working Interest

Open to **Director / Principal-level Platform Engineering, Web Engineering, or AI Platform** roles at enterprise B2B SaaS companies. East Coast time zone. Remote-friendly.

---

<sub>[All repositories](https://github.com/mizcausevic-dev?tab=repositories)</sub>