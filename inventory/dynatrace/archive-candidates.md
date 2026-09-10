# 🔴 Archive Candidates & ⚫ Transfer / Deletion — Dynatrace

Non-AppMon repos that are archived, deprecated, or should be transferred/deleted.

---

## Already Archived — Non-AppMon

### `dynatrace-oneagent-operator` ⛔ ARCHIVED
**Stars:** 90 ⭐ | **Forks:** 47 | **Open Issues:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Kubernetes/OpenShift Operator for managing Dynatrace OneAgent deployments — the predecessor to `dynatrace-operator` |
| **Strategic Relevance** | ❌ Archived — officially deprecated Summer 2022; succeeded by `dynatrace-operator` |
| **Action Required** | README clearly states deprecation ✅; 2 open issues should be closed or redirected; ensure links in external docs point to `dynatrace-operator` |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `dynatrace-api` ⛔ ARCHIVED
**Language:** Python | **Stars:** 108 ⭐ | **Forks:** 85 | **Open Issues:** 9

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Python examples and scripts for Dynatrace v1 API — timeseries, problem feed, topology |
| **Strategic Relevance** | ❌ Archived — v1 API patterns superseded by DQL, platform APIs, and `api-client-python` in `dynatrace-oss` |
| **Notable Signal** | 108 stars, 85 forks — significant legacy footprint; 9 open issues need closure |
| **Action Required** | Close or redirect 9 open issues to `dynatrace-oss/api-client-python`; add notice to README |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived — close open issues |

---

### `ufo` ⛔ ARCHIVED
**Language:** JavaScript | **Stars:** 105 ⭐ | **Forks:** 24 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Visual alert/status display device for builds, CI, continuous delivery — 1st gen Dynatrace UFO controller |
| **Strategic Relevance** | ❌ Archived — superseded by `ufo-esp32` (2nd gen) |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived — add link to `ufo-esp32` in README |

---

### `superdump` ⛔ ARCHIVED
**Language:** C# | **Stars:** 533 ⭐ | **Forks:** 78 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Automated crash dump analysis service — web UI for analyzing Windows crash dumps |
| **Strategic Relevance** | ❌ Archived — standalone tool; very high stars (533) indicate genuine community value but Dynatrace is no longer maintaining |
| **Notable Signal** | Highest star count of any archived (or active) repo in the org; significant OSS footprint |
| **Action Required** | Repo is archived — issues cannot be opened. Temporarily unarchive to add a README notice inviting fork maintainers to contact `opensource@dynatrace.com`, then re-archive; or search existing forks for active candidates and link the best one from the README |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived — evaluate transfer to a community maintainer |

---

### `AWSDevOpsTutorial` ⛔ ARCHIVED
**Language:** JavaScript | **Stars:** 102 ⭐ | **Forks:** 102

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Unbreakable DevOps Pipeline Tutorial with AWS CodeDeploy, CodePipeline, Lambda, EC2 |
| **Strategic Relevance** | ❌ Archived — dated tutorial content |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `AWSMonitoringTutorials` ⛔ ARCHIVED
**Language:** JavaScript | **Stars:** 49 ⭐ | **Forks:** 35 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | AWS monitoring tutorial series |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived — close open issue |

---

### `v8` ⛔ ARCHIVED
**Language:** C++ | **Stars:** 0 ⭐ | **Forks:** 4.3k

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Official mirror of the V8 JavaScript engine Git repository |
| **Strategic Relevance** | ❌ None — upstream mirror; 4.3k forks are inherited from V8 itself |
| **Recommended Disposition** | ⚫ **Transfer or Deletion Candidate** — upstream mirror should be private or deleted; creates misleading fork count |

---

### `Dynatrace-AppMon-Docker` ⛔ ARCHIVED
**Language:** Shell | **Stars:** 64 ⭐ | **Forks:** 36 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dockerized components of Dynatrace AppMon enterprise solution |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `Mesos-Plugin` ⛔ ARCHIVED
**Stars:** 0 | **Forks:** 0

**Recommended Disposition:** ⚫ **Deletion Candidate** — Apache Mesos EOL; zero adoption |

---

### `deployment-api-mock` ⛔ ARCHIVED
**Stars:** 1 | **Forks:** 1

**Recommended Disposition:** ⚫ **Deletion Candidate** — internal test mock; no external value |

---

### `Custom-Webhook-Python` ⛔ ARCHIVED
**Stars:** 13 ⭐ | **Forks:** 10

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Example Python webhook for Dynatrace problem notifications |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ — add redirect to Dynatrace Workflows documentation |

---

