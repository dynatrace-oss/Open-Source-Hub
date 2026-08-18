# Open Source Project Advisor

The **Open Source Project Advisor** is a guided AI experience for Dynatrace employees evaluating new or existing open source projects.

It uses the guidance in the Dynatrace Open Source Hub to help employees make better, more consistent open source decisions before they request repository creation or publication.

The advisor is designed to reduce repeated back-and-forth around questions such as:

- Should this project be open source?
- Should Dynatrace own it?
- Does the work belong upstream?
- Which GitHub organization should host it?
- What support model applies?
- Is ownership clear?
- Is the project ready for publication?
- What still needs to happen before repository creation?

---

## Operating model

```text
Idea
  ↓
Guided assessment
  ↓
Open source recommendation
  ↓
Publication readiness
  ↓
Repository request summary
  ↓
Open Source Slack request
  ↓
Governed approval and provisioning
```

The advisor supports:

**Self-service decisioning → governed repository provisioning**

The advisor does not replace the existing approval or repository provisioning process.

---

## What the advisor does

The advisor helps determine:

1. Whether a project should be open source.
2. Whether Dynatrace should own the project.
3. Whether the work would be better contributed upstream.
4. Which GitHub organization is the appropriate home.
5. Which support model applies.
6. Whether ownership and maintainer responsibility are sufficient.
7. Whether the project is ready for publication.
8. What actions remain before repository creation or publication.
9. What information should be included in the repository creation request.

---

## What the advisor does not do

The advisor does not:

- Approve repositories.
- Create repositories.
- Grant GitHub permissions.
- Authorize public release.
- Provide legal approval.
- Provide security approval.
- Replace required Dynatrace review.
- Automatically provision repositories.
- Become the technical owner or maintainer of a project.

When repository creation is the appropriate next step, the advisor prepares a structured request and directs the employee to the Dynatrace Open Source Slack channel.

---

## Files

This directory contains the configuration and validation material for the advisor.

```text
advisor/
├── README.md
├── instructions.md
└── test-scenarios.md
```

### `instructions.md`

Defines:

- Advisor role.
- Conversation behavior.
- Decision logic.
- Support-model guidance.
- Repository-placement logic.
- Publication-readiness checks.
- Final output format.
- Repository request handoff.
- Guardrails.

This file should be treated as the canonical version of the advisor instructions.

### `test-scenarios.md`

Contains representative scenarios used to validate that the advisor behaves consistently with the Open Source Hub.

Scenarios cover:

- Unowned experiments.
- Community projects.
- Officially supported components.
- Upstream contribution opportunities.
- Private-to-public transitions.
- Customer and partner projects.
- Security and licensing concerns.
- Repository placement.
- Repository readiness.

---

## Knowledge source

The **Dynatrace Open Source Hub** is the authoritative source for repository governance and open source guidance.

The advisor should use the Hub rather than inventing or independently redefining policy.

Relevant guidance includes:

### Getting started

- [How Dynatrace Approaches Open Source](../docs/getting-started/how-dynatrace-approaches-open-source.md)
- [Should This Be Open Source?](../docs/getting-started/should-this-be-open-source.md)
- [Where Does My Repository Belong?](../docs/getting-started/where-does-my-repo-belong.md)
- [Customer and Partner Guidance](../docs/getting-started/customer-and-partner-guidance.md)

### Governance

- [Repository Lifecycle](../docs/governance/repository-lifecycle.md)
- [Support Models](../docs/governance/support-models.md)
- [Contributor Access](../docs/governance/contributor-access.md)
- [Maintainer Succession](../docs/governance/maintainer-succession.md)

### Publishing

- [New Repository Requirements](../docs/publishing/new-repositories.md)
- [Private-to-Public Transition](../docs/publishing/private-to-public.md)
- [Publishing Checklist](../docs/publishing/publishing-checklist.md)
- [Repository Transfers](../docs/publishing/repository-transfers.md)

### Maintaining

- [Maintainer Guide](../docs/maintaining/maintainer-guide.md)
- [Repository Health](../docs/maintaining/repository-health.md)
- [Dependency Management](../docs/maintaining/dependency-management.md)
- [Security Readiness](../docs/maintaining/security-readiness.md)
- [OpenSSF Scorecard](../docs/maintaining/openssf-scorecard.md)

### Contributing

- [Employee Contributions](../docs/contributing/employee-contributions.md)
- [External Contributors](../docs/contributing/external-contributors.md)
- [Upstream Contributions](../docs/contributing/upstream-contributions.md)

### Retiring

