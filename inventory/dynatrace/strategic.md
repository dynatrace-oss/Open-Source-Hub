# 🟢 Strategic Repositories — Dynatrace

These repositories are core to Dynatrace product delivery, declared strategic priorities, or critical customer-facing tooling.

---

## `dynatrace-operator`

**URL:** https://github.com/Dynatrace/dynatrace-operator  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 219 ⭐ | **Forks:** 166 | **Open Issues:** 14

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Kubernetes operator for automated rollout and lifecycle management of Dynatrace OneAgent, ActiveGate, and code modules across Kubernetes and OpenShift |
| **Strategic Relevance** | Core cloud-native delivery vehicle; required by every Kubernetes customer |
| **Owning Team** | Operator engineering team, Dynatrace Inc. |
| **Support Model** | ✅ **Officially supported** — Dynatrace Support team; Helm chart on public.ecr.aws |
| **Activity Level** | 🟢 Very high — active release cadence; v1.10.x in production |
| **Documentation Status** | 🟢 Full official docs at docs.dynatrace.com; SECURITY.md, HACKING.md, CONTRIBUTING.md present |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | SECURITY.md ✅; cosign-signed container images; security benchmarks documented |
| **Dependencies & Automation** | Go modules; Helm chart; OCI packaging; GitHub Actions CI; SBOM |
| **OSSF Scorecard (estimated)** | **8–9 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** |

---

## `dynatrace-configuration-as-code`

**URL:** https://github.com/Dynatrace/dynatrace-configuration-as-code  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 188 ⭐ | **Forks:** 108 | **Open Issues:** 0

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | "Monaco" CLI — automates deployment of Dynatrace configuration to one or many environments; enables GitOps/CaC workflows |
| **Strategic Relevance** | Critical for enterprise customers managing configuration at scale |
| **Support Model** | ✅ **Officially supported** (Monaco 2.0+); Docker image on Docker Hub |
| **Activity Level** | 🟢 High — 0 open issues; well-maintained |
| **Documentation Status** | 🟢 Full docs at docs.dynatrace.com; SBOM downloadable from releases |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **7–8 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** |

---

## `dynatrace-configuration-as-code-core`

**URL:** https://github.com/Dynatrace/dynatrace-configuration-as-code-core  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 5 ⭐ | **Forks:** 11 | **Open Issues:** 1

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Shared Go libraries underpinning Monaco and other CaC tooling |
| **Strategic Relevance** | High internally — foundational library |
| **Support Model** | Engineering dependency; not end-user facing |
| **Activity Level** | 🟢 Active |
| **OSSF Scorecard (estimated)** | **6–8 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** (internal library) |

---

## `dynatrace-otel-collector`

**URL:** https://github.com/Dynatrace/dynatrace-otel-collector  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 43 ⭐ | **Forks:** 28 | **Open Issues:** 5

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Dynatrace distribution of the OpenTelemetry Collector — pre-packages exporters and processors optimized for Dynatrace ingest |
| **Strategic Relevance** | High — central to Dynatrace's OTel strategy |
| **Support Model** | Community + Engineering |
| **Activity Level** | 🟢 Active |
| **OSSF Scorecard (estimated)** | **6–8 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** |

---

## `dynatrace-bindplane-otel-collector`

**URL:** https://github.com/Dynatrace/dynatrace-bindplane-otel-collector  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 1 ⭐ | **Forks:** 49 | **Open Issues:** 1

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Bindplane's distribution of the OTel Collector providing a unified collection solution — Dynatrace fork |
| **Strategic Relevance** | High — partnership with Bindplane/observIQ; key for log and telemetry collection |
| **Support Model** | Partnership / Engineering |
| **Activity Level** | 🟢 Active — 49 forks signals broad deployment |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **5–7 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** |

---

## `dynatrace-for-ai`

**URL:** https://github.com/Dynatrace/dynatrace-for-ai  
**Language:** JavaScript | **License:** Apache 2.0 | **Stars:** 120 ⭐ | **Forks:** 26 | **Open Issues:** 4

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Skills, prompts, and instructions for building AI agents on top of Dynatrace production context; integrates with MCP, DQL, Claude Code, GitHub Copilot |
| **Strategic Relevance** | Extremely high — fastest-growing active repo in the org; AI agent observability is a declared Dynatrace strategic priority |
| **Support Model** | Community / open |
| **Activity Level** | 🟢 Very high — 120 stars with rapid growth |
| **Documentation Status** | 🟡 README + topics; would benefit from structured docs |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | ⚠️ Scripts with API credentials — credential handling audit needed |
| **OSSF Scorecard (estimated)** | **5–7 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** — harden credential handling; add OSSF scorecard; elevate support model |

