# Open Source Governance

This document defines the governance framework for Dynatrace-managed open
source repositories.

It explains how ownership, decision-making, support, publication, maintenance,
security, contribution, and retirement responsibilities are structured across
the Dynatrace open source portfolio.

Detailed operational guidance is maintained in the
[Dynatrace Open Source Hub](./docs/getting-started/overview.md).

---

## Purpose

Dynatrace participates in open source to:

- Contribute to and strengthen the broader technology ecosystem.
- Support interoperability and open standards.
- Enable customers, partners, developers, and contributors.
- Collaborate upstream where shared stewardship creates greater value.
- Develop useful technology transparently when public development is the
  appropriate model.

Public repositories should exist for a clear reason.

The goal is not to maximize the number of open source repositories.

The goal is to maintain a healthy, understandable, and sustainable open source
portfolio.

---

## Scope

This governance framework applies to public open source repositories managed by
Dynatrace, including repositories in:

- `Dynatrace`
- `dynatrace-oss`

It covers:

- New repository proposals.
- Private-to-public transitions.
- Repository ownership.
- Maintainer responsibility.
- Support models.
- Contributor access.
- Repository transfers.
- Repository lifecycle decisions.
- Archival and deletion.
- Security readiness.
- Portfolio governance.

Internal-only approval systems, infrastructure, escalation paths, and access
management processes may be documented separately in internal Dynatrace
systems.

---

## Governance principles

### Public by purpose

Repositories should be public because public development creates meaningful
value, not simply because the code can be published.

Before publication, teams should be able to explain:

> What becomes better because this project is open source?

See
[Should This Be Open Source?](./docs/getting-started/should-this-be-open-source.md).

### Clear ownership

Every active repository must have an identifiable owner.

At minimum, an active repository should have:

- An owning team.
- A primary maintainer or maintainers.
- A backup maintainer or documented succession path.

The Open Source team is not the default technical owner of public projects.

See
[Maintainer Succession](./docs/governance/maintainer-succession.md).

### Sustainable stewardship

Publishing a repository creates an ongoing stewardship obligation.

Teams should consider:

- Maintenance capacity.
- Release responsibility.
- Dependency management.
- Security response.
- Issue and pull request review.
- Documentation.
- Community expectations.
- Long-term ownership.

Projects should not be published without a realistic path for continued
stewardship.

### Explicit support

Repository ownership and support status are separate decisions.

A repository being owned by Dynatrace does not automatically mean it is
officially supported.

Support expectations must be documented clearly.

See [Support Models](./docs/governance/support-models.md).

### Upstream before unnecessary downstream ownership

When functionality naturally belongs in an existing upstream project,
community, or foundation, upstream contribution should be evaluated before a
new Dynatrace-owned repository is created.

Dynatrace should avoid unnecessary long-lived forks or duplicate ecosystem
projects where shared upstream stewardship is viable.

See
[Upstream Contributions](./docs/contributing/upstream-contributions.md).

### Review rather than abandon

Repositories that are no longer actively developed should move through an
explicit lifecycle decision.

Possible outcomes include:

- Continue active development.
- Move to maintenance-only.
- Transfer ownership.
- Archive.
- Delete in limited circumstances.

Repositories should not simply become abandoned without a documented
disposition.

See
[Repository Lifecycle](./docs/governance/repository-lifecycle.md).

---

## Roles and responsibilities

### Open Source team

The Open Source team owns the open source governance framework.

Its responsibilities include:

- Maintaining open source policy and guidance.
- Defining repository governance standards.
- Supporting repository publication and lifecycle decisions.
- Coordinating public GitHub organization governance.
- Helping teams evaluate appropriate repository placement.
- Supporting maintainers with open source practices.
- Reviewing portfolio health and repository disposition.
- Coordinating cross-functional review where necessary.
- Maintaining public open source governance documentation and tooling.

The Open Source team does not automatically assume technical ownership or
maintenance responsibility for individual projects.

---

### Project owning teams

The owning engineering or project team is responsible for the technical
stewardship of its repository.

Responsibilities generally include:

- Technical direction.
- Code maintenance.
- Issue triage.
- Pull request review.
- Releases.
- Documentation.
- Dependency management.
- Repository-specific automation.
- Maintaining appropriate CODEOWNERS.
- Communicating project-specific support expectations.
- Participating in lifecycle decisions.

Project teams are expected to notify or engage the Open Source team when major
governance changes are being considered.

Examples include:

