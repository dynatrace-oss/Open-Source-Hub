# How Dynatrace Approaches Open Source

Dynatrace participates in open source as a contributor, maintainer, consumer, and ecosystem partner.

Our approach is based on a simple idea: open source should create durable value for users, contributors, Dynatrace, and the broader ecosystem.

That means we do not treat open source as simply publishing code. Public repositories require clear purpose, ownership, contribution pathways, security practices, maintenance, and lifecycle decisions.

---

## Open source with purpose

A project should be open source for a clear reason.

That reason may include:

- Improving interoperability.
- Contributing to shared industry standards.
- Supporting open ecosystems such as OpenTelemetry.
- Enabling developers, customers, or partners.
- Encouraging external contribution.
- Collaborating with upstream projects.
- Sharing useful developer tooling or examples.
- Building technology that benefits from community participation.

Publishing code without a clear audience, owner, or long-term purpose creates maintenance burden without necessarily creating ecosystem value.

Before starting a new public project, ask:

> What becomes better because this project is open source?

See [Should This Be Open Source?](./should-this-be-open-source.md).

---

## Public by design

When a project is intended to become open source, teams should consider public requirements early rather than treating publication as a final release step.

Public development requires consideration of:

- Licensing.
- Intellectual property.
- Security.
- Documentation.
- Repository ownership.
- Contribution workflows.
- Support expectations.
- Dependencies.
- Automation.
- Long-term maintenance.

Designing for openness from the beginning reduces the effort and risk involved in making a project public later.

See [New Repository Requirements](../publishing/new-repositories.md).

---

## Clear ownership

Every active Dynatrace public repository should have clear ownership.

At minimum, that means:

- An owning team.
- Active maintainers.
- A support model.
- A succession path.
- Current repository permissions and `CODEOWNERS`.

Open source ownership should not depend indefinitely on one individual.

When ownership changes, responsibility should be intentionally transferred rather than allowed to become unclear.

See:

- [Maintainer Succession](../governance/maintainer-succession.md)
- [Contributor Access](../governance/contributor-access.md)

---

## Be explicit about support

A repository being public does not automatically mean that it is formally supported by Dynatrace.

Projects should clearly communicate whether they are:

- Officially supported.
- Community-supported.
- Experimental.
- Maintenance-only.

Users should be able to understand what level of response, maintenance, compatibility, and product support they can reasonably expect.

Community-supported does not mean abandoned.

Officially supported does not mean every interaction belongs in GitHub Issues.

See [Support Models](../governance/support-models.md).

---

## Contribute upstream when it makes sense

Dynatrace should avoid maintaining unnecessary downstream divergence when useful changes can reasonably be contributed to an upstream project.

Upstream contribution can:

- Reduce long-term maintenance.
- Improve interoperability.
- Strengthen shared standards.
- Benefit a broader community.
- Increase Dynatrace participation and influence in important projects.

When working with upstream communities, we participate within their governance and contribution processes.

Dynatrace business priorities do not automatically become upstream priorities.

Influence is built through useful, sustained participation.

See [Upstream Contributions](../contributing/upstream-contributions.md).

---

## Participate, do not just consume

Strategic open source participation is broader than using open source dependencies.

It can include:

- Code contributions.
- Documentation.
- Issue triage.
- Code review.
- Release support.
- Standards development.
- Working groups.
- Maintainer roles.
- Community education.
- Testing.
- Ecosystem collaboration.

Where open source projects are strategically important to Dynatrace, we should evaluate how we can contribute to their long-term health rather than participate only as a consumer.

---

## Build for sustainability

Publishing a repository is the beginning of its public lifecycle, not the end.

Active projects require ongoing attention to:

- Maintainer capacity.
- Documentation.
- Security.
- Dependencies.
- Automation.
- Releases.
- Community interaction.
- Repository health.

Teams should consider sustainability before creating new repositories.

A small number of healthy, useful projects is more valuable than a large number of abandoned public repositories.

---

## Review instead of abandon

Projects change over time.

A repository that was once strategically important may become stable, replaced, transferred, or no longer actively maintained.

That is normal.

Repositories should move intentionally through their lifecycle rather than simply becoming inactive.

Possible outcomes include:

- Continued active investment.
- Community-supported maintenance.
- Maintenance-only status.
- Transfer to another owner.
- Deprecation.
- Archival.
- Deletion in limited circumstances.

Inactivity alone should trigger review, not automatic archival.

See [Repository Lifecycle](../governance/repository-lifecycle.md).

---

## Prefer stewardship over accumulation

The goal is not to maximize the number of repositories Dynatrace owns.

Where appropriate, a project may be better served by:

- Contributing directly upstream.
- Moving to an open source foundation.
- Transferring to a broader community.
- Consolidating with another project.
- Archiving a repository that has reached the end of its useful lifecycle.

Repository ownership creates responsibility.

Dynatrace should retain ownership where we can provide meaningful and sustainable stewardship.

---

## Security is part of open source maintenance

Security responsibilities do not end when code becomes public.

Public repositories should have:

- A clear vulnerability reporting path.
- Appropriate dependency management.
- Appropriate access controls.
- Secure automation.
- Repository health review.
- A defined security owner.

Dynatrace provides organization-level security disclosure guidance for public repositories. Repository-specific security documentation should be added when additional guidance is required.

Security vulnerabilities should not be disclosed through public Issues, pull requests, or Discussions.

See [Security Readiness](../maintaining/security-readiness.md).

---

## Community participation should be clear and respectful

Open source depends on people.

Dynatrace projects should make it easy for contributors to understand:

- Whether contributions are welcome.
- How to propose changes.
- How decisions are made.
- What maintainers expect.
- What contributors can expect from maintainers.

Maintainers should communicate scope and decisions clearly and participate constructively with external contributors.

External participation should not require unnecessary repository access.

See [External Contributors](../contributing/external-contributors.md).

---

## Open source is an ecosystem strategy

Open source creates the most value when it connects Dynatrace to broader technical ecosystems rather than existing only as a collection of company-owned repositories.

Our approach should consider:

- Upstream projects.
- Open standards.
- Foundations.
- Contributors.
- Customers.
- Partners.
- Developers.
- Educators.
- Emerging ecosystem technologies.

Repository governance provides the foundation for this work, but governance is not the end goal.

The broader goal is to make it easier for Dynatrace to participate meaningfully, sustainably, and visibly in the open source ecosystem.

---

## Our principles

In practice, the Dynatrace approach can be summarized as:

### Start with purpose

Open source something because public participation creates value.

### Design for openness

Consider public requirements early.

### Make ownership visible

Every active project needs accountable maintainers.

### Be explicit about support

Users should understand what they can expect.

### Contribute upstream

Avoid unnecessary downstream divergence.

### Participate in the ecosystem

Contribute more than code.

### Build sustainably

Do not create projects without a realistic maintenance model.

### Review lifecycle intentionally

Do not allow repositories to become abandoned by default.

### Protect users and contributors

Security and responsible disclosure are part of maintaining open source.

### Prefer stewardship over ownership

Own projects where Dynatrace can provide meaningful long-term value.

---

## Related guidance

- [Open Source Overview](./overview.md)
- [Should This Be Open Source?](./should-this-be-open-source.md)
- [Where Does My Repository Belong?](./where-does-my-repo-belong.md)
- [Repository Lifecycle](../governance/repository-lifecycle.md)
- [Support Models](../governance/support-models.md)
- [Upstream Contributions](../contributing/upstream-contributions.md)
- [Repository Health](../maintaining/repository-health.md)
- [Security Readiness](../maintaining/security-readiness.md)
