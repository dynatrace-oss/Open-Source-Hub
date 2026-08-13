# OSSF Scorecard — Dynatrace Main Org

See [../dynatrace-oss-inventory/ossf-scorecard.md](../dynatrace-oss-inventory/ossf-scorecard.md) for full methodology, live query commands, and check-by-check remediation guide. This file covers estimates specific to the `Dynatrace` org.

---

## Estimated Scores — Strategic & Active Repos

| Repository | Estimated Score | Key Strengths | Key Gaps |
|---|---|---|---|
| `dynatrace-operator` | **8–9 / 10** | SECURITY.md, cosign releases, Helm, Go, official support | Verify dependency pinning in CI |
| `dynatrace-configuration-as-code` | **7–8 / 10** | SBOM, active releases, official support, Docker | Fuzzing, pinned CI deps |
| `dynatrace-otel-collector` | **6–8 / 10** | OTel upstream lineage, Go, Apache 2.0 | Security policy, fuzzing |
| `helm-charts` | **6–8 / 10** | Go Template, active, widely deployed | Signed releases for Helm |
| `dynatrace-for-ai` | **5–7 / 10** | Apache 2.0, active, fast-growing | Credential hygiene, no signed releases |
| `backstage-plugin` | **5–7 / 10** | TypeScript, Apache 2.0 | npm supply chain, SECURITY.md |
| `Dynatrace-OneAgent-Ansible` | **5–7 / 10** | Python, Apache 2.0, active | Signed releases |
| `easytrade` | **5–7 / 10** | TypeScript, Apache 2.0, active | No SECURITY.md confirmed |
| `easyTravel-Docker` | **4–6 / 10** | Shell, Apache 2.0 | No SECURITY.md |
| `dynatrace-configuration-as-code-samples` | **5–7 / 10** | HCL, Apache 2.0 | Sample code credential hygiene |
| `OneAgent-SDK-for-Java` | **6–7 / 10** | Java, Apache 2.0, Maven Central | Maintenance mode |
| `OneAgent-SDK-for-Python` | **5–6 / 10** | Python, Apache 2.0 | Maintenance mode |
| `opentelemetry-demo` | **7–8 / 10** | Inherits upstream CNCF score | Delta patches may introduce drift |
| `obslab-llm-observability` | **4–5 / 10** | HTML, Apache 2.0, active | Shell scripts; no SECURITY.md |

---

## Live Score Commands

```bash
# Score a single repo
export GITHUB_AUTH_TOKEN=<your_pat>
scorecard --repo=github.com/Dynatrace/dynatrace-operator --format=json | jq '{score: .score, checks: [.checks[] | {name: .name, score: .score}]}'

# Score all active Dynatrace public repos
gh api /orgs/Dynatrace/repos --paginate \
  | jq -r '.[] | select(.archived == false) | .full_name' \
  | xargs -P4 -I{} sh -c \
    'scorecard --repo=github.com/{} --format=json 2>/dev/null | jq --arg r "{}" "{repo: \$r, score: .score}"' \
  > dynatrace-scorecard-results.jsonl

# REST API (no token needed)
curl -s "https://api.securityscorecards.dev/projects/github.com/Dynatrace/dynatrace-operator"
```
