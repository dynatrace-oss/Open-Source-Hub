
# Dynatrace OSS Public Repository Inventory

**Organization:** [github.com/dynatrace-oss](https://github.com/dynatrace-oss)  
**Total Public Repos:** 95  
**Inventory Date:** August 13, 2026  
**Maintainer:** *(your team name here)*

---

## About This Inventory

This directory provides a structured assessment of every public repository in the `dynatrace-oss` GitHub organization. Each repo is evaluated across 11 dimensions and assigned a classification to guide governance decisions.

> **Note:** The `Dynatrace` main org (289 repos) is tracked separately. See [../dynatrace-main/](../dynatrace-main/) if that directory exists alongside this one.

---

## Classification Summary

| Classification | Count | Repos |
|---|---|---|
| 🟢 **Strategic** | 5 | `dynatrace-mcp`, `terraform-provider-dynatrace`, `dtctl`, `dynatrace-ai-agent-instrumentation-examples`, `dynatrace-gcp-monitor` |
| 🔵 **Active / Community-Supported** | 18 | `hash4j`, `CustomerSuccess`, `unguard`, `koney`, `nettracer-bpf`, `dynatrace-aws-s3-log-forwarder`, `dynatrace-azure-log-forwarder`, `dynatrace-github-action`, `api-client-python`, `DynatraceDashboardPowerups`, `dt-ext-cli`, `fluent-plugin-dynatrace`, `dynatrace-managed-mcp`, `dtmgd`, `dt-evals`, `open-ecosystem-challenges`, `intellij-idea-dql`, `dynatrace-metric-utils-go` |
| 🟡 **Experimental** | 20 | `dtwiz`, `dt-evals`, `ai-config-manager`, `dynatrace-snowflake-observability-agent`, `dynatrace-eks-blueprints-addon`, `Kalm-Benchmark`, `kimera`, `eBPF-Discovery`, `honeyquest`, `forge`, `opencode-coder`, `nutanix-observability`, `redhat-observability`, `dt-mcp-playground`, `dql-consumption-assistant`, `batch-configurator`, `cross-charge`, `dynatrace-insights-for-jira`, `software-lifecycle`, `kubernetes-topology-autoscaler` |
| 🟠 **Maintenance-Only** | 8 | `logstash-output-dynatrace`, `dynatrace-metric-utils-java`, `dynahist`, `index4j`, `hash4j-benchmarks`, `bizevent-pusher`, `progressiveDelivery-masterclass`, `azure-platform-health-integration` |
| 🔴 **Archive Candidate** | 22 | `barista`, `OneAgent-SDK-Python-AutoInstrumentation`, `dynatrace-aws-log-forwarder`, `opentelemetry-metric-python`, `opentelemetry-metric-java`, `opentelemetry-metric-dotnet`, `opentelemetry-metric-go`, `opentelemetry-metric-js`, `db-load-generator`, `invadium`, `jmeter-dynatrace-plugin`, `dynatrace-metric-utils-dotnet`, `dynatrace-metric-utils-python`, `dynatrace-metric-utils-js`, `kached-properties`, `junit-jupiter-open-telemetry-extension`, `ebpf-dump`, `aws-health-events-integration`, `rautee`, `dt-awslayertool`, `PTC-Windchill`, `log4j-metadata-provider` |
| ⚫ **Transfer or Deletion Candidate** | 5 | `ufo-java-wrapper`, `vercel-integration`, `dynatrace-oss.github.io`, `oss-repository-template` *(promote to active)*, `template-project` |

---

## Directory Structure

```
dynatrace-oss-inventory/
├── README.md                        ← This file (index + summary)
├── repos/
│   ├── strategic.md                 ← Strategic repos (full detail)
│   ├── active-community.md          ← Active / community-supported repos
│   ├── experimental.md              ← Experimental repos
│   ├── maintenance-only.md          ← Maintenance-only repos
│   ├── archive-candidates.md        ← Archive candidates
│   └── transfer-deletion.md         ← Transfer or deletion candidates
├── ossf-scorecard.md                ← OSSF Scorecard estimates + how to get live scores
└── recommendations.md               ← Priority actions across the full portfolio
```

---

## Evaluation Dimensions

Each repository is assessed across:

1. **Business / Ecosystem Purpose** — what problem does it solve?
2. **Strategic Relevance** — how critical is it to Dynatrace's direction?
3. **Owning Team** — who is responsible?
4. **Named Maintainers** — who are the individuals?
5. **Support Model** — official, community, or none?
6. **Activity Level** — commit cadence, open issues/PRs
7. **Documentation Status** — README, docs site, examples
8. **License Status** — type and compliance
9. **Security Readiness** — SECURITY.md, signed releases, vulnerability handling
10. **Dependencies & Automation** — package managers, CI/CD, publishing
11. **Recommended Disposition** — classification and next action

---

## Classification Definitions

| Class | Criteria |
|---|---|
| 🟢 **Strategic** | Core to product delivery or declared strategic priority; high commit velocity; customer-facing impact |
| 🔵 **Active / Community-Supported** | Regular commits, active issues/PRs, community adoption; not formally supported |
| 🟡 **Experimental** | New or nascent; low adoption; high PR-to-commit ratio; alpha/beta state |
| 🟠 **Maintenance-Only** | Rare commits; functional but not evolving; low issue activity |
| 🔴 **Archive Candidate** | No meaningful recent commits; technology deprecated or superseded; GitHub `archived` flag set or warranted |
| ⚫ **Transfer or Deletion Candidate** | Duplicate, abandoned, technology EOL confirmed, or zero external usage signals |

---

## Quick Stats (dynatrace-oss, August 2026)

| Metric | Value |
|---|---|
| Total public repos | 95 |
| Already archived by GitHub | 22 |
| Active (commits in last 90 days) | ~35 |
| Repos with open PR backlogs (>5 PRs) | ~12 |
| Highest star count | `dtctl` — 176 ⭐ |
| Highest fork count | `barista` (archived) — 74 🍴 |
| Repos with no description | ~8 |
| Repos with no license file | 1 (`logstash-output-dynatrace`) |

---

*Inventory maintained by *(your team)*. To update, follow the process in [recommendations.md](recommendations.md).*
