# 🟡 Experimental Repositories — dynatrace-oss

These repositories are new, nascent, or have not yet demonstrated sustained community adoption. They may be valuable but need investment, a defined roadmap, or further validation before promotion.

---

## `dtwiz`
**URL:** https://github.com/dynatrace-oss/dtwiz  
**Language:** Go | **License:** Apache 2.0 | **Stars:** 24 ⭐ | **Forks:** 3 | **Open Issues:** 5

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Wizard-style CLI for Dynatrace platform onboarding and initial configuration |
| **Strategic Relevance** | Medium — developer experience / onboarding |
| **Activity Level** | 🟡 Early stage |
| **OSSF Scorecard (estimated)** | 4–6 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** — define roadmap; evaluate overlap with `dtctl` |

---

## `ai-config-manager`
**URL:** https://github.com/dynatrace-oss/ai-config-manager  
**Language:** Go | **License:** MIT | **Stars:** 14 ⭐ | **Forks:** 5 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | AI-driven configuration management tool for Dynatrace |
| **Strategic Relevance** | Emerging — AI + CaC convergence is strategically interesting |
| **Activity Level** | 🟡 Early |
| **License Status** | ✅ MIT |
| **OSSF Scorecard (estimated)** | 4–6 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** — clarify scope relative to Monaco and `terraform-provider-dynatrace` |

---

## `dynatrace-snowflake-observability-agent`
**URL:** https://github.com/dynatrace-oss/dynatrace-snowflake-observability-agent  
**Language:** Python | **License:** MIT | **Stars:** 10 ⭐ | **Forks:** 2 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Streams selected Snowflake telemetry to the Dynatrace API — enables data platform observability through DT dashboards and workflows |
| **Strategic Relevance** | Medium — data platform observability is a growing use case |
| **Activity Level** | 🟡 Early |
| **License Status** | ✅ MIT |
| **OSSF Scorecard (estimated)** | 4–5 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** |

---

## `dynatrace-eks-blueprints-addon`
**URL:** https://github.com/dynatrace-oss/dynatrace-eks-blueprints-addon  
**Language:** JavaScript | **License:** Apache 2.0 | **Stars:** 1 ⭐ | **Forks:** 1 | **Open Issues:** 6

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Amazon EKS Blueprints add-on for Dynatrace — simplifies DT deployment into EKS Blueprints-managed clusters |
| **Strategic Relevance** | Medium — AWS EKS ecosystem integration; low adoption so far |
| **Activity Level** | 🟡 Early; 6 open issues with low engagement |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 3–5 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** — verify EKS Blueprints framework is still actively supported upstream before investing |

---

## `Kalm-Benchmark`
**URL:** https://github.com/dynatrace-oss/Kalm-Benchmark  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 4 ⭐ | **Forks:** 0 | **Open Issues:** 10

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Benchmark and analytics platform for evaluating Kubernetes security scanners — 235+ intentionally vulnerable manifests across 12 security categories |
| **Strategic Relevance** | Medium — security research supporting Dynatrace KSPM positioning |
| **Activity Level** | 🟡 Active PRs; low external adoption |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–6 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** |

---

## `kimera`
**URL:** https://github.com/dynatrace-oss/kimera  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 4 ⭐ | **Forks:** 0 | **Open Issues:** 4

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Kubernetes misconfiguration exploitation toolkit — for security research and demonstrating Kubernetes attack surfaces |
| **Strategic Relevance** | Niche — security research tool |
| **Activity Level** | 🟡 Active development (4 open issues) |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | ⚠️ Exploitation toolkit — dual-use risk; must include prominent responsible-use disclaimer; evaluate whether placement in a public org is appropriate |
| **OSSF Scorecard (estimated)** | 3–5 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** — add responsible-use policy immediately; evaluate org placement |

---

## `eBPF-Discovery`
**URL:** https://github.com/dynatrace-oss/eBPF-Discovery  
**Language:** C++ | **License:** Apache 2.0 | **Stars:** 21 ⭐ | **Forks:** 11 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | eBPF-based service discovery — automatically discovers services and endpoints on Linux systems |
| **Strategic Relevance** | Medium-High — eBPF service discovery is complementary to OneAgent capabilities |
| **Owning Team** | OneAgent kernel / platform team |
| **Support Model** | Community |
| **Activity Level** | 🟢 Active — reasonable star count for a C++ kernel tool |
| **License Status** | ✅ Apache 2.0 |
| **Security Readiness** | Kernel-level C++ — highest risk surface in the org; fuzzing and supply chain security critical |
| **OSSF Scorecard (estimated)** | 5–7 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** *(borderline Active)* — security review; document relationship to `nettracer-bpf` and `ebpf-common` |

---

## `honeyquest`
**URL:** https://github.com/dynatrace-oss/honeyquest  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 15 ⭐ | **Forks:** 0 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Cyber security game that asks humans to distinguish neutral, risky, and deceptive payloads — used for security awareness and honeypot research |
| **Strategic Relevance** | Low — research/educational tool; creative approach to security training |
| **Activity Level** | 🟡 Low |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–5 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** |

---

## `forge`
**URL:** https://github.com/dynatrace-oss/forge  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 0 ⭐ | **Forks:** 1 | **Open Issues:** 3

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Automated vulnerability analysis framework |
| **Strategic Relevance** | Medium — security automation tooling |
| **Activity Level** | 🟡 Very early |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 2–4 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** — needs description, README, and roadmap |

---

