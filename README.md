# Miz Causevic

> **Engineering · Platform Architecture · B2B SaaS Technologist**
> Boston, MA · ~30 years across IBM, CyberArk, Alteryx, Digital.ai, Gryphon.ai

I ship platform infrastructure for production AI: the layer between agent fleets and the people who run them. Reliability primitives, identity governance, AI observability, decision intelligence. **I also author open specifications for the answer-engine era** — see the [Kinetic Gain Protocol Suite](#-kinetic-gain-protocol-suite) below. Polyglot by choice: the language fits the problem, not the resume.

**Publication note:** many of the repos below were published in a concentrated May 2026 portfolio sprint. The dates reflect public packaging, CI, screenshots, and repo hardening, not the first moment the ideas or workstreams existed.

---

## 🚀 Currently Live

**Twenty-two** productized open-source properties live at `kineticgain.com` subdomains. **All push-to-deploy via GitHub Actions FTP CI/CD.** Front door: **[suite.kineticgain.com](https://suite.kineticgain.com)** · Quickstart hub: **[docs.kineticgain.com](https://docs.kineticgain.com)**.

### Hubs + tools

| Property | What it does | Buyer |
|---|---|---|
| [**suite.kineticgain.com**](https://suite.kineticgain.com) | **Kinetic Gain Protocol Suite** — canonical front door for all 11 open AI governance specs + [NIST AI RMF crosswalk](https://suite.kineticgain.com/docs/nist-rmf-crosswalk.md) | Recruiters / investors / generalist |
| [**docs.kineticgain.com**](https://docs.kineticgain.com) | **Quickstart hub** — per-role guides (CISO / district / healthcare vendor / answer engine) + canonical `/.well-known/` path map | New visitors / implementers |
| [**directory.kineticgain.com**](https://directory.kineticgain.com) | **Vendor directory** — curated list of domains publishing Kinetic Gain documents | Procurement reviewers |
| [**examples.kineticgain.com**](https://examples.kineticgain.com) | **Examples gallery** — pick a spec, see its canonical example with JSON highlight | Developers / spec authors |
| [**walker.kineticgain.com**](https://walker.kineticgain.com) | **well-known-walker** — paste any domain, see every Kinetic Gain disclosure it publishes | Procurement / Risk reviewers |
| [**bench.kineticgain.com**](https://bench.kineticgain.com) | **prompt-injection-bench** — visual harness, paste a JSONL transcript, see pass rates | CISO / Red-team / Trust & Safety |

### Per-spec landing pages (one per spec in the Suite)

| Property | Spec | Buyer |
|---|---|---|
| [**aeo.kineticgain.com**](https://aeo.kineticgain.com) | AEO Protocol — interactive visualizer | Platform Eng / AEO |
| [**prompts.kineticgain.com**](https://prompts.kineticgain.com) | Prompt Provenance | LLM Platform / SRE |
| [**agents.kineticgain.com**](https://agents.kineticgain.com) | Agent Cards | Platform Eng / Procurement |
| [**evidence.kineticgain.com**](https://evidence.kineticgain.com) | AI Evidence Format | RAG / Search / Answer engines |
| [**toolcards.kineticgain.com**](https://toolcards.kineticgain.com) | MCP Tool Cards | MCP authors / Platform Sec |
| [**tutor.kineticgain.com**](https://tutor.kineticgain.com) | AI Tutor Cards | EdTech / District Procurement |
| [**student.kineticgain.com**](https://student.kineticgain.com) | Student AI Disclosure | Academic integrity / LMS |
| [**aup.kineticgain.com**](https://aup.kineticgain.com) | Classroom AI AUP | District / school / instructor |
| [**clinical.kineticgain.com**](https://clinical.kineticgain.com) | Clinical AI Disclosure (HIPAA / FDA / SaMD) | Hospital CMIO / Compliance |
| [**incidents.kineticgain.com**](https://incidents.kineticgain.com) | AI Incident Card — "CVE for AI agents" | CISO / Trust & Safety |

### Earlier product surfaces

| Property | What it does | Buyer |
|---|---|---|
| [**gv.kineticgain.com**](https://gv.kineticgain.com) | **GitVisualizer** — visual portfolio intelligence for any GitHub user | Engineering / Hiring |
| [**mcp.kineticgain.com**](https://mcp.kineticgain.com) | **MCP Sentinel** — governance dashboard for Model Context Protocol servers | CISO / Platform Security |
| [**rag.kineticgain.com**](https://rag.kineticgain.com) | **RAG Sentinel** — hallucination, drift, and citation quality monitoring | ML / AI Ops |
| [**observe.kineticgain.com**](https://observe.kineticgain.com) | **AgentObserve** — operator console for AI agent fleets | SRE / Platform |

All twenty-two: mix of AGPL-3.0 and Apache-2.0, CI green, push-to-deploy via FTP Action. **8 React 19 + TypeScript apps · 14 hand-written static HTML landings.**

---

## 🧬 Kinetic Gain Protocol Suite

A family of **eleven open JSON specifications** for the answer-engine and agent era — five core (AEO, Prompt Provenance, Agent Cards, AI Evidence Format, MCP Tool Cards), a three-spec **EdTech trio** (vendor / district / student), a **HealthTech vertical extension** (Clinical AI Disclosure — HIPAA / FDA / SaMD posture), a cross-cutting **AI Incident Card** that ties everything together post-hoc, and an **AI Procurement Decision Card** that signs off on a vendor's posture across the rest of the Suite. **Two regulated verticals covered. NIST AI RMF crosswalk shipped alongside.** All AGPL-3.0, all v0.1 draft, all `kinetic-gain-protocol-suite` tagged. Single landing: [`kinetic-gain-protocol-suite`](https://github.com/mizcausevic-dev/kinetic-gain-protocol-suite).

### 📐 Specifications

| Spec | What it declares | Detect via |
|---|---|---|
| [`aeo-protocol-spec`](https://github.com/mizcausevic-dev/aeo-protocol-spec) | **AEO Protocol** — entity declaration at `/.well-known/aeo.json` | `aeo_version` |
| [`prompt-provenance-spec`](https://github.com/mizcausevic-dev/prompt-provenance-spec) | **Prompt Provenance** — versioned, lineaged, reviewable LLM prompt records | `provenance_version` |
| [`agent-cards-spec`](https://github.com/mizcausevic-dev/agent-cards-spec) | **Agent Cards** — declarative agent capability + refusal disclosure | `agent_card_version` |
| [`ai-evidence-format-spec`](https://github.com/mizcausevic-dev/ai-evidence-format-spec) | **AI Evidence Format** — structured citations for LLM-generated claims | `evidence_version` |
| [`mcp-tool-card-spec`](https://github.com/mizcausevic-dev/mcp-tool-card-spec) | **MCP Tool Cards** — per-tool disclosure for Model Context Protocol servers | `tool_card_version` |
| [`ai-tutor-card-spec`](https://github.com/mizcausevic-dev/ai-tutor-card-spec) | **AI Tutor Cards** — EdTech vendor-side: pedagogy, FERPA/COPPA/GDPR posture | `tutor_card_version` |
| [`student-ai-disclosure-spec`](https://github.com/mizcausevic-dev/student-ai-disclosure-spec) | **Student AI Disclosure** — student-side: roles, prompt evidence (full/hashed/omitted), artifact-hash binding | `disclosure_version` |
| [`classroom-ai-aup-spec`](https://github.com/mizcausevic-dev/classroom-ai-aup-spec) | **Classroom AI AUP** — district / school / course-side policy (closes the EdTech trio) | `aup_version` |
| [`clinical-ai-disclosure-spec`](https://github.com/mizcausevic-dev/clinical-ai-disclosure-spec) | **Clinical AI Disclosure** — HealthTech vendor-side: HIPAA / FDA / SaMD posture, bias audits, EHR (FHIR / CDS Hooks) | `clinical_ai_card_version` |
| [`ai-incident-card-spec`](https://github.com/mizcausevic-dev/ai-incident-card-spec) | **AI Incident Card** — "CVE for AI agents," cross-references every other affected document in the Suite | `incident_card_version` |
| [`ai-procurement-decision-spec`](https://github.com/mizcausevic-dev/ai-procurement-decision-spec) | **AI Procurement Decision Card** — buyer-side approval/rejection record that signs off on a vendor's posture across the rest of the Suite | `decision_card_version` |

### 🛠️ AEO Reference Stack

The canonical depth example — every layer needed to consume the spec, across five languages:

| Layer | Repos |
|---|---|
| **SDKs** | [`aeo-sdk-python`](https://github.com/mizcausevic-dev/aeo-sdk-python) (live on [PyPI](https://pypi.org/project/aeo-protocol/)) · [`aeo-sdk-typescript`](https://github.com/mizcausevic-dev/aeo-sdk-typescript) · [`aeo-sdk-rust`](https://github.com/mizcausevic-dev/aeo-sdk-rust) · [`aeo-sdk-go`](https://github.com/mizcausevic-dev/aeo-sdk-go) · [`aeo-sdk-swift`](https://github.com/mizcausevic-dev/aeo-sdk-swift) |
| **CLI** | [`aeo-cli`](https://github.com/mizcausevic-dev/aeo-cli) — `aeo validate / fetch / inspect / claim`, colored output, end-to-end against the live well-known URL |
| **Crawler** | [`aeo-crawler`](https://github.com/mizcausevic-dev/aeo-crawler) — BFS over AEO graphs, JSON Lines output, configurable depth + concurrency |
| **Validator service** | [`aeo-validator-service`](https://github.com/mizcausevic-dev/aeo-validator-service) — **always-on HTTP validator** for AEO + all 11 Suite docs. Auto-detects the spec via `*_version` sniffing, hashes canonically, tracks **drift** across re-checks (`POST /watches/{id}/recheck` returns a structured `DriftReport`). |

### 🔌 MCP Integration

| Repo | What it does |
|---|---|
| [`mcp-aeo-server`](https://github.com/mizcausevic-dev/mcp-aeo-server) | AEO-only MCP server — 4 tools, one Claude Desktop config entry |
| [`mcp-kinetic-gain`](https://github.com/mizcausevic-dev/mcp-kinetic-gain) | **Unified MCP server** — **47 tools across 11 specs** (v0.5.2, git-tagged), one Claude Desktop config entry, 96 tests passing. Headline tools: `aup_check_compliance` joins an AUP + Student AI Disclosure into a single allow/deny call; `decision_card_validate` enforces the full procurement Decision Card conditional ruleset. |
| [`mcp-reliability-toolkit`](https://github.com/mizcausevic-dev/mcp-reliability-toolkit) | **Reliability MCP server** — 4 tools (`compute_slo_burn`, `design_rate_limiter`, `design_circuit_breaker`, `compose_reliability_pattern`). Same math as `slo-budget-tracker`; emits drop-in Python + Rust configs from a Claude conversation. |

### 🖼️ Visualizers + galleries

| Live | Repo | What it does |
|---|---|---|
| [`aeo.kineticgain.com`](https://aeo.kineticgain.com) | [`aeo-visualizer`](https://github.com/mizcausevic-dev/aeo-visualizer) | Dedicated AEO Protocol web visualizer |
| [`kinetic-gain-visualizer`](https://mizcausevic-dev.github.io/kinetic-gain-visualizer/) | [`kinetic-gain-visualizer`](https://github.com/mizcausevic-dev/kinetic-gain-visualizer) | **Unified visualizer** — auto-detects the spec from the top-level `*_version` field and renders the appropriate view. **Eleven specs auto-detected**; five views: Visualize / Editor / Architecture / Tools / About |
| [`examples.kineticgain.com`](https://examples.kineticgain.com) | [`kinetic-gain-examples-gallery`](https://github.com/mizcausevic-dev/kinetic-gain-examples-gallery) | **Examples gallery** — sidebar of 11 specs, click any to see its canonical example rendered with JSON syntax highlighting |
| [`walker.kineticgain.com`](https://walker.kineticgain.com) | [`well-known-walker-web`](https://github.com/mizcausevic-dev/well-known-walker-web) | **well-known-walker** — paste any domain, see every Kinetic Gain disclosure document it publishes |
| [`bench.kineticgain.com`](https://bench.kineticgain.com) | [`prompt-injection-bench-web`](https://github.com/mizcausevic-dev/prompt-injection-bench-web) | **prompt-injection-bench** visual harness |

The unified visualizer + unified MCP server give the Suite a complete read-side (human) and tool-side (agent) entry point. **Eleven specs, two front doors, twenty-two live properties.**

### 🛡️ Testing companion

| Repo | What it does |
|---|---|
| [`prompt-injection-bench`](https://github.com/mizcausevic-dev/prompt-injection-bench) | **30-attack prompt-injection corpus + Python harness.** Every record back-references the Agent Card `refusal_taxonomy[].category` it tests, so a vendor can mechanically verify declared refusals hold under attack. Failed runs feed AI Incident Cards. Not a 10th spec — the *testing-counterpart* to the disclosure layer. |

---

## 🛡️ Platform Reliability Stack

Reliability primitives. Each independent. All designed to compose:

| Repo | Lang | Surface | Buyer |
|---|---|---|---|
| [`rate-limit-shield`](https://github.com/mizcausevic-dev/rate-limit-shield) | Python | Token bucket + circuit breaker + jittered retry, HTTP 429 / Retry-After awareness | **SRE** |
| [`identity-mesh`](https://github.com/mizcausevic-dev/identity-mesh) | Python | SPIFFE-style JWT-SVID broker — short-lived tokens, audience binding, zero long-lived keys | **CISO** |
| [`agent-canary`](https://github.com/mizcausevic-dev/agent-canary) | Python | Progressive rollout, shadow mode, sticky-percent routing, auto-rollback | **Platform / SRE** |
| [`model-registry-pro`](https://github.com/mizcausevic-dev/model-registry-pro) | Python | Model lifecycle catalog: lineage, stage promotion, approval gates | **Platform / MLOps** |
| [`slo-budget-tracker`](https://github.com/mizcausevic-dev/slo-budget-tracker) | Python | SLO + error-budget library, FastAPI middleware, Prometheus exporter, multi-window burn-rate alerts | **SRE** |
| [`reliability-toolkit-rs`](https://github.com/mizcausevic-dev/reliability-toolkit-rs) | **Rust** | Async Tokio primitives: token-bucket rate limiter · 3-state circuit breaker · exponential-backoff retry with jitter · bulkhead | **SRE / Platform** |
| [`feature-flag-rs`](https://github.com/mizcausevic-dev/feature-flag-rs) | **Rust** | Server-side feature flag eval — targeting rules, sticky percentage rollouts (SHA-256 bucketing, no RNG), hot reload | **Platform / SRE** |

Identity at the edge → rate limits at the model → canary at deploy → registry as source of truth → SLO budget at the API surface → Rust primitives for hot paths → feature flags for rollout control. **Defense-in-depth for the agent era.**

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

## 🧪 Decision Intelligence Engines

| Repo | Lang | What it does |
|---|---|---|
| [`procurement-decision-api`](https://github.com/mizcausevic-dev/procurement-decision-api) | Python | **First cross-ecosystem bridge in the portfolio.** Drafts AI Procurement Decision Cards from a buyer rubric and vendor Suite documents (AEO + agent-card + tool-card + ai-evidence + …). Connects [Kinetic Gain Protocol Suite](#-kinetic-gain-protocol-suite) (spec #11) with Decision Intelligence. Pydantic v2, FastAPI, httpx async, NIST AI RMF crosswalk linked from the OpenAPI spec. |
| [`policy-as-code-engine`](https://github.com/mizcausevic-dev/policy-as-code-engine) | Python | **Companion to `procurement-decision-api`.** Declarative policy evaluator — JSON/YAML rules, first-match-wins, deny-trumps-allow. Headline: `POST /bundles/from-decision-card` turns a Decision Card's conditions into a runtime-enforceable PolicyBundle. Closes the loop from "buyer signed off" to "request gated." |
| [`incident-correlation-rs`](https://github.com/mizcausevic-dev/incident-correlation-rs) | **Rust** | **Walks the Suite graph from an AI Incident Card** and emits a structured remediation plan. BFS over typed `SuiteEdge`s; `DecisionCard` → `RecheckPolicy`, `Vendor` → `RequestReview`, AEO/agent/tool → `Revalidate`. petgraph under the hood. The piece that turns "we had an incident" into "here's exactly what to touch next." |
| [`briefing-intelligence-engine`](https://github.com/mizcausevic-dev/briefing-intelligence-engine) | Python | Executive briefing scoring, narrative generation, risk ranking |
| [`signal-orchestration-lab`](https://github.com/mizcausevic-dev/signal-orchestration-lab) | Python | Dependency-aware signal routing, escalation sequencing |

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

| Repo | What it does |
|---|---|
| [`data-contract-registry`](https://github.com/mizcausevic-dev/data-contract-registry) | **Schema registry for data contracts.** Semver versioning, compatibility checks (backward / forward / full), declared owners, freshness SLAs. Bridges to `procurement-decision-api` via `POST /contracts/owners/from-decision-card` — buyer + decision_maker from a Decision Card become the contract's paging targets. **Cross-ecosystem hook #3.** |
| [`revops-database-lab`](https://github.com/mizcausevic-dev/revops-database-lab) | PostgreSQL revenue modeling lab. |
| [`revenue-intelligence-db`](https://github.com/mizcausevic-dev/revenue-intelligence-db) | Attribution + forecast + renewal-risk reporting. |
| [`cloud-cost-intelligence-dashboard`](https://github.com/mizcausevic-dev/cloud-cost-intelligence-dashboard) | Cloud cost intelligence dashboards. |

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
