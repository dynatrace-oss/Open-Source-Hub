# ⚫ Transfer or Deletion Candidates — dynatrace-oss

These repositories have no meaningful external purpose in their current state. Recommended actions are deletion, transfer to a more appropriate owner, or conversion to private.

---

## `ufo-java-wrapper` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/ufo-java-wrapper  
**Language:** Java | **License:** Apache 2.0 | **Stars:** 2 ⭐ | **Forks:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Java wrapper for the Dynatrace UFO API — the UFO is a physical LED lighting device used to show build/deployment status |
| **Strategic Relevance** | ❌ None — the Dynatrace UFO device appears to be discontinued |
| **Activity Level** | 🔴 Archived; zero forks |
| **Recommended Action** | **Delete** — the UFO device is EOL; no users; zero forks |
| **Recommended Disposition** | ⚫ **Transfer or Deletion Candidate** |

---

## `vercel-integration`
**URL:** https://github.com/dynatrace-oss/vercel-integration  
**Language:** (undetected) | **License:** (unspecified) | **Stars:** 0 ⭐ | **Forks:** 0 | **Open Issues:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Unknown — no description; no detectable language |
| **Strategic Relevance** | Unknown |
| **Activity Level** | 🔴 Zero signals of any kind |
| **Recommended Action** | **Make private or delete** — a public repo with no description, no license, no stars, and no issues is indistinguishable from abandoned scaffolding; adds noise to the org's public profile |
| **Recommended Disposition** | ⚫ **Transfer or Deletion Candidate** |

---

## `dynatrace-oss.github.io`
**URL:** github.com/ dynatrace-oss/dynatrace-oss.github.io  
**Language:** HTML | **License:** (unspecified) | **Stars:** 0 ⭐ | **Forks:** 0 | **Open Issues:** 0
⚫ Deleted

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | GitHub Pages site for the dynatrace-oss organization |
| **Strategic Relevance** | Low — the landing page at `dynatrace-oss.github.io` is the public face of the OSS org, but appears to be empty or unmaintained |
| **Activity Level** | 🔴 Zero adoption signals |
| **Recommended Action** | **Invest or delete** — either build this into a meaningful OSS landing page (portfolio, links to key repos, contribution guide) or remove it. An empty GitHub Pages site is worse than no site |
| **Recommended Disposition** | ⚫ Deleted 09/15/26|

---

## `oss-repository-template` (Public template)
**URL:** https://github.com/dynatrace-oss/oss-repository-template  
**Language:** (undetected) | **Stars:** 0 ⭐ | **Forks:** 0 | **Open Issues:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Template repository for new open-source projects at Dynatrace |
| **Strategic Relevance** | Medium *if actively used* — a good template enforces SECURITY.md, LICENSE, CONTRIBUTING, and CI from day one |
| **Activity Level** | 🔴 Zero forks from the template; 1 open issue |
| **Recommended Action** | **Invest or deprecate in favor of `template-project`** — two template repos exist (`oss-repository-template` and `template-project`); consolidate to one, update it with org defaults (Apache 2.0, OSSF Scorecard workflow, Dependabot config), and delete the other |
| **Recommended Disposition** | ⚫ **Transfer or Deletion Candidate** *(consolidate with `template-project`)* |

---

## `template-project` (Public template)
**URL:** https://github.com/dynatrace-oss/template-project  
**Language:** Makefile | **License:** Apache 2.0 | **Stars:** 0 ⭐ | **Forks:** 5

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Template repository for open-source projects at Dynatrace — provides Makefile-based project structure |
| **Strategic Relevance** | Medium *if actively used* — 5 forks suggests some use |
| **Activity Level** | 🟡 Low — no stars but 5 forks from the template |
| **Recommended Action** | **Consolidate** — merge the best elements of `oss-repository-template` and `template-project` into one canonical template; the winning template should include: Apache 2.0 license, SECURITY.md, CONTRIBUTING.md, CODE_OF_CONDUCT.md, Dependabot config, OSSF Scorecard GitHub Action, and a README template |
| **Recommended Disposition** | ⚫ **Transfer or Deletion Candidate** *(consolidate into one template)* |

---

## Other Zero-Signal Repos to Review

The following repos had no description, no stars, no forks, and no open issues at inventory time. They should be reviewed by their creating team and either populated with content or made private/deleted:

| Repo | Language | Notes |
|---|---|---|
| `ebpf-common` | C | Described as shared code between `nettracer-bpf` and `eBPF-Discovery` — if internal utility only, consider making private |
| `rampart-api` | Java | No description; 0 stars, 0 forks |
| `rampart-spec` | (undetected) | No description; 0 stars, 0 forks |
| `rampart-antlr` | Java | No description; 0 stars, 0 forks — the three `rampart-*` repos appear to be a suite; document or consolidate |
| `BusinessObservability-DBExtension` | Python | No description; 0 stars, 0 forks, 0 issues — possibly a private project accidentally made public |
| `nvidia-observability` | (undetected) | No description; 0 stars, 0 forks — evaluate if still active |
| `open-ecosystem-challenge-verifier` | JavaScript | GitHub Action for verifying challenge solutions — companion to `open-ecosystem-challenges`; 0 stars, 0 forks |
