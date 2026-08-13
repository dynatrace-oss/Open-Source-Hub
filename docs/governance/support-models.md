# Support Models

Dynatrace public repositories should clearly communicate what level of support users and contributors can expect.

A repository being public does **not** automatically mean that it is formally supported by Dynatrace.

Each active public repository should have an explicit support model that reflects:

- Who owns the project.
- Who maintains it.
- How users should ask for help.
- Whether formal Dynatrace Support applies.
- What response expectations are reasonable.
- How actively the project is developed.
- How security issues should be reported.
- What lifecycle commitments exist.

Support expectations should be visible in the repository documentation and should match the actual capacity of the owning team.

---

## Support model categories

Dynatrace public repositories generally fall into one of the following support models:

- **Officially supported**
- **Community-supported**
- **Experimental**
- **Maintenance-only**

A repository may later become deprecated or archived as part of its lifecycle.

Support model and lifecycle classification are related, but they are not the same thing.

For example:

- A strategic repository may be officially supported or community-supported.
- A community-supported repository may still be highly active.
- A maintenance-only repository may remain important to existing users.
- An experimental repository may later become officially supported.

See [Repository Lifecycle](./repository-lifecycle.md).

---

# Officially supported projects

Officially supported projects are maintained as part of Dynatrace-supported product, service, integration, SDK, distribution, or other supported technical delivery.

These repositories should have a clearly defined relationship to an officially supported Dynatrace offering.

## What users can expect

Where applicable, officially supported projects should provide:

- A clearly identified owning team.
- Active maintainer responsibility.
- Maintained documentation.
- Defined release or compatibility expectations.
- Active dependency management.
- Security monitoring and remediation.
- A documented path to Dynatrace Support.
- Ongoing maintenance appropriate to the supported offering.

The repository documentation should clearly explain which support channel applies.

GitHub Issues should not be presented as a replacement for formal Dynatrace Support unless that is explicitly part of the project's support model.

## Repository expectations

Officially supported repositories should maintain:

- A current `README.md`.
- Clear ownership.
- Current `CODEOWNERS`.
- Contribution guidance where contributions are accepted.
- Appropriate repository automation.
- Security policy coverage.
- Dependency and vulnerability management.
- Appropriate branch protection or rulesets.
- Current release documentation where applicable.

Repositories associated with supported products should not rely entirely on a single maintainer.

## Support statement example

A repository may use language such as:

> **Support**
>
> This project is officially supported by Dynatrace.
>
> For product support, troubleshooting, and service-related questions, use the appropriate Dynatrace Support channel.
>
> GitHub Issues may be used for repository-specific bugs, feature requests, or contribution discussions where documented.

The exact statement should be customized to the project.

---

# Community-supported projects

Community-supported projects are maintained openly by Dynatrace employees and/or community contributors but are not covered by formal Dynatrace product support unless explicitly stated.

Community-supported does **not** mean abandoned, unsupported in every sense, or unmaintained.

It means that support is provided through the open source project rather than through a formal product-support commitment.

## What users can expect

Community-supported repositories may:

- Accept issues and pull requests.
- Receive maintainer responses as capacity allows.
- Have community-driven priorities.
- Have less predictable release schedules.
- Evolve based on maintainer and contributor capacity.
- Provide no guaranteed response or resolution time.

Users should not assume that:

- A reported issue will receive an immediate response.
- A feature request will be implemented.
- A release will occur on a fixed schedule.
- Dynatrace Support will troubleshoot the project.

## Repository expectations

A community-supported repository should still have:

- A known owning team or maintainer.
- A current README.
- Clear contribution guidance.
- A documented support statement.
- Security reporting coverage.
- Appropriate dependency maintenance.
- Appropriate repository health review.
- Clear lifecycle status.

Community-supported status should never be used as a label for a repository that has no real maintainer ownership.

If maintainers no longer have capacity to support the project, the repository should enter lifecycle review.

See [Repository Health](../maintaining/repository-health.md).

## Support statement example

A repository may use language such as:

> **Community Support**
>
> This project is maintained as a community-supported open source project.
>
> Issues and pull requests are welcome, and maintainers will respond as capacity allows.
>
> This repository is not covered by formal Dynatrace product support unless explicitly stated elsewhere.

---

# Experimental projects

Experimental repositories are used for early-stage ideas, technical exploration, prototypes, proofs of concept, or emerging ecosystem work.

Experimental projects may change significantly or be discontinued.

## What users can expect

Experimental projects may:

- Introduce breaking changes.
- Have incomplete documentation.
- Have limited test coverage.
- Change architecture or scope.
- Have no guaranteed release cadence.
- Have limited maintainer capacity.
- Be transferred, promoted, consolidated, or archived.

Users should not assume experimental projects are suitable for production use.

## Repository expectations

Experimental repositories should clearly state:

- That the project is experimental.
- What the project is attempting to validate.
- Who owns or maintains it.
- Whether contributions are welcome.
- What support, if any, users should expect.
- Whether production use is recommended.

Experimental status should not be permanent by default.

Projects should periodically be reviewed to determine whether they should:

- Continue experimentation.
- Become actively maintained.
- Become officially supported.
- Become community-supported.
- Be transferred.
- Be archived.

## Support statement example

> **Experimental**
>
> This project is experimental and may change or be discontinued without notice.
>
> It is not officially supported by Dynatrace and is not recommended for production use unless explicitly documented otherwise.
>
> Issues and contributions may be reviewed as maintainer capacity allows.

---