---

## `helm-charts`

**URL:** https://github.com/Dynatrace/helm-charts  
**Language:** Go Template | **License:** Apache 2.0 | **Stars:** 30 ⭐ | **Forks:** 45 | **Open Issues:** 3

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Official Helm Charts provided by Dynatrace — primary distribution mechanism for `dynatrace-operator` and related components |
| **Strategic Relevance** | High — distribution infrastructure for Kubernetes deployments |
| **Support Model** | Officially supported (companion to operator) |
| **Activity Level** | 🟢 Active |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **6–8 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** |

---

## `Dynatrace-OneAgent-Ansible`

**URL:** https://github.com/Dynatrace/Dynatrace-OneAgent-Ansible  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 47 ⭐ | **Forks:** 51 | **Open Issues:** 1

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Ansible role for installing Dynatrace OneAgent — primary automation path for non-Kubernetes deployments |
| **Strategic Relevance** | High — large enterprise segment still uses Ansible for bare metal and VM deployments |
| **Support Model** | Community; widely adopted |
| **Activity Level** | 🟢 Active |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **6–7 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** — evaluate for official support elevation given adoption (51 forks) |

---

## `dynatrace-configuration-as-code-samples`

**URL:** https://github.com/Dynatrace/dynatrace-configuration-as-code-samples  
**Language:** HCL | **License:** Apache 2.0 | **Stars:** 32 ⭐ | **Forks:** 25 | **Open Issues:** 2

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Sample projects demonstrating Dynatrace Configuration as Code using Terraform and Monaco — covers pipeline observability, GitLab, GitHub, ArgoCD, Azure DevOps |
| **Strategic Relevance** | High — companion to Monaco and Terraform provider; reduces customer time-to-value |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **5–7 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** |

---

## `backstage-plugin`

**URL:** https://github.com/Dynatrace/backstage-plugin  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 37 ⭐ | **Forks:** 18 | **Open Issues:** 16

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Dynatrace plugin for Backstage IDP — surfaces DT observability data in developer portals |
| **Strategic Relevance** | High — platform engineering / IDP integration; ecosystem play in CNCF toolchain |
| **Support Model** | Community |
| **Activity Level** | 🔴 Bottlenecked — 16 open issues signals under-resourcing |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **5–7 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** — assign dedicated reviewer; clear issue backlog |

---

## `swift-mobile-sdk`

**URL:** https://github.com/Dynatrace/swift-mobile-sdk  
**Language:** Swift | **License:** Apache 2.0 | **Stars:** 15 ⭐ | **Forks:** 8 | **Open Issues:** 0

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Swift Package Manager distribution of Dynatrace OneAgent for iOS and tvOS mobile monitoring |
| **Strategic Relevance** | High for mobile observability segment |
| **Support Model** | ✅ Officially supported via commercial SDK support |
| **Activity Level** | 🟢 Active |
| **OSSF Scorecard (estimated)** | **6–7 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** |

---

## `dynatrace-bootstrapper`

**URL:** https://github.com/Dynatrace/dynatrace-bootstrapper  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 3 ⭐ | **Forks:** 11 | **Open Issues:** 3

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | Sets up Dynatrace OneAgent in containers at init time; companion to the Operator |
| **Strategic Relevance** | High — part of the Operator ecosystem |
| **Support Model** | Supported via Operator support |
| **Activity Level** | 🟢 Active |
| **OSSF Scorecard (estimated)** | **6–7 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** |

---

## `bosh-oneagent-release`

**URL:** https://github.com/Dynatrace/bosh-oneagent-release  
**Language:** Ruby | **License:** MIT | **Stars:** 11 ⭐ | **Forks:** 15 | **Open Issues:** 0

| Dimension | Assessment |
| --- | --- |
| **Business / Ecosystem Purpose** | BOSH release for deploying Dynatrace OneAgent on Cloud Foundry / BOSH-managed VMs |
| **Strategic Relevance** | Medium — CF/BOSH market declining but still active in large enterprise |
| **Support Model** | Community / partner |
| **Activity Level** | 🟡 Low — periodic maintenance |
| **License Status** | ✅ MIT |
| **OSSF Scorecard (estimated)** | **4–6 / 10** |
| **Recommended Disposition** | 🟢 **Strategic** *(borderline Maintenance-Only)* — evaluate CF customer base size; downgrade if BOSH usage below threshold |