- Publishing a new repository.
- Moving a private repository to public.
- Changing support model.
- Transferring a repository.
- Moving to maintenance-only.
- Archiving.
- Deleting.

---

### Maintainers

Maintainers are responsible for the ongoing health and stewardship of a
project.

Maintainers should:

- Review contributions.
- Respond to project issues as appropriate.
- Maintain project documentation.
- Manage releases where applicable.
- Keep dependencies and automation reasonably current.
- Follow security disclosure processes.
- Help maintain repository ownership continuity.
- Escalate lifecycle concerns when sustainable maintenance is no longer
  possible.

See
[Maintainer Guide](./docs/maintaining/maintainer-guide.md).

---

### Contributors

Contributors are expected to follow the contribution and conduct expectations
defined by the project.

Contribution access should follow least-privilege principles.

External contributors should not automatically receive elevated repository
permissions.

See:

- [External Contributors](./docs/contributing/external-contributors.md)
- [Employee Contributions](./docs/contributing/employee-contributions.md)
- [Contributor Access](./docs/governance/contributor-access.md)

---

## Decision rights

Open source governance decisions should be made at the lowest appropriate level
while preserving organization-wide consistency.

| Decision | Primary responsibility |
| --- | --- |
| Technical direction | Project owning team |
| Day-to-day maintenance | Project maintainers |
| Release decisions | Project owning team |
| Contribution acceptance | Project maintainers |
| Repository support model proposal | Project owning team |
| Repository support model governance | Open Source team with relevant stakeholders |
| New public repository approval | Governed repository creation process |
| Public repository placement | Open Source team with project owning team |
| Private-to-public transition | Project team with required governance review |
| Repository transfer | Open Source team and current/new owning teams |
| Maintenance-only transition | Owning team with Open Source governance review |
| Archival | Owning team and Open Source team |
| Deletion | Open Source team with appropriate ownership and risk review |
| Security vulnerability handling | Security process and project owners |
| Open source governance policy | Open Source team |

Some decisions may require additional Legal, Security, Product, Engineering, or
other review depending on the circumstances.

The Open Source Hub does not replace those required approvals.

---

## Repository ownership requirements

Every active public repository should have a clearly identifiable ownership
model.

At minimum:

- An owning team should be known.
- A primary maintainer should be identifiable.
- A backup maintainer or succession path should exist.
- CODEOWNERS should reflect current ownership where appropriate.

Ownership should preferably be team-based rather than dependent on a single
individual.

When ownership changes, access, CODEOWNERS, security responsibilities,
documentation, and release responsibilities should be reviewed.

See:

- [Contributor Access](./docs/governance/contributor-access.md)
- [Maintainer Succession](./docs/governance/maintainer-succession.md)

---

## Support models

Dynatrace open source repositories should communicate their support
expectations clearly.

Common support models include:

### Officially Supported

Used when a project is part of an officially supported Dynatrace product,
service, SDK, integration, distribution, or technical offering and formal
support expectations exist.

Repository location alone does not establish official support.

### Community-Supported

Used for actively maintained open source projects that are not covered by
formal Dynatrace product support.

Community-supported does not mean abandoned.

These projects should still have clear ownership and maintenance expectations.

### Experimental

Used for early-stage projects, prototypes, proofs of concept, or technical
exploration.

Experimental repositories should communicate that:

- Interfaces may change.
- Stability is not guaranteed.
- The project may be discontinued.

### Maintenance-Only

Used when a project remains available but is no longer receiving significant
new feature development.

Maintenance-only repositories should clearly document their current
maintenance expectations.

See [Support Models](./docs/governance/support-models.md).

---

## Repository placement

Repository placement should reflect purpose, ownership, audience, and project
context.

### `Dynatrace`

Generally appropriate for:

- Product-aligned projects.
- Officially supported components.
- Strategic technical assets.
- Supported SDKs, distributions, or integrations.

### `dynatrace-oss`

Generally appropriate for:

- Community-supported projects.
- Ecosystem integrations.
- Developer tooling.
- Educational projects.
- Customer or partner enablement.
- Experiments.
- Broader community collaboration.

### Upstream or foundation

An upstream project, standards community, or foundation should be preferred
when it is the natural long-term home for the work.

### Private

Projects should remain private when:

- The public purpose is unclear.
- Ownership is unresolved.
- Licensing is unresolved.
- Security or confidentiality concerns remain.
- The project is primarily internal.
- Publication readiness is incomplete.

