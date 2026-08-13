# 🔵 Active / Community-Supported Repositories — Dynatrace

Regular activity, community adoption, ongoing maintenance — not formally supported by Dynatrace support contracts unless noted.

---

## `easytrade`
**URL:** https://github.com/Dynatrace/easytrade  
**Language:** TypeScript | **Stars:** 55 ⭐ | **Forks:** 121 | **Open Issues:** 4

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | EasyTrade — microservices demo app (stock trading) for demonstrating Dynatrace observability; developed by Demoability Team |
| **Strategic Relevance** | Medium-High — primary demo application used in customer-facing HOT sessions and enablement globally |
| **Activity Level** | 🟢 Active — 121 forks indicates very wide field use |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **5–7 / 10** |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `easyTravel-Docker`
**URL:** https://github.com/Dynatrace/easyTravel-Docker  
**Language:** Shell | **Stars:** 66 ⭐ | **Forks:** 106 | **Open Issues:** 4

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace easyTravel Demo Application in Docker — the classic demo app for APM scenarios |
| **Strategic Relevance** | Medium — legacy demo; `easytrade` is the modern successor but easyTravel still used in many demo scenarios |
| **Activity Level** | 🟢 Active — 106 forks, 66 stars |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **5–6 / 10** |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — document relationship to `easytrade`; plan eventual deprecation path |

---

## `opentelemetry-demo`
**URL:** https://github.com/Dynatrace/opentelemetry-demo  
**Language:** TypeScript | **Stars:** 0 ⭐ (fork) | **Forks:** 7k

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Fork of the CNCF OpenTelemetry Astronomy Shop demo — Dynatrace variant for internal demos and HOT days |
| **Strategic Relevance** | Medium — demonstration asset; forks from upstream CNCF project |
| **Activity Level** | 🟡 Periodic syncs with upstream |
| **License Status** | ✅ Apache 2.0 |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — keep in sync with upstream; document DT-specific changes |

---

## `community-examples`
**URL:** https://github.com/Dynatrace/community-examples  
**Language:** HCL | **Stars:** 16 ⭐ | **Forks:** 10 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Community-driven collection of examples and solutions to get inspired by or use as templates for Dynatrace platform |
| **Strategic Relevance** | Medium — community enablement |
| **Activity Level** | 🟢 Active |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **4–6 / 10** |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `dt-app-templates`
**URL:** https://github.com/Dynatrace/dt-app-templates  
**Language:** JavaScript | **Stars:** 13 ⭐ | **Forks:** 8 | **Open Issues:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace App Bundle Templates for building Dynatrace platform apps (DT Platform App Framework) |
| **Strategic Relevance** | High for DT App ecosystem / partner development |
| **Activity Level** | 🟢 Active |
| **OSSF Scorecard (estimated)** | **5–6 / 10** |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `OneAgent-SDK` (conceptual)
**URL:** https://github.com/Dynatrace/OneAgent-SDK  
**Language:** Java | **Stars:** 24 ⭐ | **Forks:** 6 | **Open Issues:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Describes technical concepts of the Dynatrace OneAgent SDK — the conceptual/documentation hub for all language SDKs |
| **Strategic Relevance** | Medium — documentation hub; increasingly superseded by OTel |
| **Activity Level** | 🟡 Low-moderate |
| **OSSF Scorecard (estimated)** | **5–6 / 10** |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## OneAgent SDK Language Implementations

| Repo | Language | Stars | Forks | Status | Notes |
|---|---|---|---|---|---|
| `OneAgent-SDK-for-Java` | Java | 41 ⭐ | 15 | 🔵 Active | Widely deployed; monitor for OTel supersession |
| `OneAgent-SDK-for-Python` | Python | 28 ⭐ | 12 | 🔵 Active | Still used where OTel not yet adopted |
| `OneAgent-SDK-for-NodeJs` | TypeScript | 21 ⭐ | 5 | 🔵 Active | |
| `OneAgent-SDK-for-dotnet` | C# | 22 ⭐ | 8 | 🔵 Active | |
| `OneAgent-SDK-for-Go` | Go | 4 ⭐ | 1 | 🟠 Maintenance | Low adoption |
| `OneAgent-SDK-for-PHP` | N/A | 1 ⭐ | 0 | 🟠 Maintenance | Very low adoption |
| `OneAgent-SDK-for-C` | C | 21 ⭐ | 3 | 🔵 Active | Native apps |

**Disposition for all OneAgent SDKs:** Evaluate collectively against OTel SDK adoption. Define a clear sunset timeline and publish a migration guide to OTel instrumentation.

---

## OpenKit SDKs

| Repo | Language | Stars | Forks | Notes |
|---|---|---|---|---|
| `openkit-java` | Java | 37 ⭐ | 36 | 🔵 Active — dev program |
| `openkit-dotnet` | C# | 18 ⭐ | 17 | 🔵 Active |
| `openkit-native` | C++ | 14 ⭐ | 11 | 🔵 Active |
| `openkit-js` | TypeScript | 17 ⭐ | 10 | 🟠 Maintenance |

**Note:** OpenKit SDKs serve environments where OneAgent cannot run. Evaluate for OTel supersession.

---

## `Dynatrace-workflow-samples`
**URL:** https://github.com/Dynatrace/Dynatrace-workflow-samples  
**Stars:** 19 ⭐ | **Forks:** 16

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Samples and templates for Dynatrace Workflows — automation patterns for the DT platform |
| **Strategic Relevance** | High — Workflows is a key DT platform capability |
| **Activity Level** | 🟢 Active |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `obslab-llm-observability`
**URL:** https://github.com/Dynatrace/obslab-llm-observability  
**Language:** HTML | **Stars:** 12 ⭐ | **Forks:** 146 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | ObsLab: LLM observability hands-on demo — holiday destination advisor with Dynatrace AI Observability |
| **Strategic Relevance** | High — 146 forks is the highest fork count among active non-fork repos; signals massive HOT day usage |
| **Activity Level** | 🟢 Very active (used in training programs) |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | **4–5 / 10** |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — the fork count signals this is a flagship training repo; elevate visibility |