## `forge-artifacts`
**URL:** https://github.com/dynatrace-oss/forge-artifacts  
**Language:** Jupyter Notebook | **License:** Apache 2.0 | **Stars:** 1 ⭐ | **Forks:** 0 | **Open Issues:** 38

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Companion artifact storage for the `forge` vulnerability analysis framework |
| **Strategic Relevance** | Internal dependency on `forge` |
| **Activity Level** | ⚠️ 38 open issues is unusual for a near-zero-adoption repo — likely automated issue creation from the framework |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 2–3 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** — clarify the 38 open issues; consider making private if purely internal |

---

## `opencode-coder`
**URL:** https://github.com/dynatrace-oss/opencode-coder  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 3 ⭐ | **Forks:** 0 | **Open Issues:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | (No description available) — TypeScript repo |
| **Strategic Relevance** | Unknown — no description |
| **Activity Level** | 🟡 Unknown |
| **Recommended Disposition** | 🟡 **Experimental** — add description and README immediately; without context this is indistinguishable from abandoned code |

---

## `nutanix-observability`
**URL:** https://github.com/dynatrace-oss/nutanix-observability  
**Language:** SCSS | **License:** Apache 2.0 | **Stars:** 1 ⭐ | **Forks:** 0 | **Open Issues:** 4

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace observability integration for Nutanix hyperconverged infrastructure |
| **Strategic Relevance** | Low — niche Nutanix segment |
| **Activity Level** | 🟡 Very early |
| **OSSF Scorecard (estimated)** | 2–4 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** |

---

## `redhat-observability`
**URL:** https://github.com/dynatrace-oss/redhat-observability  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 0 ⭐ | **Forks:** 0 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Red Hat platform observability integration |
| **Strategic Relevance** | Medium — Red Hat/OpenShift is a key enterprise platform |
| **Activity Level** | 🔴 No stars, no forks, no issues — possibly unpublished |
| **Recommended Disposition** | 🟡 **Experimental** — add description; verify this is intentionally public |

---

## `dt-mcp-playground`
**URL:** https://github.com/dynatrace-oss/dt-mcp-playground  
**Language:** Shell | **License:** Apache 2.0 | **Stars:** 5 ⭐ | **Forks:** 14 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Playground/sandbox environment for experimenting with the Dynatrace MCP server |
| **Strategic Relevance** | Medium — enables developers to try `dynatrace-mcp` without full setup |
| **Activity Level** | 🟢 Active — 14 forks relative to 5 stars suggests practical use |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–5 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** |

---

## `dql-consumption-assistant`
**URL:** https://github.com/dynatrace-oss/dql-consumption-assistant  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 0 ⭐ | **Forks:** 0 | **Open Issues:** 11

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Provides insights into DQL query consumption for a Dynatrace company/tenant — cost management tooling |
| **Strategic Relevance** | Medium — cost visibility is a customer concern |
| **Activity Level** | 🟡 11 open issues, zero external adoption — very early |
| **Recommended Disposition** | 🟡 **Experimental** |

---

## `batch-configurator`
**URL:** https://github.com/dynatrace-oss/batch-configurator  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 0 ⭐ | **Forks:** 0 | **Open Issues:** 10

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Save and apply Dynatrace configurations to multiple entities in bulk |
| **Strategic Relevance** | Medium — operational efficiency tooling |
| **Activity Level** | 🟡 10 open issues, zero external adoption |
| **Recommended Disposition** | 🟡 **Experimental** — evaluate overlap with Monaco/CaC |

---

## `cross-charge`
**URL:** https://github.com/dynatrace-oss/cross-charge  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 0 ⭐ | **Forks:** 0 | **Open Issues:** 12

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Workflow actions for identifying DPS (Dynatrace Platform Subscription) cost per entity/tag — chargeback tooling |
| **Strategic Relevance** | Medium — FinOps/chargeback use case |
| **Activity Level** | 🟡 12 open issues, zero external adoption |
| **Recommended Disposition** | 🟡 **Experimental** |

---

## `dynatrace-insights-for-jira`
**URL:** https://github.com/dynatrace-oss/dynatrace-insights-for-jira  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 0 ⭐ | **Forks:** 0 | **Open Issues:** 19

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Surfaces Dynatrace observability insights within Jira — incident/problem context in tickets |
| **Strategic Relevance** | Medium — Jira is ubiquitous in enterprise; Atlassian integration play |
| **Activity Level** | 🟡 19 open issues is high for zero adoption — likely heavy internal development |
| **Recommended Disposition** | 🟡 **Experimental** — highest open issue count with no stars; needs description and public roadmap |

---

## `software-lifecycle`
**URL:** https://github.com/dynatrace-oss/software-lifecycle  
**Language:** TypeScript | **License:** Apache 2.0 | **Stars:** 0 ⭐ | **Forks:** 0 | **Open Issues:** 7

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Provides insights into end-of-life dates for software technologies, OS versions, and reports |
| **Strategic Relevance** | Medium — lifecycle management is relevant to security and compliance teams |
| **Activity Level** | 🟡 Early |
| **Recommended Disposition** | 🟡 **Experimental** |

---

## `kubernetes-topology-autoscaler`
**URL:** https://github.com/dynatrace-oss/kubernetes-topology-autoscaler  
**Language:** Java | **License:** Apache 2.0 | **Stars:** 8 ⭐ | **Forks:** 1 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Kubernetes Topology Autoscaler — builds and deploys autoscaling algorithms for stream processing applications |
| **Strategic Relevance** | Low-Medium — research/engineering tool |
| **Activity Level** | 🟡 Low |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–5 / 10 |
| **Recommended Disposition** | 🟡 **Experimental** |
