# OSSF Scorecard — dynatrace-oss

[OSSF Scorecard](https://github.com/ossf/scorecard) evaluates open-source repositories across security best practices. Scores are out of 10.

> **Live scores** were not retrieved directly at inventory time. The estimates below are derived from publicly observable signals (SECURITY.md presence, signed releases, CI/CD, license, branch protection indicators, activity). Obtain live scores using the methods below.

---

## How to Get Live Scores

### Single Repo (CLI)

```bash
# Install
brew install scorecard   # macOS
# or: go install sigs.k8s.io/scorecard/v4@latest
export GITHUB_AUTH_TOKEN=<your_pat>
scorecard --repo=github.com/dynatrace-oss/dynatrace-mcp --format=json | jq '{score: .score, checks: [.checks[] | {name: .name, score: .score}]}'
```

### All dynatrace-oss Public Repos (Batch)

```bash
gh api /orgs/dynatrace-oss/repos --paginate \
  | jq -r '.[] | select(.archived == false) | .full_name' \
  | xargs -P4 -I{} sh -c \
    'scorecard --repo=github.com/{} --format=json 2>/dev/null | jq --arg r "{}" "{repo: \$r, score: .score}"' \
  > scorecard-results.jsonl
```

### REST API (No Token Required for Public Repos)

```bash
curl -s "https://api.securityscorecards.dev/projects/github.com/dynatrace-oss/dynatrace-mcp" | jq '{score: .score, date: .date}'
```

### Add Scorecard as a GitHub Action (Recommended)
Add this to `.github/workflows/scorecard.yml` in each repo:
```yaml
name: Scorecard supply-chain security
on:
  branch_protection_rule:
  schedule:
    - cron: '0 6 * * 1'  # Every Monday
  push:
    branches: [main]

permissions: read-all

jobs:
  analysis:
    name: Scorecard analysis
    runs-on: ubuntu-latest
    permissions:
      security-events: write
      id-token: write
    steps:
      - uses: actions/checkout@v4
        with:
          persist-credentials: false
      - uses: ossf/scorecard-action@v2.4.0
        with:
          results_file: results.sarif
          results_format: sarif
          publish_results: true
      - uses: actions/upload-artifact@v4
        with:
          name: SARIF file
          path: results.sarif
      - uses: github/codeql-action/upload-sarif@v3
        with:
          sarif_file: results.sarif
```

---

## Estimated Scores by Repository

Scores are estimated based on observable signals. Confidence is noted where signals were limited.

| Repository | Estimated Score | Confidence | Key Strengths | Key Gaps |
|---|---|---|---|---|
| `terraform-provider-dynatrace` | **8–9** | High | Terraform Registry verified, Go, official support, Apache 2.0 | Dependency pinning confirmation |
| `hash4j` | **7–9** | High | Maven Central, CI, Apache 2.0, active, stable releases | Fuzzing not documented |
| `dtctl` | **6–8** | Medium | Go, Apache 2.0, Homebrew, active | Signed releases not confirmed, SECURITY.md not confirmed |
| `dynatrace-mcp` | **5–7** | Medium | Active, MIT, CI assumed | No signed releases, security policy urgently needed, fast-moving |
| `dynatrace-ai-agent-instrumentation-examples` | **5–7** | Medium | Apache 2.0, active, OTel standard | PR backlog, credential hygiene in examples |
| `koney` | **6–8** | Medium | Go, Apache 2.0, active, security-focused | SECURITY.md for a security tool is critical |
| `api-client-python` | **6–7** | Medium | Apache 2.0, active | Python dependency pinning |
| `dynatrace-gcp-monitor` | **5–7** | Medium | Apache 2.0, active | PR backlog, IAM security guide missing |
| `dynatrace-aws-s3-log-forwarder` | **5–7** | Medium | Apache 2.0, serverless | IAM security guide missing |
| `dynatrace-azure-log-forwarder` | **5–7** | Medium | Active, cloud integration | License confirmation needed |
| `nettracer-bpf` | **5–7** | Medium | Apache 2.0, C++, active | Kernel module — fuzzing, supply chain |
| `dynatrace-github-action` | **5–7** | Medium | Apache 2.0, TypeScript | Token scoping docs, PR backlog |
| `unguard` | **N/A** | N/A | Intentionally insecure — scorecard not applicable | Add prominent warning banner |
| `dynatrace-managed-mcp` | **5–6** | Low | Active, TypeScript | Fast-moving; same concerns as `dynatrace-mcp` |
| `DynatraceDashboardPowerups` | **5–6** | Medium | JavaScript, Apache 2.0 | Chrome extension scope audit |
| `dt-evals` | **3–5** | Low | TypeScript, Apache 2.0 | Early-stage; many open issues |
| `eBPF-Discovery` | **5–7** | Medium | C++, Apache 2.0 | Kernel module — highest risk surface |
| `kimera` | **3–5** | Low | Apache 2.0 | Exploitation toolkit — responsible use policy missing |
| `logstash-output-dynatrace` | **4–6** | Medium | Apache 2.0 (gemspec), Ruby plugin | No SECURITY.md; low activity |
| `CustomerSuccess` | **4–5** | Low | Apache 2.0 | Mixed content types; limited CI signals |
| `forge` | **2–4** | Low | Apache 2.0 | Very new; no description; limited signals |

---

## Scorecard Check Explanations

| Check | What It Tests | How to Fix |
|---|---|---|
| **Branch-Protection** | Default branch requires reviews before merge | Enable branch protection with required reviews |
| **CI-Tests** | CI runs on PRs | Add GitHub Actions workflow that runs tests on PR |
| **Code-Review** | PRs require code review before merge | Enforce review requirements in branch protection |
| **Contributors** | Diverse contributors over past 90 days | Organic — recruit external contributors |
| **Dangerous-Workflow** | No `pull_request_target` without pinning | Audit workflow files |
| **Dependency-Update-Tool** | Dependabot or Renovate configured | Add `.github/dependabot.yml` |
| **Fuzzing** | Fuzz testing present | Integrate OSS-Fuzz or local fuzzing |
| **License** | License file present | Add `LICENSE` file (Apache 2.0 for DT default) |
| **Maintained** | Commits in last 90 days | Keep repos active or archive them |
| **Pinned-Dependencies** | CI workflow steps use pinned SHAs | Pin `uses: actions/checkout@<SHA>` not `@v4` |
| **SAST** | Static analysis tool runs on commits | Add CodeQL or similar SAST workflow |
| **Security-Policy** | `SECURITY.md` present | Add `SECURITY.md` with vulnerability reporting instructions |
| **Signed-Releases** | Releases are signed (cosign, GPG) | Implement cosign signing in release workflow |
| **Token-Permissions** | Workflows use minimal token permissions | Add `permissions: read-all` to workflow files |
| **Vulnerabilities** | No unfixed vulnerabilities in OSV | Ensure Dependabot alerts are triaged |

---

## Priority Scorecard Actions for dynatrace-oss

### Immediate (all repos, 1 week)
1. Add `SECURITY.md` to every Strategic and Active repo — this alone closes the Security-Policy check
2. Add `permissions: read-all` to all GitHub Actions workflows — closes Token-Permissions
3. Add `SECURITY.md` to `logstash-output-dynatrace` — closes Security-Policy check

### Short Term (1 month)
4. Add Dependabot config (`.github/dependabot.yml`) to Strategic repos — closes Dependency-Update-Tool
5. Pin all workflow steps to SHA — closes Pinned-Dependencies
6. Add CodeQL or similar SAST to Strategic repos — closes SAST

### Medium Term (3 months)
7. Implement cosign signing for Strategic repo releases — closes Signed-Releases
8. Enable Scorecard GitHub Action on all repos — surfaces score in Security tab and badges in READMEs
9. Add fuzzing for `nettracer-bpf` and `eBPF-Discovery` — kernel modules are highest risk
