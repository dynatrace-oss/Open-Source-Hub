# 🟢 Strategic Repositories — dynatrace-oss

These repositories are central to Dynatrace's declared strategic priorities, have significant community adoption, and warrant elevated support and security attention.

---

## `dynatrace-mcp`
**URL:** https://github.com/dynatrace-oss/dynatrace-mcp  
**Language:** TypeScript | **License:** MIT | **Stars:** 134 ⭐ | **Forks:** 27 | **Open PRs:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | MCP (Model Context Protocol) server for Dynatrace Observability — enables AI agents (Claude, GitHub Copilot, Cline, and others) to query Dynatrace using DQL and platform APIs |
| **Strategic Relevance** | 🔴→🟢 Extremely high. AI agent/MCP integration is a declared Dynatrace strategic priority. 134 stars signals very rapid community adoption for a new repo |
| **Owning Team** | AI Platform / OSS team |
| **Named Maintainers** | Not publicly listed |
| **Support Model** | Community — not officially supported |
| **Activity Level** | 🟢 Very active — top repo in org by star velocity |
| **Documentation Status** | 🟡 README + topic tags; would benefit from hardened setup guide and security considerations page |
| **License Status** | ✅ MIT |
| **Security Readiness** | ⚠️ HIGH PRIORITY — MCP server with direct access to production Dynatrace tenants. Authentication model, credential scope, and prompt-injection attack surface must be formally reviewed before broader adoption |
| **Dependencies & Automation** | TypeScript/npm; MCP SDK; GitHub Actions CI assumed |
| **OSSF Scorecard (estimated)** | 5–7 / 10 — fast-moving; no confirmed signed releases; security policy needed |
| **Recommended Disposition** | 🟢 **Strategic** — elevate support model; conduct urgent security review; consider promoting to main `Dynatrace` org |

---

## `terraform-provider-dynatrace`
**URL:** https://github.com/dynatrace-oss/terraform-provider-dynatrace  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 95 ⭐ | **Forks:** 41 | **Open PRs:** 5

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Official Dynatrace Terraform provider — enables infrastructure-as-code configuration of all Dynatrace platform resources via the Terraform Registry |
| **Strategic Relevance** | Very high — the primary IaC path for customers using Terraform; officially supported; listed in Terraform Registry as verified publisher |
| **Owning Team** | Dynatrace Inc. (officially supported) |
| **Named Maintainers** | Not public-facing; managed by DT engineering |
| **Support Model** | ✅ **Officially supported** — Dynatrace Support team; Terraform Registry verified publisher |
| **Activity Level** | 🟢 High — regular releases; v1.89+ in production use |
| **Documentation Status** | 🟢 Full Terraform Registry documentation; credential handling guidance in companion samples repo |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | Go provider; credential handling documented (OAuth preferred; no TF variables for secrets); Terraform Registry validation applies |
| **Dependencies & Automation** | Go modules; Terraform Plugin SDK; GitHub Actions |
| **OSSF Scorecard (estimated)** | 7–9 / 10 — Terraform Registry verified, official support, mature Go codebase |
| **Recommended Disposition** | 🟢 **Strategic** — should be promoted to the main `Dynatrace` org to reflect official support status; add OSSF Scorecard badge |

---

## `dtctl`
**URL:** https://github.com/dynatrace-oss/dtctl  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 176 ⭐ | **Forks:** 60 | **Open Issues:** 8 | **Open PRs:** 8 (estimated)

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | CLI for managing Dynatrace platform resources — built for both humans and AI agents alike; interfaces with DQL, DT APIs, and automation workflows |
| **Strategic Relevance** | High — top star count in the OSS org (176); developer experience + AI-agent tooling intersection |
| **Owning Team** | Platform / OSS team |
| **Named Maintainers** | Not public |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active — high fork count (60) indicates broad use |
| **Documentation Status** | 🟡 README + topic tags; Homebrew tap available |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | CLI with API credentials; manageable risk surface; credential handling needs documentation |
| **Dependencies & Automation** | Go modules; distributed via `dynatrace-oss/homebrew-tap` |
| **OSSF Scorecard (estimated)** | 6–8 / 10 |
| **Recommended Disposition** | 🟢 **Strategic** — add OSSF Scorecard badge; consider official support path given adoption level, dtctl and dtmgd should remain separate because:They serve different customer bases (different products),They address different APIs — a single CLI for both would create confusing UX, Maintenance and governance are harder when maintained by different teams `dtctl` | |

---

## `dynatrace-ai-agent-instrumentation-examples`
**URL:** https://github.com/dynatrace-oss/dynatrace-ai-agent-instrumentation-examples  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 88 ⭐ | **Forks:** 25 | **Open Issues:** 15 | **Open PRs:** 15

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | OpenTelemetry instrumentation examples for AI apps and agents (Python, TypeScript); demonstrates Dynatrace AI Observability integration patterns |
| **Strategic Relevance** | Very high — GenAI observability is a key Dynatrace growth area; this is the primary reference implementation |
| **Owning Team** | AI Observability team |
| **Named Maintainers** | Not public |
| **Support Model** | Community |
| **Activity Level** | 🟢 Very active — 15 open PRs signals high contributor interest but bottleneck in review capacity |
| **Documentation Status** | 🟡 README + topic tags; examples-driven structure |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | ⚠️ Python examples — credential handling in examples must be audited; no hardcoded secrets check confirmed |
| **Dependencies & Automation** | Python pip; TypeScript npm; OTel SDK dependencies |
| **OSSF Scorecard (estimated)** | 5–7 / 10 |
| **Recommended Disposition** | 🟢 **Strategic** — increase reviewer bandwidth urgently; audit example credential patterns; add OSSF badge |

---

## `dynatrace-gcp-monitor`
**URL:** https://github.com/dynatrace-oss/dynatrace-gcp-monitor  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 40 ⭐ | **Forks:** 29 | **Open Issues:** 18 | **Open PRs:** 18

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace integration for Google Cloud Platform monitoring — ingests GCP metrics and logs into Dynatrace via Cloud Functions / Cloud Run |
| **Strategic Relevance** | High — GCP is a key cloud partnership; this is the primary integration mechanism for GCP customers |
| **Owning Team** | Cloud integrations team |
| **Named Maintainers** | Not public |
| **Support Model** | Community |
| **Activity Level** | 🔴 Bottlenecked — 18 open PRs and 18 open issues indicates significant under-resourcing relative to demand |
| **Documentation Status** | 🟡 README-level |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | GCP IAM roles and service accounts involved; deployment security guide needed |
| **Dependencies & Automation** | Python; GCP Cloud Functions/Cloud Run; GitHub Actions |
| **OSSF Scorecard (estimated)** | 5–7 / 10 |
| **Recommended Disposition** | 🟢 **Strategic** — critically needs dedicated reviewer; PR backlog is a reputational risk given the GCP partnership; evaluate for official support |