- [Archive Policy](../docs/retiring/archive-policy.md)
- [Archive Checklist](../docs/retiring/archive-checklist.md)
- [Deletion Policy](../docs/retiring/deletion-policy.md)

---

## Current implementation

The initial implementation uses a Claude Project.

The Claude Project should include:

1. The relevant Open Source Hub documents as Project Knowledge.
2. The contents of [`instructions.md`](./instructions.md) as the project instructions.
3. [`test-scenarios.md`](./test-scenarios.md) as the validation set used before broader rollout.

The first version intentionally does not automate repository creation.

---

## Recommended Claude setup

### Project name

```text
Open Source Project Advisor
```

### Project description

```text
Guides Dynatrace employees through deciding whether a project should be open source, where it should live, what support model applies, and whether it is ready for publication.
```

### Project knowledge

Upload the relevant Open Source Hub Markdown files.

At minimum, include:

```text
docs/getting-started/
├── how-dynatrace-approaches-open-source.md
├── should-this-be-open-source.md
└── where-does-my-repo-belong.md

docs/governance/
├── repository-lifecycle.md
├── support-models.md
├── contributor-access.md
└── maintainer-succession.md

docs/publishing/
├── new-repositories.md
├── private-to-public.md
├── publishing-checklist.md
└── repository-transfers.md

docs/maintaining/
├── repository-health.md
└── security-readiness.md
```

Additional Hub documents may be added as the advisor expands.

---

## Starting the advisor

A user should be able to start with a simple statement such as:

> I have an idea for an open source project.

The advisor should then conduct a guided conversation.

It should not immediately return a checklist or recommendation.

The advisor should ask a small number of relevant questions at a time and adapt based on the user's answers.

---

## Expected final output

When sufficient information has been collected, the advisor should provide:

### Open Source Recommendation

Including:

- Decision.
- Recommended repository home.
- Support model.
- Readiness status.
- Reasoning.
- Ownership.
- Completed requirements.
- Outstanding requirements.
- Risks or open questions.
- One clear next step.

### Repository Request Summary

When repository creation is the appropriate next step, the advisor should also produce a summary containing:

- Proposed repository name.
- Purpose.
- Audience.
- Owning team.
- Primary maintainer.
- Backup maintainer or succession path.
- Recommended organization.
- Support model.
- License.
- External contribution expectations.
- Upstream assessment.
- Security readiness.
- Publishing readiness.
- Remaining actions.
- Additional notes.

The summary should be suitable for copying into the repository creation request.

---

## Repository creation handoff

Repository creation remains a governed process.

When the advisor determines that repository creation is the appropriate next step, it should direct the user to:

[Dynatrace Open Source Slack channel](https://dynatrace.enterprise.slack.com/archives/CJGELHH5E)

The employee should include the Repository Request Summary generated by the advisor.

The advisor must not tell the user that the repository has already been approved.

---

## Validation

Before broader rollout, test the advisor against the scenarios in:

[`test-scenarios.md`](./test-scenarios.md)

For each test, evaluate:

- Did the advisor ask useful questions?
- Did it avoid unnecessary questions?
- Did it identify blocking issues?
- Did it recommend the appropriate support model?
- Did it evaluate upstream before recommending a new repository?
- Did it avoid treating the Open Source team as the project owner?
- Did it use the Hub guidance accurately?
- Did it produce a usable final summary?
- Did it point to Slack when repository creation was the next step?

A technically polished answer that produces the wrong governance decision should be considered a failed test.

---

## Updating the advisor

Changes to advisor behavior should be made in:

```text
advisor/instructions.md
```

Recommended workflow:

```text
Proposed advisor change
        ↓
Update instructions.md
        ↓
Pull request
        ↓
Review
        ↓
Merge
        ↓
Update Claude Project instructions
        ↓
Re-run relevant test scenarios
```

Changes to repository policy should generally be made in the relevant Open Source Hub documentation first.

The advisor should follow the current Hub guidance rather than becoming an independent source of policy.

---

## Future capabilities

Potential future versions may include:

- Automatic retrieval of the latest Hub guidance.
- GitHub integration.
- Repository metadata validation.
- Existing-repository assessment.
- Automated publication-readiness checks.
- Repository inventory lookup.
- OpenSSF Scorecard retrieval.
- Repository request submission.
- Juno or GitHub-as-Code integration.
- Post-approval repository provisioning.

These capabilities should only be introduced after the advisory behavior is validated.

---

## Design principle

The advisor should make it easier for employees to arrive at the Open Source team with a complete, well-considered request.

The goal is not to remove governance.

The goal is to reduce repetitive discovery work and make governance easier to follow.

**Self-service decisioning → governed repository provisioning.**