# Maintenance-only projects

Maintenance-only repositories remain available and maintained for existing users, but active feature development has substantially ended.

These projects may still be important and should not automatically be treated as abandoned.

## What users can expect

Maintenance-only projects may receive:

- Critical bug fixes.
- Security updates.
- Compatibility updates.
- Dependency updates.
- Limited documentation corrections.

Users generally should not expect:

- Significant new features.
- Major architectural changes.
- Expansion of project scope.
- A high volume of new releases.

## Repository expectations

Maintenance-only repositories should clearly communicate:

- That active feature development has ended.
- What types of changes may still be accepted.
- Whether a successor project exists.
- Whether users should plan to migrate.
- Who currently owns the repository.

Maintenance-only status should be reviewed periodically.

Possible future outcomes include:

- Return to active development.
- Transfer.
- Deprecation.
- Archival.

## Support statement example

> **Maintenance Mode**
>
> This project is in maintenance mode.
>
> Critical fixes, security updates, and compatibility updates may be provided, but active feature development should not be expected.
>
> See the repository documentation for recommended alternatives or migration guidance where available.

---

# Security disclosures

Support model does not change how vulnerabilities should be disclosed.

Security vulnerabilities should be reported through the private disclosure process defined by the Dynatrace organization-level `SECURITY.md`.

Do **not** report suspected vulnerabilities through:

- Public GitHub Issues.
- Pull requests.
- GitHub Discussions.
- Other public repository channels.

Repositories should rely on the organization-level security policy unless repository-specific security guidance is required.

A repository-specific `SECURITY.md` may be appropriate when a project needs to document:

- Supported versions.
- Project-specific reporting instructions.
- Additional security contacts.
- Repository-specific disclosure expectations.
- Additional security information not covered by the organization-level policy.

Repository-specific guidance must not conflict with the organization-level security policy.

See [Security Readiness](../maintaining/security-readiness.md).

---

# Support and GitHub Issues

GitHub Issues may serve different purposes depending on the project.

They may be used for:

- Bug reports.
- Feature requests.
- Documentation issues.
- Contribution discussions.
- Community questions.

Repositories should clearly explain what Issues are intended for.

For officially supported projects, users should be directed to the appropriate Dynatrace Support channel for formal product support.

For community-supported and experimental projects, GitHub may be the primary public interaction channel, but response times should not be guaranteed unless explicitly documented.

---

# Contribution expectations by support model

| Support model | Contributions | Formal Dynatrace Support | Response expectation | Active development |
|---|---|---|---|---|
| **Officially supported** | Usually accepted where documented | Yes, where tied to a supported offering | Defined by applicable support and project processes | Expected |
| **Community-supported** | Encouraged where documented | No, unless explicitly stated | Best effort / maintainer capacity | Usually |
| **Experimental** | May be accepted | No | No guarantee | Exploratory |
| **Maintenance-only** | Usually limited in scope | Depends on project context | Limited | No major feature development |

Repository-specific guidance always takes precedence where more precise expectations are documented.

---

# Changing a support model

Support models may change during a repository's lifecycle.

Common transitions include:

```text
Experimental → Community-Supported
Experimental → Officially Supported
Officially Supported → Maintenance-Only
Community-Supported → Maintenance-Only
Maintenance-Only → Deprecated → Archived
```

A support model change should include review of:

- Ownership.
- Maintainer capacity.
- README language.
- Support disclaimers.
- Documentation.
- Release expectations.
- Security responsibilities.
- User or community impact.
- Repository inventory classification.

Where the change materially reduces support expectations, communicate it clearly to existing users.

---

# Support model review

Support models should be reviewed when:

- Ownership changes.
- Maintainer capacity changes.
- A project becomes part of a supported product.
- A supported product stops depending on the project.
- Development substantially slows.
- A repository is transferred.
- A repository enters lifecycle review.
- The documented support model no longer matches reality.

A repository should not continue advertising a support model that the owning team can no longer provide.

---

# Choosing a support model

Ask the following questions:

1. Is this repository directly associated with an officially supported Dynatrace offering?
2. Is there a team committed to maintaining it?
3. Is formal Dynatrace Support expected to assist users?
4. Are releases or compatibility commitments required?
5. Is the project primarily community-driven?
6. Is the project still experimental?
7. Has active feature development ended?

A simple decision guide:

```text
Is it part of an officially supported Dynatrace offering?
│
├── Yes → Officially Supported
│
└── No
    │
    ├── Is it actively maintained for community use?
    │      └── Yes → Community-Supported
    │
    ├── Is it primarily experimentation or validation?
    │      └── Yes → Experimental
    │
    └── Is active feature development finished?
           └── Yes → Maintenance-Only
```

---

# Documentation requirements

Every active public repository should make its support model easy to find.

At minimum, the README should communicate:

- Current project status.
- Support model.
- Where users should ask for help.
- Whether formal Dynatrace Support applies.
- How security vulnerabilities should be reported.
- Whether contributions are accepted.

See [Support Disclaimers](../templates/support-disclaimers.md) for reusable language.

---

# Related guidance

- [Repository Lifecycle](./repository-lifecycle.md)
- [Maintainer Succession](./maintainer-succession.md)
- [Contributor Access](./contributor-access.md)
- [Maintainer Guide](../maintaining/maintainer-guide.md)
- [Repository Health](../maintaining/repository-health.md)
- [Security Readiness](../maintaining/security-readiness.md)
- [Support Disclaimers](../templates/support-disclaimers.md)