See
[Where Does My Repository Belong?](./docs/getting-started/where-does-my-repo-belong.md).

---

## New repository governance

New public repositories should not be created solely as an administrative
convenience.

Before repository creation, the proposing team should establish:

- Project purpose.
- Intended audience.
- Open source value.
- Owning team.
- Maintainers.
- Support model.
- Repository location.
- License status.
- Publication readiness.
- Security readiness.
- Whether an upstream alternative exists.

See:

- [New Repository Requirements](./docs/publishing/new-repositories.md)
- [Publishing Checklist](./docs/publishing/publishing-checklist.md)

When repository creation is ready to proceed, teams should use the current
Dynatrace Open Source request process.

---

## Private-to-public transitions

Existing private repositories require additional review before publication.

Teams should evaluate:

- Repository history.
- Historical secrets.
- Credentials.
- Internal-only references.
- Customer information.
- Confidential information.
- Third-party code.
- Licensing.
- Automation.
- Documentation.
- Ownership.
- Support expectations.

Removing sensitive information from the current branch does not necessarily
remove it from repository history.

See
[Private-to-Public Transition](./docs/publishing/private-to-public.md).

---

## Repository transfers

Repository transfers are governance and ownership decisions, not simply
administrative moves.

Before transfer, teams should review:

- Current and future ownership.
- Repository purpose.
- Support expectations.
- Destination organization.
- CODEOWNERS.
- Permissions.
- Actions.
- Secrets.
- Packages.
- Releases.
- Documentation.
- Security responsibilities.
- External dependencies.

See
[Repository Transfers](./docs/publishing/repository-transfers.md).

---

## Security responsibilities

Public repositories must follow applicable security disclosure and repository
security requirements.

Dynatrace organizations may provide an organization-level security policy that
applies to repositories by default.

A repository-specific `SECURITY.md` is only required where additional
project-specific guidance is necessary.

Examples may include:

- Supported versions.
- Project-specific security contacts.
- Additional disclosure guidance.
- Project-specific vulnerability handling expectations.

Vulnerabilities must not be reported through public issues, pull requests, or
discussions.

See
[Security Readiness](./docs/maintaining/security-readiness.md).

---

## Repository health

Maintainers and owning teams should periodically evaluate repository health.

Signals may include:

- Recent maintenance activity.
- Open issue and pull request responsiveness.
- Dependency health.
- Security findings.
- Release activity.
- Maintainer availability.
- Documentation quality.
- Community activity.
- Support expectations.

Automated tools may assist with repository health assessment, but automated
metrics should inform rather than replace human governance decisions.

See:

- [Repository Health](./docs/maintaining/repository-health.md)
- [OpenSSF Scorecard](./docs/maintaining/openssf-scorecard.md)

---

## Repository lifecycle

Repositories move through different states during their lifetime.

Typical classifications may include:

- Strategic.
- Active / Community-Supported.
- Experimental.
- Maintenance-Only.
- Archive Candidate.
- Transfer or Deletion Candidate.

Classification describes the current portfolio state.

Disposition describes the action being considered.

Examples of dispositions include:

- Keep and invest.
- Continue.
- Move.
- Transfer.
- Archive.
- Delete.

See
[Repository Lifecycle](./docs/governance/repository-lifecycle.md).

---

## Maintenance-only

A repository may move to maintenance-only when it remains useful but no longer
receives significant feature development.

The repository should clearly communicate:

- Current maintenance expectations.
- Whether security fixes continue.
- Whether contributions are accepted.
- Whether a replacement exists.
- Whether future archival is expected.

Maintenance-only should be an explicit lifecycle state rather than an
accidental result of reduced activity.

---

## Archival

Archiving is generally preferred over deletion when a repository contains
meaningful history or may still provide reference value.

Before archival, teams should consider:

- Replacement or migration guidance.
- README archive notice.
- Documentation updates.
- Dependency references.
- Package and release implications.
- Support expectations.
- Open issues and pull requests.

Archived repositories should clearly communicate that they are intentionally
retired.

See:

- [Archive Policy](./docs/retiring/archive-policy.md)
- [Archive Checklist](./docs/retiring/archive-checklist.md)

---

## Deletion

Deletion should be uncommon.

Appropriate cases may include:

- Accidental repository creation.
- Empty temporary repositories.
- Duplicates.
- Legal requirements.
- Security requirements.
- Other exceptional circumstances where retaining the repository creates
  material risk or no meaningful historical value exists.

