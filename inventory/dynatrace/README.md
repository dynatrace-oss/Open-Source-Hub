# Dynatrace Main Org — Public Repository Inventory

**Organization:** [github.com/Dynatrace](https://github.com/Dynatrace)  
**Total Repos (all visibility):** 403 | **Public Repos:** 294  
**Teams:** 167 | **People:** 504  
**Inventory Date:** August 13, 2026  
**Maintainer:** *(your team name here)*

> For the `dynatrace-oss` org inventory, see [Dynatrace OSS Inventory](../dynatrace-oss/).

---

## Classification Summary

| Classification | Count | Key Repos |
|---|---|---|
| 🟢 **Strategic** | 12 | `dynatrace-operator`, `dynatrace-configuration-as-code`, `dynatrace-otel-collector`, `dynatrace-for-ai`, `helm-charts`, `Dynatrace-OneAgent-Ansible`, `dynatrace-configuration-as-code-samples`, `backstage-plugin`, `dynatrace-bootstrapper`, `bosh-oneagent-release`, `swift-mobile-sdk`, `dynatrace-bindplane-otel-collector` |
| 🔵 **Active / Community-Supported** | 30 | `easytrade`, `easyTravel-Docker`, `opentelemetry-demo`, `community-examples`, `dt-app-templates`, `OneAgent-SDK-for-Java`, `OneAgent-SDK-for-Python`, `OneAgent-SDK-for-NodeJs`, `openkit-java`, `openkit-dotnet`, `OneAgent-SDK`, `agent-nodejs`, `Dynatrace-workflow-samples`, `obslab-llm-observability`, `obslab-release-validation`, `helm-charts`, `snippets`, `dynatrace-service-broker`, `demo-live-debugging`, `fastlane-plugin-dynatrace`, `Dynatrace-EventDrivenAnsible`, `k8s-problem-patterns`, `libbuildpack-dynatrace`, `heroku-buildpack-dynatrace`, `ace-box`, `ufo-esp32`, `dynatrace-configuration-as-code-core`, `dynatrace-otel-collector`, `demo-opentelemetry-patterns`, `openkit-native` |
| 🟡 **Experimental** | 18 | `otel-target-allocator`, `opentelemetry-demo-gitops`, `dynatrace-bindplane-otel-contrib`, `demo-crossplane`, `dynatrace-log-enrichment`, `obslab-*` series, `demo-*` series, `dynatrace-eda-integration`, `anomaly-simulation-service`, `dtctl-ai-bug-demo`, `livedebugger-file-coverage-dashboard`, `dynatrace-aws-platform-monitoring-s3-log-forwarder` |
| 🟠 **Maintenance-Only** | 12 | `OneAgent-SDK-for-Go`, `OneAgent-SDK-for-PHP`, `openkit-js`, `OneAgent-SDK-for-C`, `openkit-native`, `db-connection-check`, `dynatrace-log-enrichment`, `datahub`, `OneAgent-SDK-for-dotnet`, `Dynatrace-OneAgent-Ansible`, `easyTravel-Docker` (some) |
| 🔴 **Archive Candidate** | ~170 | All `Dynatrace-AppMon-*`, `DCRUM-*`, `dynatrace-oneagent-operator` ⛔, `ufo` ⛔, `superdump` ⛔, `AWSDevOpsTutorial` ⛔, `v8` ⛔, and all others already archived |
| ⚫ **Transfer or Deletion** | 8 | `datahub` (fork), `community-operators*` (upstream mirrors), `certified-operators` (upstream mirror), `redhat-marketplace-operators` (upstream mirror), `v8` (upstream mirror), `dem-license`, `Sody-scripts` |

---

## Directory Structure

```
dynatrace-main-inventory/
├── README.md                        ← This file
├── repos/
│   ├── strategic.md                 ← Strategic repos (full detail)
│   ├── active-community.md          ← Active / community-supported
│   ├── experimental.md              ← Experimental repos
│   ├── maintenance-only.md          ← Maintenance-only repos
│   ├── appmon-legacy.md             ← All Dynatrace-AppMon-* archived repos (bulk)
│   ├── archive-candidates.md        ← Non-AppMon archive candidates
│   └── transfer-deletion.md         ← Transfer or deletion candidates
├── ossf-scorecard.md                ← Scorecard estimates + live query commands
└── recommendations.md               ← Priority actions
```

---

## Quick Stats (Dynatrace org, August 2026)

| Metric | Value |
|---|---|
| Total public repos | 294 |
| Already GitHub-archived | ~170 (mostly AppMon era) |
| Active (commits in last 90 days) | ~35–40 |
| Repos with significant PR backlogs (>5) | ~8 |
| Highest star count (active) | `dynatrace-for-ai` — 120 ⭐ |
| Highest star count (archived) | `superdump` — 533 ⭐ |
| Largest fork count (non-fork repo) | `opentelemetry-demo` — 7k 🍴 |
| Repos with no description | ~15 |
| Upstream forks/mirrors (should be private or transferred) | 5 |

---

## Key Observations

**The AppMon Legacy:** The vast majority (~150+) of repos in this org are archived `Dynatrace-AppMon-*` plugins, fastpacks, and sensor packs from the pre-Dynatrace era (2012–2018). They are correctly archived but create significant noise in the org's public profile. Consider bulk-deleting the zero-adoption ones or moving to a dedicated `dynatrace-legacy` org.

**Upstream Mirrors:** Several repos (`community-operators`, `certified-operators`, `community-operators-prod`, `redhat-marketplace-operators`, `datahub`, `v8`) are forks of upstream projects with 0 stars and hundreds/thousands of forks inherited from the original. These should be private or managed as proper upstream contributions rather than public org repos.

**Strong AI Signal:** `dynatrace-for-ai` (120 ⭐, 26 forks) is now the highest-star active repo in the main org, surpassing `dynatrace-operator` (219 ⭐ but more mature/slower growth). The AI agent ecosystem repos are growing fastest.

**obslab Program:** ~15 `obslab-*` repos form a structured hands-on lab program. They are small but deliberately maintained. Consider a meta-repo or GitHub Pages site to surface them as a cohesive catalog.

---

## Classification Definitions

| Class | Criteria |
|---|---|
| 🟢 **Strategic** | Core to product delivery or declared strategic priority; high commit velocity; customer-facing |
| 🔵 **Active / Community-Supported** | Regular commits, community adoption, ongoing maintenance; not formally supported |
| 🟡 **Experimental** | New or nascent; low adoption; alpha/beta; in-progress |
| 🟠 **Maintenance-Only** | Functional but not evolving; rare commits |
| 🔴 **Archive Candidate** | No meaningful recent commits; technology deprecated; already archived or should be |
| ⚫ **Transfer or Deletion Candidate** | Upstream mirror, duplicate, abandoned, or zero-value public presence |
