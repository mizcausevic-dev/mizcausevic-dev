# Miz Causevic

**Platform architecture and web engineering for enterprise B2B SaaS.** Boston, Massachusetts.
Founder of **Kinetic Gain LLC**, where I build governance tooling for the answer-engine and agent era.

Miz Causevic (Mirza Causevic). Background across IBM, CyberArk, Alteryx, Digital.ai and Gryphon.ai,
in platform engineering, identity and privileged access, and analytics workflow.

**Open to Director of Web Engineering, Principal Platform Engineering, and VP Platform Architecture
roles.** East Coast US, remote friendly.
[LinkedIn](https://www.linkedin.com/in/mirzacausevic/) · [kineticgain.com](https://kineticgain.com)

<!-- INTERNAL NOTE, does not render on the profile page.
     Two gaps a hiring manager will look for that this file cannot honestly assert yet:

     1. LEADERSHIP EVIDENCE. A six-lens fleet review grepped the previous 13,000-word version and
        found ZERO occurrences of: mentor, engineers, stakeholder, roadmap, on-call, hired, P&L.
        For a Director or VP screen that reads as a very high-leverage IC who has not yet led.
        Add two or three concrete lines to Background: team size led, what you owned, one outcome.

     2. YEARS OF EXPERIENCE. The old README said "~30 years" while the role brief says "20+".
        A screener who cross-checks distrusts every other number on the page once two disagree.
        Deliberately omitted here rather than guessed. Pick one and state it. -->

## Start here

| If you are | Go to |
|---|---|
| A developer who found `mcp-kinetic-gain` | [MCP server](#mcp-kinetic-gain) below. Install is one line |
| Evaluating the governance specs | [suite.kineticgain.com](https://suite.kineticgain.com) |
| A recruiter or hiring manager | [Background](#background) and the role note above |
| Doing security or vendor diligence | [kineticgain.com/trust/](https://kineticgain.com/trust/) |
| Looking for the full estate | [portfolio.kineticgain.com](https://portfolio.kineticgain.com) |

## mcp-kinetic-gain

One MCP server exposing every Kinetic Gain Protocol Suite spec as a callable tool, over stdio.
**v0.9.1, 75 tools, 12 specs, 172 tests passing, AGPL-3.0.**

```bash
npx -y mcp-kinetic-gain validate <files...>
```

Claude Desktop, one entry:

```json
{
  "mcpServers": {
    "kinetic-gain": {
      "command": "npx",
      "args": ["-y", "mcp-kinetic-gain"]
    }
  }
}
```

Three tools that show the shape of it:

- `aup_check_compliance` joins a Classroom AI AUP and a Student AI Disclosure into one allow or deny call.
- `decision_card_validate` enforces the full AI Procurement Decision Card conditional ruleset.
- `defensetech_vault_resolve_3axis` resolves a CUI tier, export-control status and foreign-person
  restriction tuple to the most restrictive policy that satisfies all three.

Published on [npm](https://www.npmjs.com/package/mcp-kinetic-gain) and the
[MCP Registry](https://registry.modelcontextprotocol.io), both at 0.9.1. Also listed on Glama,
PulseMCP, metatext and mcpmarket.

## What this is, and what it is not

The specs are **v0.1 drafts**. Nothing here has been certified or attested by a third party, and I do
not claim otherwise. Where you see regulatory names such as FERPA, HIPAA, DFARS or NYC Local Law 144,
they mark **which obligation a field is modelled against**. They are not a compliance claim about your
use of it.

Vertical reference implementations ship with **synthetic fixtures only**. No PHI, no student records,
no real claimant data. Tools report **conformance** against a JSON Schema, which is a structural check,
not a legal opinion.

Every repo carries its own `SECURITY.md`. That is where the scoped, checkable version of any claim lives.

## The Kinetic Gain estate

<!-- BEGIN GENERATED estate-block — replace contents with generated/github-readme-block.md from kineticgain-com-apex when canonical changes; do not hand-edit between markers -->
<!-- GENERATED from canonical.json — do not hand-edit -->
### Kinetic Gain estate

12 named platforms · 107 live properties · 17 open specs · 17 verticals

| Named platform | Repos |
|---|---|
| Kinetic Gain Protocol Suite | 12 |
| Kinetic Gain Implementation Stack | 27 |
| AEO Reference Stack | 13 |
| Agent Operations Suite | 23 |
| Platform Reliability Stack | 17 |
| Decision Intelligence | 11 |
| AI Procurement Pulse | 5 |
| HealthTech / Clinical Stack | 18 |
| Growth & Consent Operations | 20 |
| MCP Servers | 38 |
| Landing Sites | 12 |
| Frontend Showcase | 28 |

> Counts are platform cluster sizes; a repo may belong to several platforms, so they sum to 224 membership-slots.
<!-- END GENERATED estate-block -->

Those figures regenerate from `kinetic-gain-canonical.json` every six hours. They are cluster sizes,
not a repo total, because one repo can belong to several platforms. The raw public-repo count is
deliberately not a headline here: it drifts, and a wrong number costs more than a missing one.

## Proof you can run

Claims on this page are meant to be checkable in about a minute.

- **The server works.** `npx -y mcp-kinetic-gain validate <file>` against any Suite document.
- **The tests pass.** `git clone`, `npm ci`, `npm test`. 172 passing at v0.9.1.
- **The specs are real.** Each is a public repo with a JSON Schema and test vectors.
- **The disclosures are live.** Any Kinetic Gain domain serves its own `/.well-known/` documents.
- **The numbers reconcile.** The estate block above is generated, not typed.

<!-- BEGIN GENERATED security-stats-inline — content sourced from generated/security-stats-inline.md in kineticgain-com-apex; do not hand-edit between markers -->
<!-- GENERATED from canonical.json — do not hand-edit -->
Dependabot on **410 repos** · CodeQL on **98** · OpenSSF Scorecard on **52** (strict subset of CodeQL) · SHA-pinned actions across **558 `uses:` lines** (measured 2026-06-04).
<!-- END GENERATED security-stats-inline -->

## Background

Platform engineering, identity and privileged access, and analytics workflow, across IBM, CyberArk,
Alteryx, Digital.ai and Gryphon.ai. That history is why the Kinetic Gain work sits where it does:
governance, evidence and trust boundaries rather than features.

Two of the surfaces exist because I lived the problem.
[cert.kineticgain.com](https://cert.kineticgain.com) and
[jml.kineticgain.com](https://jml.kineticgain.com) are the CyberArk certification-review and the
joiner-mover-leaver lines from that history turned into working software.

Polyglot by choice, and the language is picked for the problem rather than for the list. Rust for hot
paths and cryptographic primitives, Python for the audit-stream services, TypeScript for the operator
surfaces, Go and Elixir where the concurrency model earns it.

## Selected work

Concrete, live, and checkable. Not a portfolio of screenshots.

| Surface | What it is |
|---|---|
| [suite.kineticgain.com](https://suite.kineticgain.com) | The Protocol Suite front door. Twelve specs, the full spec table, the two-front-doors model |
| [cert.kineticgain.com](https://cert.kineticgain.com) | CyberArk access-certification review turned into working software |
| [jml.kineticgain.com](https://jml.kineticgain.com) | Joiner-mover-leaver identity lifecycle, from the CyberArk years |
| [pulse.kineticgain.com](https://pulse.kineticgain.com) | Weekly self-scored procurement telemetry, signed receipts published at `/.well-known/` |
| [bench.kineticgain.com](https://bench.kineticgain.com) | A 30-attack prompt-injection corpus that back-references the refusal taxonomies it tests |

## Tech stack

The languages are ranked by how many repositories actually lead with them across the estate, not by
preference. The tooling is what genuinely ships and deploys the work.

**Languages**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Elixir](https://img.shields.io/badge/Elixir-4B275F?style=flat-square&logo=elixir&logoColor=white)
![Julia](https://img.shields.io/badge/Julia-9558B2?style=flat-square&logo=julia&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![Haskell](https://img.shields.io/badge/Haskell-5D4F85?style=flat-square&logo=haskell&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Astro](https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**Backend and data**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)

**Cloud, infra and CI/CD**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=flat-square&logo=netlify&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)

**AI and protocol**

![Anthropic Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![MCP](https://img.shields.io/badge/Model%20Context%20Protocol-000000?style=flat-square&logo=modelcontextprotocol&logoColor=white)

## Working interest

Open to **Director of Web Engineering**, **Principal Platform Engineering**, and **VP Platform
Architecture** roles at enterprise B2B SaaS companies. East Coast US time zone. Remote friendly.

[LinkedIn](https://www.linkedin.com/in/mirzacausevic/) ·
[kineticgain.com](https://kineticgain.com) ·
[Medium](https://medium.com/@mizcausevic) ·
[All repositories](https://github.com/mizcausevic-dev?tab=repositories)
