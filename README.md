# Miz Causevic

> **Director of Web Engineering · Platform Architecture · B2B SaaS Technologist**
> Boston, MA · ~30 years across IBM, CyberArk, Alteryx, Digital.ai, Gryphon.ai

I ship platform infrastructure for production AI: the layer between agent fleets and the people who run them. Reliability primitives, identity governance, AI observability, decision intelligence. **I also author open specifications for the answer-engine era** — see the [Kinetic Gain Protocol Suite](#-kinetic-gain-protocol-suite) below. Polyglot by choice: the language fits the problem, not the resume.

---

## 🚀 Currently Live

**Five** productized open-source products live at `kineticgain.com` subdomains. **All push-to-deploy via GitHub Actions FTP CI/CD.**

| Product | What it does | Buyer |
|---|---|---|
| [**gv.kineticgain.com**](https://gv.kineticgain.com) | **GitVisualizer** — visual portfolio intelligence for any GitHub user | Engineering / Hiring |
| [**mcp.kineticgain.com**](https://mcp.kineticgain.com) | **MCP Sentinel** — governance dashboard for Model Context Protocol servers | CISO / Platform Security |
| [**rag.kineticgain.com**](https://rag.kineticgain.com) | **RAG Sentinel** — hallucination, drift, and citation quality monitoring | ML / AI Ops |
| [**observe.kineticgain.com**](https://observe.kineticgain.com) | **AgentObserve** — operator console for AI agent fleets | SRE / Platform |
| [**aeo.kineticgain.com**](https://aeo.kineticgain.com) | **AEO Visualizer** — interactive renderer for AEO Protocol declarations | Platform Eng / AEO |

All five: React 19 + TypeScript, AGPL-3.0, CI green, push-to-deploy via FTP Action.

---

## 🧬 Kinetic Gain Protocol Suite

A family of **five open JSON specifications** for the answer-engine era, with full reference implementations and unified tooling. All AGPL-3.0, all v0.1 draft, all `kinetic-gain-protocol-suite` tagged.

### 📐 Specifications

| Spec | What it declares | Detect via |
|---|---|---|
| [`aeo-protocol-spec`](https://github.com/mizcausevic-dev/aeo-protocol-spec) | **AEO Protocol** — entity declaration at `/.well-known/aeo.json` | `aeo_version` |
| [`prompt-provenance-spec`](https://github.com/mizcausevic-dev/prompt-provenance-spec) | **Prompt Provenance** — versioned, lineaged, reviewable LLM prompt records | `provenance_version` |
| [`agent-cards-spec`](https://github.com/mizcausevic-dev/agent-cards-spec) | **Agent Cards** — declarative agent capability + refusal disclosure | `agent_card_version` |
| [`ai-evidence-format-spec`](https://github.com/mizcausevic-dev/ai-evidence-format-spec) | **AI Evidence Format** — structured citations for LLM-generated claims | `evidence_version` |
| [`mcp-tool-card-spec`](https://github.com/mizcausevic-dev/mcp-tool-card-spec) | **MCP Tool Cards** — per-tool disclosure for Model Context Protocol servers | `tool_card_version` |

### 🛠️ AEO Reference Stack

The canonical depth example — every layer needed to consume the spec, across five languages:

| Layer | Repos |
|---|---|
| **SDKs** | [`aeo-sdk-python`](https://github.com/mizcausevic-dev/aeo-sdk-python) (live on [PyPI](https://pypi.org/project/aeo-protocol/)) · [`aeo-sdk-typescript`](https://github.com/mizcausevic-dev/aeo-sdk-typescript) · [`aeo-sdk-rust`](https://github.com/mizcausevic-dev/aeo-sdk-rust) · [`aeo-sdk-go`](https://github.com/mizcausevic-dev/aeo-sdk-go) · [`aeo-sdk-swift`](https://github.com/mizcausevic-dev/aeo-sdk-swift) |
| **CLI** | [`aeo-cli`](https://github.com/mizcausevic-dev/aeo-cli) — `aeo validate / fetch / inspect / claim`, colored output, end-to-end against the live well-known URL |
| **Crawler** | [`aeo-crawler`](https://github.com/mizcausevic-dev/aeo-crawler) — BFS over AEO graphs, JSON Lines output, configurable depth + concurrency |

### 🔌 MCP Integration

| Repo | What it does |
|---|---|
| [`mcp-aeo-server`](https://github.com/mizcausevic-dev/mcp-aeo-server) | AEO-only MCP server — 4 tools, one Claude Desktop config entry |
| [`mcp-kinetic-gain`](https://github.com/mizcausevic-dev/mcp-kinetic-gain) | **Unified MCP server** — 18 tools across all five specs, one config entry, 27 tests |

### 🖼️ Visualizers

| Live | Repo | What it does |
|---|---|---|
| [`aeo.kineticgain.com`](https://aeo.kineticgain.com) | [`aeo-visualizer`](https://github.com/mizcausevic-dev/aeo-visualizer) | Dedicated AEO Protocol web visualizer |
| [`kinetic-gain-visualizer`](https://mizcausevic-dev.github.io/kinetic-gain-visualizer/) | [`kinetic-gain-visualizer`](https://github.com/mizcausevic-dev/kinetic-gain-visualizer) | **Unified visualizer** — auto-detects the spec from the top-level `*_version` field and renders the appropriate view. Five views: Visualize / Editor / Architecture / Tools / About |

The unified visualizer + unified MCP server give the Suite a complete read-side (human) and tool-side (agent) entry point. Five specs, two front doors.

---

## 🛡️ Platform Reliability Stack · Python

A four-piece set. Each independent. All designed to compose:

| Repo | Surface | Buyer |
|---|---|---|
| [`rate-limit-shield`](https://github.com/mizcausevic-dev/rate-limit-shield) | Token bucket + circuit breaker + jittered retry, HTTP 429 / Retry-After awareness | **SRE** |
| [`identity-mesh`](https://github.com/mizcausevic-dev/identity-mesh) | SPIFFE-style JWT-SVID broker — short-lived tokens, audience binding, zero long-lived keys | **CISO** |
| [`agent-canary`](https://github.com/mizcausevic-dev/agent-canary) | Progressive rollout, shadow mode, sticky-percent routing, auto-rollback | **Platform / SRE** |
| [`model-registry-pro`](https://github.com/mizcausevic-dev/model-registry-pro) | Model lifecycle catalog: lineage, stage promotion, approval gates | **Platform / MLOps** |

Identity at the edge → rate limits at the model → canary at deploy → registry as source of truth. **Defense-in-depth for the agent era.**

---

## 🌐 Polyglot Platform Stack

Production-shaped backend services in the right language for the problem. **15+ languages across one coherent platform.**

| Language | Repo | What it does |
|---|---|---|
| **Go** | [`edge-policy-enforcer`](https://github.com/mizcausevic-dev/edge-policy-enforcer) | Edge request governance, bot handling, redirect control |
| **Go** | [`latency-budget-enforcer`](https://github.com/mizcausevic-dev/latency-budget-enforcer) | Latency budget enforcement, dependency drag review |
| **Rust** | [`crawl-anomaly-detector`](https://github.com/mizcausevic-dev/crawl-anomaly-detector) | Crawl log anomaly scoring, indexing risk review |
| **Rust** | [`support-escalation-router`](https://github.com/mizcausevic-dev/support-escalation-router) | Support queue escalation, SLA pressure scoring |
| **Java** | [`compliance-event-ledger`](https://github.com/mizcausevic-dev/compliance-event-ledger) | Spring Boot immutable compliance event history |
| **C#** | [`tenant-isolation-guard`](https://github.com/mizcausevic-dev/tenant-isolation-guard) | ASP.NET Core tenant-boundary policy evaluation |
| **C#** | [`approval-workflow-orchestrator`](https://github.com/mizcausevic-dev/approval-workflow-orchestrator) | ASP.NET Core approval routing, SLA-aware escalation |
| **Kotlin** | [`release-readiness-gatekeeper`](https://github.com/mizcausevic-dev/release-readiness-gatekeeper) | Release gate evaluation, dependency readiness scoring |
| **Kotlin** | [`reliability-policy-coordinator`](https://github.com/mizcausevic-dev/reliability-policy-coordinator) | Dependency drag review, error-budget policy |
| **Scala** | [`policy-decision-simulator`](https://github.com/mizcausevic-dev/policy-decision-simulator) | Policy simulation for governance scenarios, launch gates |
| **Elixir** | [`incident-handoff-broker`](https://github.com/mizcausevic-dev/incident-handoff-broker) | Incident routing, SLA-aware handoff scoring |
| **Ruby** | [`message-retention-guardian`](https://github.com/mizcausevic-dev/message-retention-guardian) | Retention policy enforcement, legal hold protection |
| **PHP** | [`entitlement-request-portal-api`](https://github.com/mizcausevic-dev/entitlement-request-portal-api) | Entitlement requests, approval routing, access review |
| **Dart** | [`mobile-briefing-companion`](https://github.com/mizcausevic-dev/mobile-briefing-companion) | Flutter mobile app for executive briefings, signal summaries |
| **Terraform** | [`platform-foundation-blueprint`](https://github.com/mizcausevic-dev/platform-foundation-blueprint) | Multi-environment networking, IAM blueprint |
| **Go** | [`grpc-mesh-shadow`](https://github.com/mizcausevic-dev/grpc-mesh-shadow) | gRPC shadow traffic mirroring, divergence detection, sampling |
| **Go** | [`miz-otel-pack`](https://github.com/mizcausevic-dev/miz-otel-pack) | OpenTelemetry SpanProcessor — GenAI spans → business cost/latency spans |
| **Rust** | [`wasm-policy-gateway`](https://github.com/mizcausevic-dev/wasm-policy-gateway) | WASI policy engine — geo + rate-limit + A/B routing, ~128 KB module |
| **Rust** | [`bls-attestation-broker`](https://github.com/mizcausevic-dev/bls-attestation-broker) | BLS12-381 aggregate signatures for multi-signer attestation |
| **Zig** | [`zig-agent-graph-db`](https://github.com/mizcausevic-dev/zig-agent-graph-db) | In-memory directed graph for agent context, stdlib only |
| **Haskell** | [`haskell-policy-engine`](https://github.com/mizcausevic-dev/haskell-policy-engine) | Type-safe policy DSL with Hspec + QuickCheck properties |
| **Python** | [`embedding-drift-graph`](https://github.com/mizcausevic-dev/embedding-drift-graph) | Track cosine drift of entity embeddings across encoder versions, GraphQL API |
| **Python** | [`audit-graph-explorer`](https://github.com/mizcausevic-dev/audit-graph-explorer) | Neo4j + Cypher relationship-driven audit analysis |
| **Python** | [`secret-rotation-scheduler`](https://github.com/mizcausevic-dev/secret-rotation-scheduler) | Secret rotation windows, owner prompts, stale-secret detection |
| **Python** | [`warehouse-reconciliation-engine`](https://github.com/mizcausevic-dev/warehouse-reconciliation-engine) | Source-to-warehouse drift detection, finance-grade reconciliation |
| **Python** | [`data-quality-guardrail`](https://github.com/mizcausevic-dev/data-quality-guardrail) | Schema drift, freshness lag, null spike detection |
| **dbt + DuckDB** | [`dbt-search-observatory`](https://github.com/mizcausevic-dev/dbt-search-observatory) | Search console, crawl, index coverage, freshness modeling |
| **SQL Warehouse** | [`search-observability-warehouse`](https://github.com/mizcausevic-dev/search-observability-warehouse) | Crawl analytics, indexation, technical SEO observability |

---

## 🧠 AI Governance & Platform Engines · TypeScript

Production-shaped governance and observability for AI / LLM workloads:

- [`mcp-sentinel`](https://github.com/mizcausevic-dev/mcp-sentinel) — MCP server observability + security audit
- [`rag-sentinel`](https://github.com/mizcausevic-dev/rag-sentinel) — RAG quality / drift / hallucination signals
- [`agentobserve`](https://github.com/mizcausevic-dev/agentobserve) — Datadog-shaped operator surface for agent fleets
- [`agent-codex`](https://github.com/mizcausevic-dev/agent-codex) — governance-as-code: SOC 2 / EU AI Act / ISO 27001 / NIST mappings
- [`agent-eval-arena`](https://github.com/mizcausevic-dev/agent-eval-arena) — eval harness with regression detection + CI gates
- [`agent-router`](https://github.com/mizcausevic-dev/agent-router) — LLM router with provider-aware routing and breakers
- [`llm-redaction-gateway`](https://github.com/mizcausevic-dev/llm-redaction-gateway) — PII + secret redaction for LLM API calls
- [`shadow-ai-detector`](https://github.com/mizcausevic-dev/shadow-ai-detector) — unauthorized LLM usage detection
- [`ai-finops-radar`](https://github.com/mizcausevic-dev/ai-finops-radar) — token-level cost attribution + anomaly detection
- [`kinetic-flightdeck`](https://github.com/mizcausevic-dev/kinetic-flightdeck) — unified AI Platform Engineering ops console

---

## 🧪 Decision Intelligence Engines · Python + FastAPI

| Repo | What it does |
|---|---|
| [`briefing-intelligence-engine`](https://github.com/mizcausevic-dev/briefing-intelligence-engine) | Executive briefing scoring, narrative generation, risk ranking |
| [`signal-orchestration-lab`](https://github.com/mizcausevic-dev/signal-orchestration-lab) | Dependency-aware signal routing, escalation sequencing |

---

## 📊 Operator Surfaces · React + TypeScript

Executive dashboards, control planes, decision studios — organized by domain:

**Executive & Portfolio**
[`executive-briefing-studio`](https://github.com/mizcausevic-dev/executive-briefing-studio) · [`portfolio-command-center`](https://github.com/mizcausevic-dev/portfolio-command-center) · [`executive_operations_dashboard`](https://github.com/mizcausevic-dev/executive_operations_dashboard) · [`scenario-planning-atlas`](https://github.com/mizcausevic-dev/scenario-planning-atlas)

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
| **Languages** | Python · TypeScript · Go · Rust · Java · C# · Kotlin · Scala · Elixir · Ruby · PHP · Dart · Swift · Zig · Haskell · SQL · HCL · dbt |
| **Backend** | FastAPI · Express · Spring Boot · ASP.NET Core · Javalin · Cowboy/Plug · WEBrick |
| **Frontend** | React 19 · Vue 3 · Flutter · TypeScript · Vite · Tailwind · Recharts · Motion |
| **Data** | PostgreSQL · DuckDB · dbt · Neo4j · Pandas · Pydantic |
| **AI / Platform** | SPIFFE zero-trust identity · governance-as-code · LLM routing · token-cost attribution · OpenAPI specs · MCP servers · OpenTelemetry GenAI · BLS aggregate signatures · WASI · spec authorship |
| **CI/CD** | GitHub Actions · FTP auto-deploy · Hostinger · AGPL-3.0 licensing |

---

## 🤝 Working Interest

Open to **Director / Principal-level Platform Engineering, Web Engineering, or AI Platform** roles at enterprise B2B SaaS companies. East Coast time zone. Remote-friendly.

> *"Long-lived credentials are tomorrow's incident reports. Build short-lived. Audit always. Document once."*

---

<sub>[All active repositories](https://github.com/mizcausevic-dev?tab=repositories&type=public&sort=updated) · [Career one-pager](https://mizcausevic-dev.github.io/)</sub>

---

**Connect:** [LinkedIn](https://www.linkedin.com/in/mirzacausevic/) · [Kinetic Gain](https://kineticgain.com) · [Medium](https://medium.com/@mizcausevic/) · [Skills](https://mizcausevic.com/skills/)
