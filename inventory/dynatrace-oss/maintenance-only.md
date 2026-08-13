# 🟠 Maintenance-Only Repositories — dynatrace-oss

These repositories are functional and still receiving occasional attention, but are not actively evolving. They may be candidates for archive if activity does not resume.

---

## `logstash-output-dynatrace`
**URL:** https://github.com/dynatrace-oss/logstash-output-dynatrace  
**Language:** Ruby | **License:** ⚠️ None specified | **Stars:** 7 ⭐ | **Forks:** 3 | **Open Issues:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Logstash output plugin for sending logs to Dynatrace — enables Elastic Stack log pipelines to route to Dynatrace |
| **Strategic Relevance** | Low-Medium — Logstash/Elastic Stack integration is declining relative to OTel log pipelines |
| **Owning Team** | Cloud integrations |
| **Support Model** | Community |
| **Activity Level** | 🟠 Low — periodic maintenance |
| **Documentation Status** | 🟡 Basic README |
| **License Status** | ⚠️ **No explicit license file** — violates org default of Apache 2.0; must be corrected |
| **Security Readiness** | Low risk; Ruby gem |
| **OSSF Scorecard (estimated)** | 3–5 / 10 — license gap lowers score |
| **Recommended Disposition** | 🟠 **Maintenance-Only** — add Apache 2.0 license file immediately; evaluate against OTel log forwarding alternatives; archive within 12 months if OTel supersedes |

---

## `dynatrace-metric-utils-java`
**URL:** https://github.com/dynatrace-oss/dynatrace-metric-utils-java  
**Language:** Java | **License:** Apache 2.0 | **Stars:** 3 ⭐ | **Forks:** 6 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Java utility library for interacting with the Dynatrace Metrics v2 API |
| **Strategic Relevance** | Low — the Java/Python/.NET/JS equivalents are mostly archived; this one is not yet archived but shows the same trajectory |
| **Activity Level** | 🟠 Low — open issues: 0; likely stable but unmaintained |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–6 / 10 |
| **Recommended Disposition** | 🟠 **Maintenance-Only** — evaluate for archive alongside the other `dynatrace-metric-utils-*` repos; superseded by OTel Java SDK |

---

## `dynahist`
**URL:** https://github.com/dynatrace-oss/dynahist  
**Language:** Java | **License:** Apache 2.0 | **Stars:** 51 ⭐ | **Forks:** 12 | **Open Issues:** 7

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | DynaHist — dynamic histogram library for Java; efficient approximate data distribution tracking |
| **Strategic Relevance** | Low externally — internal data structures library open-sourced; moderate stars indicate some community interest |
| **Owning Team** | Platform / infrastructure engineering |
| **Support Model** | Community |
| **Activity Level** | 🟠 Low-moderate — open issues not resolved |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 5–7 / 10 |
| **Recommended Disposition** | 🟠 **Maintenance-Only** — address open issues or explicitly mark as unmaintained |

---

## `index4j`
**URL:** https://github.com/dynatrace-oss/index4j  
**Language:** Java | **License:** Apache 2.0 | **Stars:** 18 ⭐ | **Forks:** 2 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace FM-Index library for Java — space-efficient full-text search index data structure |
| **Strategic Relevance** | Low — research/infrastructure library |
| **Activity Level** | 🟠 Low |
| **License Status** | ✅ Apache 2.0 |
| **OSSF Scorecard (estimated)** | 4–6 / 10 |
| **Recommended Disposition** | 🟠 **Maintenance-Only** |

---

## `hash4j-benchmarks`
**URL:** https://github.com/dynatrace-oss/hash4j-benchmarks  
**Language:** Python (visualization) | **License:** Apache 2.0 | **Stars:** 1 ⭐ | **Forks:** 0 | **Open Issues:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Companion benchmark results repository for `hash4j` — stores and visualizes performance benchmark data |
| **Strategic Relevance** | Low — supporting artifact for `hash4j` |
| **Activity Level** | 🟠 Low — updated only when `hash4j` benchmarks run |
| **Recommended Disposition** | 🟠 **Maintenance-Only** — consider merging into `hash4j` as a `/benchmarks` subdirectory |

---

## `bizevent-pusher`
**URL:** https://github.com/dynatrace-oss/bizevent-pusher  
**Language:** Python | **License:** Apache 2.0 | **Stars:** 5 ⭐ | **Forks:** 0 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Tool to push Dynatrace Business Events (bizevents) to the DT platform |
| **Strategic Relevance** | Low-Medium — business observability tooling |
| **Activity Level** | 🟠 Low — no open issues, no PRs |
| **License Status** | ✅ Apache 2.0 |
| **Recommended Disposition** | 🟠 **Maintenance-Only** — evaluate if this is superseded by built-in Workflow actions for bizevents |

---

## `progressiveDelivery-masterclass`
**URL:** https://github.com/dynatrace-oss/progressiveDelivery-masterclass  
**Language:** Shell | **License:** Apache 2.0 | **Stars:** 4 ⭐ | **Forks:** 12 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Materials from a Progressive Delivery masterclass — demo and lab scripts |
| **Strategic Relevance** | Low — event/training material |
| **Activity Level** | 🟠 Low — 12 forks suggests it was used in sessions |
| **Recommended Disposition** | 🟠 **Maintenance-Only** — if no further sessions planned, archive |

---

## `azure-platform-health-integration`
**URL:** https://github.com/dynatrace-oss/azure-platform-health-integration  
**Language:** Bicep | **License:** Apache 2.0 | **Stars:** 3 ⭐ | **Forks:** 2 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Azure platform health integration — forwards Azure service health events to Dynatrace |
| **Strategic Relevance** | Low-Medium — Azure health event routing |
| **Activity Level** | 🟠 Low |
| **License Status** | ✅ Apache 2.0 |
| **Recommended Disposition** | 🟠 **Maintenance-Only** — evaluate against `dynatrace-azure-log-forwarder`; may overlap |