Meaningful project history should normally be preserved through archival rather
than deletion.

See
[Deletion Policy](./docs/retiring/deletion-policy.md).

---

## Exceptions

There may be legitimate cases where standard guidance does not fit a project's
circumstances.

Examples may include:

- Mirrors.
- Generated repositories.
- Distribution-only repositories.
- Package publishing repositories.
- Foundation-managed projects.
- Regulatory or contractual constraints.
- Unusual licensing arrangements.

Exceptions should be intentional and documented.

A repository should not silently ignore governance requirements because its
architecture or purpose is unusual.

If an exception cannot be resolved through existing Open Source Hub guidance,
the issue should be reviewed with the Open Source team and any relevant
stakeholders.

---

## Governance review and advisory input

Open source governance benefits from input across multiple disciplines.

Depending on the decision, relevant participants may include representatives
from:

- Engineering.
- Developer Relations.
- Product.
- Security.
- Legal.
- Communications.
- Open Source.
- Other teams with direct ownership or subject-matter responsibility.

Advisory participation does not transfer technical ownership away from the
responsible project team.

The purpose of cross-functional review is to improve decisions, surface risks,
and provide consistent organizational guidance.

---

## Portfolio governance

The Open Source team periodically reviews the public repository portfolio to
identify:

- Strategic projects.
- Healthy active projects.
- Projects requiring ownership clarification.
- Maintenance-only candidates.
- Archive candidates.
- Transfer candidates.
- Deletion candidates.
- Opportunities for consolidation.
- Opportunities for upstream contribution.
- Repository security and governance improvements.

Portfolio review findings are recommendations until the appropriate project
owners and governance stakeholders have evaluated the proposed action.

Automated signals should not be treated as sufficient evidence for lifecycle
decisions without project context.

---

## Governance changes

This governance framework should evolve as Dynatrace's open source strategy,
portfolio, and operating model change.

Significant changes should:

1. Be proposed through a pull request.
2. Explain the reason for the change.
3. Identify related policy documents that may also need updates.
4. Receive appropriate review.
5. Be reflected in supporting Open Source Hub documentation.

Detailed policy should be maintained in the relevant guidance document rather
than duplicated unnecessarily in this file.

---

## Related guidance

### Getting started

- [Open Source Hub Overview](./docs/getting-started/overview.md)
- [How Dynatrace Approaches Open Source](./docs/getting-started/how-dynatrace-approaches-open-source.md)
- [Should This Be Open Source?](./docs/getting-started/should-this-be-open-source.md)
- [Where Does My Repository Belong?](./docs/getting-started/where-does-my-repo-belong.md)
- [Customer and Partner Guidance](./docs/getting-started/customer-and-partner-guidance.md)

### Governance

- [Repository Lifecycle](./docs/governance/repository-lifecycle.md)
- [Support Models](./docs/governance/support-models.md)
- [Contributor Access](./docs/governance/contributor-access.md)
- [Maintainer Succession](./docs/governance/maintainer-succession.md)

### Publishing

- [New Repository Requirements](./docs/publishing/new-repositories.md)
- [Private-to-Public Transition](./docs/publishing/private-to-public.md)
- [Publishing Checklist](./docs/publishing/publishing-checklist.md)
- [Repository Transfers](./docs/publishing/repository-transfers.md)

### Maintaining

- [Maintainer Guide](./docs/maintaining/maintainer-guide.md)
- [Repository Health](./docs/maintaining/repository-health.md)
- [Dependency Management](./docs/maintaining/dependency-management.md)
- [Security Readiness](./docs/maintaining/security-readiness.md)
- [OpenSSF Scorecard](./docs/maintaining/openssf-scorecard.md)

### Contributing

- [Employee Contributions](./docs/contributing/employee-contributions.md)
- [External Contributors](./docs/contributing/external-contributors.md)
- [Upstream Contributions](./docs/contributing/upstream-contributions.md)

### Retiring

- [Archive Policy](./docs/retiring/archive-policy.md)
- [Archive Checklist](./docs/retiring/archive-checklist.md)
- [Deletion Policy](./docs/retiring/deletion-policy.md)

---

## Governance principle

The Open Source team provides the framework, guidance, coordination, and
governance for Dynatrace open source.

Individual repositories remain technically owned and maintained by their
responsible teams.

The objective is not governance for its own sake.

The objective is to make open source participation easier to understand,
sustainable to maintain, and valuable to Dynatrace and the broader ecosystem.
