# 🔵 Active / Community-Supported Repositories — dynatrace-oss

These repositories have regular activity, community adoption signals, and ongoing maintenance — but are not formally supported by Dynatrace support contracts.

---

## `hash4j`
**URL:** https://github.com/dynatrace-oss/hash4j  
**Language:** Java | **License:** Apache 2.0 | **Stars:** 157 ⭐ | **Forks:** 15 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | High-performance Java hashing library — xxHash, MurmurHash3, FarmHash, SimHash, MinHash, consistent hashing. Used internally by Dynatrace and open-sourced for the broader Java ecosystem |
| **Strategic Relevance** | Medium — infrastructure library used beyond DT; high star count for a utility library signals genuine ecosystem value |
| **Owning Team** | Platform / infrastructure engineering |
| **Support Model** | Community OSS |
| **Activity Level** | 🟢 Active — steady commit cadence; 17+ topic tags indicating well-maintained metadata |
| **Documentation Status** | 🟢 Well-documented for a library; companion benchmark repo (`hash4j-benchmarks`) available |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | Non-cryptographic hashes — lower risk profile; no CVEs expected; Maven Central publishing implies signing |
| **OSSF Scorecard (estimated)** | 7–9 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — flagship OSS library; add OSSF Scorecard badge |

---

## `CustomerSuccess`
**URL:** https://github.com/dynatrace-oss/CustomerSuccess  
**Language:** N/A (config/notebooks) | **License:** Apache 2.0 | **Stars:** 35 ⭐ | **Forks:** 8

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Open-source solutions for customer success: SRE dashboards, adoption metrics, notebooks, AI/automation templates — helps customers get more value from Dynatrace |
| **Strategic Relevance** | Medium — post-sales enablement and adoption tooling; reduces time-to-value for customers |
| **Owning Team** | Customer Success / DevRel |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–5 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `koney`
**URL:** https://github.com/dynatrace-oss/koney  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 95 ⭐ | **Forks:** 11 | **Open Issues:** 3

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Kubernetes operator that enables deception policies — automates setup, rotation, and teardown of honeytokens and fake API endpoints for threat detection |
| **Strategic Relevance** | High for Application Security / KSPM segment; novel honeypot-as-operator approach |
| **Owning Team** | Application Security research |
| **Support Model** | Community / research |
| **Activity Level** | 🟢 Active — strong star count (95) for a security research tool |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | Security tool — must be carefully scoped; SECURITY.md recommended |
| **OSSF Scorecard (estimated)** | 6–8 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — add OSSF badge; document threat model |

---

## `unguard`
**URL:** https://github.com/dynatrace-oss/unguard  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 73 ⭐ | **Forks:** 64 | **Open Issues:** 6

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Intentionally insecure cloud-native microservices demo application — used to demonstrate Dynatrace Runtime Application Protection, KSPM, and Application Security capabilities |
| **Strategic Relevance** | High for AppSec demos; 73 stars and 64 forks indicates very broad field adoption |
| **Owning Team** | Application Security / Demoability |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active |
| **Documentation Status** | 🟡 README present — needs prominent "DO NOT RUN IN PRODUCTION" disclaimer |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | By design insecure — OSSF Scorecard does not apply in the normal sense; responsible use disclaimer required |
| **OSSF Scorecard (estimated)** | N/A — intentionally vulnerable |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — add prominent warning banner; consider a dedicated security demo landing page |

---

## `dynatrace-aws-s3-log-forwarder`
**URL:** https://github.com/dynatrace-oss/dynatrace-aws-s3-log-forwarder  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 7 ⭐ | **Forks:** 9 | **Open Issues:** 3

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Serverless architecture (AWS Lambda) to forward logs from Amazon S3 to the Dynatrace Log Ingest API — supports CloudTrail, access logs, service logs |
| **Strategic Relevance** | Medium — AWS ecosystem integration; enables S3-based log routing to DT |
| **Owning Team** | Cloud integrations |
| **Support Model** | Community |
| **Activity Level** | 🟡 Moderate — some open issues |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | IAM roles and Lambda execution context — needs IAM least-privilege deployment guide |
| **OSSF Scorecard (estimated)** | 5–7 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — add security deployment guide |

---