### `serverless-hotday-2019` ⛔ ARCHIVED
**Stars:** 2 | **Forks:** 4

**Recommended Disposition:** 🔴 **Archive Candidate** ✅ — event material; consider deletion after 5+ years |

---

### `JMX-Extensions` ⛔ ARCHIVED
**Stars:** 14 ⭐ | **Forks:** 22 | **Open Issues:** 4

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace Platform JMX plugins |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ — close 4 open issues |

---

### `BizOpsConfigurator` ⛔ ARCHIVED
**Stars:** 21 ⭐ | **Forks:** 8

**Recommended Disposition:** 🔴 **Archive Candidate** ✅ |

---

### Other Archived (abbreviated)

| Repo | Stars | Notes |
|---|---|---|
| `Dynatrace-Config-Manager` | 18 ⭐ | Superseded by Monaco |
| `dynatrace-automation-tools` | 22 ⭐ | Superseded |
| `xk6-output-dynatrace` | 8 ⭐ | k6 extension; archived |
| `extension-automated-config` | 9 ⭐ | ActiveGate extension |
| `Dynatrace-OneAgent-Chef` | 6 ⭐ | Chef recipe |
| `quickstart-dynatrace` | 1 ⭐ | AWS Quick Start |
| `perform-2022-hotday` | 2 ⭐ | Event material — delete |
| `serverless-oneagent` | 3 ⭐ | Serverless Framework |
| `insightify` | 4 ⭐ | Open issues: 5 |
| `Dynatrace-developer-launchpad` | 0 ⭐ | Delete candidate |
| `demo-opentelemetry-cleanup` | 0 ⭐ | Redirects to new location |
| `Native-Swift-iOS-Sample-Application` | 3 ⭐ | |
| `Native-Android-Sample-Application` | 9 ⭐ | |
| `dtPocketTopology` | 4 ⭐ | iOS app; Swift |
| `OneAgent-SDK-AspectJ` | 1 ⭐ | |
| `OneAgent-SDK-Ruby-Sample-Binding` | 6 ⭐ | |
| `nodejs-agent-api` | 1 ⭐ | Moved to OneAgent-SDK-for-NodeJs |
| `diagnostics-eventflow` | 3 ⭐ | C# |
| `Dynatrace-LoadRunner-Request-Tagging` | 4 ⭐ | |
| `alyeska` | 3 ⭐ | Data Pipeline Toolkit |

---

## ⚫ Transfer or Deletion Candidates

### Upstream Forks — Classify Before Acting

These repos are forks of external upstream projects. Their large fork counts are inherited from the upstream network, not from Dynatrace's OSS community, and inflate org-level metrics.

> **Note:** Privatizing a fork permanently removes its upstream relationship and associated GitHub metadata, which could affect future contribution workflows. The correct fix for inflated metrics is to **filter by `fork: true`** when calculating community size, not to privatize. Only privatize or delete individual repos when there is a separate operational or security reason to do so.

**Recommended action:** Identify the owner and current purpose of each repo, then classify as one of:
- **Active upstream contribution fork** — keep public, ensure owner is identified
- **Automated mirror** — evaluate whether mirroring is still needed
- **Historical archive** — archive on GitHub if not already; add a note to the README
- **Unused** — candidate for deletion after owner confirmation

| Repo | Upstream | Forks (inherited) | Suspected Classification | Next Step |
|---|---|---|---|---|
| `community-operators` | OperatorHub.io | 757 | Active upstream contribution | Confirm owner; keep public |
| `community-operators-prod` | OperatorHub.io | 654 | Active upstream contribution | Confirm owner; keep public |
| `certified-operators` | Red Hat | 646 | Active upstream contribution | Confirm owner; keep public |
| `redhat-marketplace-operators` | Red Hat | 130 | Active upstream contribution | Confirm owner; keep public |
| `datahub` | DataHub Project (LinkedIn) | 3.7k | Unclear — 15 open issues | Identify owner; classify |
| `v8` | Google V8 | 4.3k | Unused mirror — already archived | Confirm no active use; deletion candidate |

**Metrics fix:** Exclude `fork: true` repos when reporting Dynatrace OSS community size. This requires no repo changes and immediately gives an accurate picture.

---

### Zero-Value Public Repos

| Repo | Notes |
|---|---|
| `Sody-scripts` | Shell; no description; 0 stars, 0 forks, 0 issues |
| `dem-license` | 1 star; no description; likely internal |
| `dynatrace-eda-integration` | 0 everything; needs description or should be private |
| `demo-opentelemetry-cleanup` | Archived; redirects only; delete |
| `Dynatrace-developer-launchpad` | Archived; 0 stars; delete |
