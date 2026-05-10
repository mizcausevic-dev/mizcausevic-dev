# Miz Causevic

> **Director of Web Engineering · Platform Architecture · B2B SaaS Technologist**
> Boston, MA · ~30 years across IBM, CyberArk, Alteryx, Digital.ai, Gryphon.ai

I ship platform infrastructure for production AI: the layer between agent fleets and the people who run them. Reliability, identity, governance, decision intelligence. Python reliability primitives, FastAPI intelligence engines, React operator surfaces. Audit trails on everything.

---

## 🚀 Currently Live

Four productized open-source dashboards live at `kineticgain.com` subdomains:

| Product | What it does | Buyer |
|---|---|---|
| [**gv.kineticgain.com**](https://gv.kineticgain.com) | **GitVisualizer** — visual portfolio for any GitHub user | Engineering |
| [**mcp.kineticgain.com**](https://mcp.kineticgain.com) | **MCP Sentinel** — governance dashboard for Model Context Protocol servers | CISO |
| [**rag.kineticgain.com**](https://rag.kineticgain.com) | **RAG Sentinel** — hallucination + drift + citation quality monitoring | ML / AI Ops |
| [**observe.kineticgain.com**](https://observe.kineticgain.com) | **AgentObserve** — operator console for AI agent fleets | SRE |

All four: React 19 + TypeScript, AGPL-3.0, CI green. Source repos under [`mizcausevic-dev`](https://github.com/mizcausevic-dev).

---

## 🚦 Platform Reliability Stack for AI Agents · Python

A four-piece set. Each independent. All designed to compose:

| Repo | Surface | Buyer |
|---|---|---|
| [`rate-limit-shield`](https://github.com/mizcausevic-dev/rate-limit-shield) | Token bucket + circuit breaker + jittered retry, HTTP 429 / Retry-After awareness | **SRE** |
| [`identity-mesh`](https://github.com/mizcausevic-dev/identity-mesh) | SPIFFE-style JWT-SVID broker — short-lived tokens, audience binding, zero long-lived API keys | **CISO** |
| [`agent-canary`](https://github.com/mizcausevic-dev/agent-canary) | Progressive rollout, shadow mode, sticky-percent routing, auto-rollback | **Platform / SRE** |
| [`model-registry-pro`](https://github.com/mizcausevic-dev/model-registry-pro) | Model lifecycle catalog with lineage, stage promotion, approval gates | **Platform / MLOps** |

Identity at the edge → rate limits at the model → canary at deploy → registry as source of truth. **Defense-in-depth for the agent era.**

---

## 🧠 Decision Intelligence Engines · Python + FastAPI

| Repo | What it does |
|---|---|
| [`briefing-intelligence-engine`](https://github.com/mizcausevic-dev/briefing-intelligence-engine) | Executive briefing scoring, narrative generation, risk ranking, action sequencing |
| [`signal-orchestration-lab`](https://github.com/mizcausevic-dev/signal-orchestration-lab) | Dependency-aware signal routing, escalation sequencing, cross-functional response planning |

These pair with the React + TypeScript executive surfaces below into full-stack decision products.

---

## 🧰 AI Platform & Governance · TypeScript

Production-shaped governance and observability for AI / LLM workloads:

- [`mcp-sentinel`](https://github.com/mizcausevic-dev/mcp-sentinel) — MCP server observability + security audit
- [`rag-sentinel`](https://github.com/mizcausevic-dev/rag-sentinel) — RAG quality / drift / hallucination signals
- [`agent-codex`](https://github.com/mizcausevic-dev/agent-codex) — governance-as-code with SOC 2 / EU AI Act / ISO 27001 / NIST mappings
- [`agent-eval-arena`](https://github.com/mizcausevic-dev/agent-eval-arena) — eval harness with regression detection + CI gates
- [`agent-router`](https://github.com/mizcausevic-dev/agent-router) — LLM router with provider-aware routing and breakers
- [`agentobserve`](https://github.com/mizcausevic-dev/agentobserve) — Datadog-shaped operator surface for agent fleets
- [`llm-redaction-gateway`](https://github.com/mizcausevic-dev/llm-redaction-gateway) — PII + secret redaction for LLM API calls
- [`shadow-ai-detector`](https://github.com/mizcausevic-dev/shadow-ai-detector) — unauthorized LLM usage detection across enterprise networks
- [`ai-finops-radar`](https://github.com/mizcausevic-dev/ai-finops-radar) — token-level cost attribution + anomaly detection
- [`kinetic-flightdeck`](https://github.com/mizcausevic-dev/kinetic-flightdeck) — unified AI Platform Engineering ops console

---

## 📊 Operator Surfaces · React + TypeScript

Executive dashboards, control planes, decision studios:

**Executive & Portfolio**
[`executive-briefing-studio`](https://github.com/mizcausevic-dev/executive-briefing-studio) · [`portfolio-command-center`](
cd $env:USERPROFILE\Downloads

Remove-Item -Recurse -Force .\profile-repo -ErrorAction SilentlyContinue
git clone https://github.com/mizcausevic-dev/mizcausevic-dev.git profile-repo
cd .\profile-repo

# Diagnostic: confirm mojibake is in the current file
$current = Get-Content .\README.md -Raw
if ($current -match "Ã.Â") {
    Write-Host "✗ Mojibake confirmed in current README" -ForegroundColor Red
} else {
    Write-Host "Current file looks clean (maybe display-only issue?)" -ForegroundColor Yellow
}


> **Director of Web Engineering · Platform Architecture · B2B SaaS Technologist**
> Boston, MA · ~30 years across IBM, CyberArk, Alteryx, Digital.ai, Gryphon.ai

I ship platform infrastructure for production AI: the layer between agent fleets and the people who run them. Reliability, identity, governance, decision intelligence. Python reliability primitives, FastAPI intelligence engines, React operator surfaces. Audit trails on everything.

---

## 🚀 Currently Live

Four productized open-source dashboards live at `kineticgain.com` subdomains:

| Product | What it does | Buyer |
|---|---|---|
| [**gv.kineticgain.com**](https://gv.kineticgain.com) | **GitVisualizer** — visual portfolio for any GitHub user | Engineering |
| [**mcp.kineticgain.com**](https://mcp.kineticgain.com) | **MCP Sentinel** — governance dashboard for Model Context Protocol servers | CISO |
| [**rag.kineticgain.com**](https://rag.kineticgain.com) | **RAG Sentinel** — hallucination + drift + citation quality monitoring | ML / AI Ops |
| [**observe.kineticgain.com**](https://observe.kineticgain.com) | **AgentObserve** — operator console for AI agent fleets | SRE |

All four: React 19 + TypeScript, AGPL-3.0, CI green. Source repos under [`mizcausevic-dev`](https://github.com/mizcausevic-dev).

---

## 🚦 Platform Reliability Stack for AI Agents · Python

A four-piece set. Each independent. All designed to compose:

| Repo | Surface | Buyer |
|---|---|---|
| [`rate-limit-shield`](https://github.com/mizcausevic-dev/rate-limit-shield) | Token bucket + circuit breaker + jittered retry, HTTP 429 / Retry-After awareness | **SRE** |
| [`identity-mesh`](https://github.com/mizcausevic-dev/identity-mesh) | SPIFFE-style JWT-SVID broker — short-lived tokens, audience binding, zero long-lived API keys | **CISO** |
| [`agent-canary`](https://github.com/mizcausevic-dev/agent-canary) | Progressive rollout, shadow mode, sticky-percent routing, auto-rollback | **Platform / SRE** |
| [`model-registry-pro`](https://github.com/mizcausevic-dev/model-registry-pro) | Model lifecycle catalog with lineage, stage promotion, approval gates | **Platform / MLOps** |

Identity at the edge → rate limits at the model → canary at deploy → registry as source of truth. **Defense-in-depth for the agent era.**

---

## 🧠 Decision Intelligence Engines · Python + FastAPI

| Repo | What it does |
|---|---|
| [`briefing-intelligence-engine`](https://github.com/mizcausevic-dev/briefing-intelligence-engine) | Executive briefing scoring, narrative generation, risk ranking, action sequencing |
| [`signal-orchestration-lab`](https://github.com/mizcausevic-dev/signal-orchestration-lab) | Dependency-aware signal routing, escalation sequencing, cross-functional response planning |

These pair with the React + TypeScript executive surfaces below into full-stack decision products.

---

## 🧰 AI Platform & Governance · TypeScript

Production-shaped governance and observability for AI / LLM workloads:

- [`mcp-sentinel`](https://github.com/mizcausevic-dev/mcp-sentinel) — MCP server observability + security audit
- [`rag-sentinel`](https://github.com/mizcausevic-dev/rag-sentinel) — RAG quality / drift / hallucination signals
- [`agent-codex`](https://github.com/mizcausevic-dev/agent-codex) — governance-as-code with SOC 2 / EU AI Act / ISO 27001 / NIST mappings
- [`agent-eval-arena`](https://github.com/mizcausevic-dev/agent-eval-arena) — eval harness with regression detection + CI gates
- [`agent-router`](https://github.com/mizcausevic-dev/agent-router) — LLM router with provider-aware routing and breakers
- [`agentobserve`](https://github.com/mizcausevic-dev/agentobserve) — Datadog-shaped operator surface for agent fleets
- [`llm-redaction-gateway`](https://github.com/mizcausevic-dev/llm-redaction-gateway) — PII + secret redaction for LLM API calls
- [`shadow-ai-detector`](https://github.com/mizcausevic-dev/shadow-ai-detector) — unauthorized LLM usage detection across enterprise networks
- [`ai-finops-radar`](https://github.com/mizcausevic-dev/ai-finops-radar) — token-level cost attribution + anomaly detection
- [`kinetic-flightdeck`](https://github.com/mizcausevic-dev/kinetic-flightdeck) — unified AI Platform Engineering ops console

---

## 📊 Operator Surfaces · React + TypeScript

Executive dashboards, control planes, decision studios:

**Executive & Portfolio**
[`executive-briefing-studio`](https://github.com/mizcausevic-dev/executive-briefing-studio) · [`portfolio-command-center`](https://github.com/mizcausevic-dev/portfolio-command-center) · [`executive_operations_dashboard`](https://github.com/mizcausevic-dev/executive_operations_dashboard)

**Revenue & Growth**
[`customer-intelligence-graph`](https://github.com/mizcausevic-dev/customer-intelligence-graph) · [`growth-systems-control-room`](https://github.com/mizcausevic-dev/growth-systems-control-room) · [`revenue-forecasting-workbench`](https://github.com/mizcausevic-dev/revenue-forecasting-workbench) · [`attribution-intelligence-studio`](https://github.com/mizcausevic-dev/attribution-intelligence-studio) · [`pricing-experiment-studio`](https://github.com/mizcausevic-dev/pricing-experiment-studio) · [`conversion-funnel-intelligence-hub`](https://github.com/mizcausevic-dev/conversion-funnel-intelligence-hub) · [`deal-desk-workspace`](https://github.com/mizcausevic-dev/deal-desk-workspace)

**AI Governance & Risk**
[`ai-governance-review-studio`](https://github.com/mizcausevic-dev/ai-governance-review-studio) · [`model-risk-oversight-hub`](https://github.com/mizcausevic-dev/model-risk-oversight-hub) · [`vendor-risk-operations-center`](https://github.com/mizcausevic-dev/vendor-risk-operations-center) · [`compliance-workflow-hub`](https://github.com/mizcausevic-dev/compliance-workflow-hub) · [`ai-operations-console`](https://github.com/mizcausevic-dev/ai-operations-console)

**Identity & Security**
[`identity-command-center`](https://github.com/mizcausevic-dev/identity-command-center) · [`identity-lifecycle-workbench`](https://github.com/mizcausevic-dev/identity-lifecycle-workbench) · [`security-posture-control-room`](https://github.com/mizcausevic-dev/security-posture-control-room)

**Workflow & Operations**
[`workflow-orchestration-studio`](https://github.com/mizcausevic-dev/workflow-orchestration-studio) · [`feature-flag-rollout-studio`](https://github.com/mizcausevic-dev/feature-flag-rollout-studio) · [`ab-testing-command-center`](https://github.com/mizcausevic-dev/ab-testing-command-center) · [`customer-journey-control-plane`](https://github.com/mizcausevic-dev/customer-journey-control-plane)

---

## 🔌 Backend APIs · TypeScript + Node

Spec-first OpenAPI services:

[`Identity-Access-Audit-API`](https://github.com/mizcausevic-dev/Identity-Access-Audit-API) · [`observability-incident-command-api`](https://github.com/mizcausevic-dev/observability-incident-command-api) · [`customer-health-churn-api`](https://github.com/mizcausevic-dev/customer-health-churn-api) · [`partner-lead-distribution-engine`](https://github.com/mizcausevic-dev/partner-lead-distribution-engine) · [`content-workflow-intelligence-platform`](https://github.com/mizcausevic-dev/content-workflow-intelligence-platform) · [`experimentation_insights_kpi`](https://github.com/mizcausevic-dev/experimentation_insights_kpi) · [`seo-governance-platform`](https://github.com/mizcausevic-dev/seo-governance-platform) · [`webhook-ingestion-pipeline`](https://github.com/mizcausevic-dev/webhook-ingestion-pipeline) · [`kinetic-api-gateway`](https://github.com/mizcausevic-dev/kinetic-api-gateway) · [`revenue-ops-ai-assistant`](https://github.com/mizcausevic-dev/revenue-ops-ai-assistant)

---

## 🗃️ Data & Analytics

[`revops-database-lab`](https://github.com/mizcausevic-dev/revops-database-lab) · [`revenue-intelligence-db`](https://github.com/mizcausevic-dev/revenue-intelligence-db) · [`cloud-cost-intelligence-dashboard`](https://github.com/mizcausevic-dev/cloud-cost-intelligence-dashboard)

PostgreSQL revenue modeling, attribution analysis, forecast and renewal risk reporting, cloud cost intelligence.

---

## 🛠️ Stack

| Layer | Tools |
|---|---|
| **Languages** | Python · TypeScript · SQL (PostgreSQL) · Bash |
| **Backend** | FastAPI · Express · Hatchling packaging · GitHub Actions CI |
| **Frontend** | React · TypeScript · Vite · Tailwind · Recharts |
| **Data** | PostgreSQL · Pandas · OpenAPI / Swagger / Pydantic |
| **Reliability** | SRE primitives (buckets · breakers · retries · canaries) · SPIFFE zero-trust identity · governance-as-code |
| **Process** | Spec-first APIs · TDD · MIT-licensed · documented architectures · audit-ready |

---

## 🤝 Working Interest

Open to **Director / Principal-level Platform Engineering, Web Engineering, or AI Platform** roles at enterprise B2B SaaS companies. East Coast time zone. Remote-friendly.

> *"Long-lived credentials are tomorrow's incident reports. Build short-lived. Audit always. Document once."*

---

<sub>[All repositories](https://github.com/mizcausevic-dev?tab=repositories)</sub>