## `dynatrace-azure-log-forwarder`
**URL:** https://github.com/dynatrace-oss/dynatrace-azure-log-forwarder  
**Language:** Python | **License:** (not specified in view — check repo) | **Stars:** 27 ⭐ | **Forks:** 19 | **Open Issues:** 3

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Streams Azure logs from Azure Event Hub into Dynatrace Logs via Azure Function App — supports Azure Resource Logs and Azure Activity Logs |
| **Strategic Relevance** | Medium-High — Azure is a key cloud partnership |
| **Owning Team** | Cloud integrations |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active |
| **License Status** | ⚠️ Verify license file present |
| **OSSF Scorecard (estimated)** | 5–7 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — verify license; add security guide for Azure Managed Identity |

---

## `dynatrace-github-action`
**URL:** https://github.com/dynatrace-oss/dynatrace-github-action  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 36 ⭐ | **Forks:** 9 | **Open Issues:** 17 | **Open PRs:** 17

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | GitHub Action that pushes metrics and events from GitHub workflows to a Dynatrace monitoring environment — enables pipeline observability |
| **Strategic Relevance** | High — GitHub Actions is the dominant CI platform; this bridges developer workflows into DT |
| **Owning Team** | Platform / DevOps integrations |
| **Support Model** | Community |
| **Activity Level** | 🔴 Bottlenecked — 17 open issues and 17 open PRs; significant backlog |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | GitHub Actions with DT API token — SECURITY.md and token scoping guidance needed |
| **OSSF Scorecard (estimated)** | 5–7 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — PR backlog is a reputational risk; assign dedicated reviewer; this repo may warrant strategic elevation |

---

## `api-client-python`
**URL:** https://github.com/dynatrace-oss/api-client-python  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 70 ⭐ | **Forks:** 27 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace API Python client — programmatic access to the Dynatrace platform APIs from Python |
| **Strategic Relevance** | Medium-High — Python is the dominant language for automation and AI tooling; widely used by customers and partners |
| **Owning Team** | SDK / API team |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active — high star count (70) |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 6–7 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — evaluate whether this should become an officially supported SDK |

---

## `DynatraceDashboardPowerups`
**URL:** https://github.com/dynatrace-oss/DynatraceDashboardPowerups  
**Language:** JavaScript | **License:** Apache 2.0 | **Stars:** 42 ⭐ | **Forks:** 12 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Chrome Extension that boosts Dynatrace dashboard capabilities — adds features and visualizations beyond the default dashboard UI |
| **Strategic Relevance** | Medium — community productivity tool; high star count for an extension |
| **Owning Team** | Community / DevRel |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | Chrome extension — content security policy and permissions should be minimal; Chrome Web Store review applies |
| **OSSF Scorecard (estimated)** | 5–6 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `dt-ext-cli`
**URL:** https://github.com/dynatrace-oss/dt-ext-cli  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 17 ⭐ | **Forks:** 12 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Command-line utility for signing, building, and uploading Dynatrace Extensions (Extensions 2.0 framework) |
| **Strategic Relevance** | Medium — part of the Extensions ecosystem developer toolchain |
| **Owning Team** | Extensions platform team |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 5–7 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `fluent-plugin-dynatrace`
**URL:** https://github.com/dynatrace-oss/fluent-plugin-dynatrace  
**Language:** Ruby | **License:** Apache 2.0 | **Stars:** 6 ⭐ | **Forks:** 7 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Fluentd output plugin for sending logs to the Dynatrace Generic Log Ingest API v2 |
| **Strategic Relevance** | Low-Medium — Fluentd is widely used in Kubernetes logging stacks |
| **Owning Team** | Cloud integrations |
| **Support Model** | Community |
| **Activity Level** | 🟡 Low-moderate |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–6 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — monitor for OTel log pipeline supersession |

---

## `dynatrace-managed-mcp`
**URL:** https://github.com/dynatrace-oss/dynatrace-managed-mcp  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 27 ⭐ | **Forks:** 12 | **Open Issues:** 14

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | MCP server variant for Dynatrace Managed (on-premises / private cloud) deployments |
| **Strategic Relevance** | High for the Managed customer segment |
| **Owning Team** | AI Platform / OSS team |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active — 14 open issues indicates demand |
| **Security Readiness** | ⚠️ Same concerns as `dynatrace-mcp` — production tenant access; security review needed |
| **OSSF Scorecard (estimated)** | 5–6 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — consider consolidating with `dynatrace-mcp`; security review needed |