---

## `obslab-release-validation`
**URL:** https://github.com/Dynatrace/obslab-release-validation  
**Language:** Python | **Stars:** 3 ⭐ | **Forks:** 19 | **Open Issues:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Uses Grafana k6, Dynatrace business events, workflows, and Site Reliability Guardian to validate software releases |
| **Strategic Relevance** | Medium — quality gate / SRE automation demo |
| **Activity Level** | 🟢 Active |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## ObsLab Series (abbreviated)

All `obslab-*` repos form a structured hands-on lab program. Most are small Python/Shell repos with modest stars but consistent fork activity (indicating HOT day usage).

| Repo | Purpose | Stars | Forks | Disposition |
|---|---|---|---|---|
| `obslab-llm-observability` | LLM observability demo | 12 | 146 | 🔵 Active — flagship |
| `obslab-release-validation` | Release quality gates | 3 | 19 | 🔵 Active |
| `obslab-log-problem-detection` | Log-based problem detection | 3 | 6 | 🔵 Active |
| `obslab-predictive-kubernetes-scaling` | Predictive K8s autoscaling | 4 | 31 | 🔵 Active |
| `obslab-live-debugger-otel` | Live debugger + OTel | 3 | 4 | 🔵 Active |
| `obslab-otel-collector-data-ingest` | OTel Collector data ingest | 3 | 1 | 🔵 Active |
| `obslab-syslog` | Syslog → DT via OTel | 0 | 2 | 🟡 Experimental |
| `obslab-jmeter` | JMeter + DT integration | 0 | 2 | 🟡 Experimental |
| `obslab-k6` | Grafana k6 → DT | 1 | 3 | 🟡 Experimental |
| `obslab-unguard` | Security vulnerability detection | 0 | 1 | 🟡 Experimental |

**Recommendation:** Create a `obslab` GitHub Pages catalog or pinned README in the org linking all labs as a cohesive curriculum.

---

## `agent-nodejs`
**URL:** https://github.com/Dynatrace/agent-nodejs  
**Language:** JavaScript | **Stars:** 15 ⭐ | **Forks:** 15 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace agent for PaaS environments (Node.js) |
| **Strategic Relevance** | Medium — PaaS/Node.js deployment path |
| **Activity Level** | 🟢 Active |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `fastlane-plugin-dynatrace`
**URL:** https://github.com/Dynatrace/fastlane-plugin-dynatrace  
**Language:** Ruby | **Stars:** 15 ⭐ | **Forks:** 6 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Fastlane plugin to decode and upload symbolication files to Dynatrace — essential for iOS crash reporting |
| **Strategic Relevance** | Medium — mobile crash symbolication |
| **Activity Level** | 🟢 Active |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `Dynatrace-EventDrivenAnsible`
**URL:** https://github.com/Dynatrace/Dynatrace-EventDrivenAnsible  
**Language:** Python | **Stars:** 9 ⭐ | **Forks:** 10 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Event-Driven Ansible integration with Dynatrace — enables automated remediation triggered by Dynatrace problems |
| **Strategic Relevance** | Medium-High — AIOps automation pattern |
| **Activity Level** | 🟢 Active |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `ace-box`
**URL:** https://github.com/Dynatrace/ace-box  
**Language:** Jinja | **Stars:** 11 ⭐ | **Forks:** 8 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | ACE-Box — all-in-one Autonomous Cloud Enablement portable lab machine; includes ArgoCD, Backstage, OTel, Keptn, and Dynatrace |
| **Strategic Relevance** | Medium — field enablement / ACE program |
| **Activity Level** | 🟢 Active |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `snippets`
**URL:** https://github.com/Dynatrace/snippets  
**Language:** Python | **Stars:** 15 ⭐ | **Forks:** 21 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Useful samples and snippets for Dynatrace APIs and platform |
| **Strategic Relevance** | Low-Medium — community utility |
| **Activity Level** | 🟢 Active |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** |

---

## `ufo-esp32`
**URL:** https://github.com/Dynatrace/ufo-esp32  
**Language:** C++ | **Stars:** 18 ⭐ | **Forks:** 20 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | 2nd generation Dynatrace UFO with ESP32 microcontroller — physical LED status display for builds and deployments |
| **Strategic Relevance** | Low — fun project; distinguishes from the archived `ufo` (1st gen) |
| **Activity Level** | 🟡 Low maintenance |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** (low priority) |

---

## `demo-live-debugging`
**URL:** https://github.com/Dynatrace/demo-live-debugging  
**Language:** Go | **Stars:** 7 ⭐ | **Forks:** 12 | **Open Issues:** 26

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Live Debugging hands-on demo with Dynatrace |
| **Strategic Relevance** | Medium — Live Debugger is a key DT differentiator |
| **Activity Level** | 🔴 26 open issues — bottlenecked; needs reviewer |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** — address issue backlog urgently |

---

## `heroku-buildpack-dynatrace`
**URL:** https://github.com/Dynatrace/heroku-buildpack-dynatrace  
**Language:** Shell | **Stars:** 10 ⭐ | **Forks:** 19 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Heroku buildpack enabling application monitoring for Heroku apps |
| **Strategic Relevance** | Low-Medium — Heroku segment is declining |
| **Activity Level** | 🟡 Low |
| **Recommended Disposition** | 🔵 **Active / Community-Supported** *(borderline Maintenance-Only)* |