---

## `dtmgd`
**URL:** https://github.com/dynatrace-oss/dtmgd  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 10 ⭐ | **Forks:** 2 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | CLI for managing Dynatrace Managed environments — built for humans and AI agents alike |
| **Strategic Relevance** | Medium — Managed-specific companion to `dtctl` |
| **Owning Team** | Platform / OSS team |
| **Support Model** | Community |
| **Activity Level** | 🟡 Moderate |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 5–6 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — evaluate consolidation with `dtctl` |

---

## `nettracer-bpf`
**URL:** https://github.com/dynatrace-oss/nettracer-bpf  
**Language:** C++ | **License:** Apache 2.0 | **Stars:** 31 ⭐ | **Forks:** 7 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | eBPF-based module for event-driven monitoring of network traffic on Linux/Unix kernels — used by Dynatrace OneAgent and available for third-party solutions |
| **Strategic Relevance** | High — eBPF is a strategic observability technology; powers network topology in OneAgent |
| **Owning Team** | OneAgent kernel team |
| **Support Model** | Community OSS |
| **Activity Level** | 🟢 Active |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | Kernel module — supply chain risk; fuzzing and static analysis recommended |
| **OSSF Scorecard (estimated)** | 5–7 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — kernel module security review; add OSSF badge |

---

## `open-ecosystem-challenges`
**URL:** https://github.com/dynatrace-oss/open-ecosystem-challenges  
**Language:** Shell | **License:** MIT | **Stars:** 13 ⭐ | **Forks:** 59 | **Open Issues:** 4

> **Note:** Repo may also appear as `open-source-challenges` in some pages — treat as the same project.

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Recurring challenge prompts for practicing Cloud Native, OTel, AI/ML, and OSS skills — community talent-building program |
| **Strategic Relevance** | Medium — ecosystem community building and partner talent pipeline |
| **Owning Team** | Community / DevRel |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active — 59 forks signals very broad engagement relative to stars |
| **License Status** | ✅ MIT |
| **OSSF Scorecard (estimated)** | 4–5 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `intellij-idea-dql`
**URL:** https://github.com/dynatrace-oss/intellij-idea-dql  
**Language:** Java | **License:** Apache 2.0 | **Stars:** 14 ⭐ | **Forks:** 2 | **Open Issues:** 5

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Unofficial IntelliJ IDEA plugin for DQL (Dynatrace Query Language) — syntax highlighting, autocompletion, works offline without DT Notebooks |
| **Strategic Relevance** | Medium — developer productivity for DT power users on IntelliJ-based IDEs |
| **Owning Team** | Community / developer tools |
| **Support Model** | Community; unofficial |
| **Activity Level** | 🟢 Active |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–6 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — consider making official via JetBrains Marketplace |

---

## `dynatrace-metric-utils-go`
**URL:** https://github.com/dynatrace-oss/dynatrace-metric-utils-go  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 4 ⭐ | **Forks:** 0 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Go utility library for interacting with the Dynatrace Metrics v2 API |
| **Strategic Relevance** | Low-Medium — active (not archived) unlike the Java/Python/JS/dotnet equivalents |
| **Owning Team** | SDK / API team |
| **Support Model** | Community |
| **Activity Level** | 🟡 Low activity but not archived |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–6 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — monitor for OTel SDK supersession; if superseded, archive |

---

## `dt-evals`
**URL:** https://github.com/dynatrace-oss/dt-evals  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 44 ⭐ | **Forks:** 2 | **Open Issues:** 16

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | AI evaluators CLI for AI apps and agents — LLM-as-judge evaluation framework integrated with Dynatrace AI Observability |
| **Strategic Relevance** | High potential — AI eval tooling is a nascent but rapidly growing market |
| **Owning Team** | AI Observability team |
| **Support Model** | Community |
| **Activity Level** | 🟡 Active but high issue count (16) suggests early-stage instability |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 3–5 / 10 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** *(borderline Experimental)* — define roadmap; reduce issue chaos before promoting |
