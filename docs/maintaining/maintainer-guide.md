# Maintainer Guide

Maintainers are responsible for the ongoing health, usability, and sustainability of a Dynatrace public repository.

Maintainer responsibility includes more than reviewing pull requests. Maintainers are expected to keep the repository understandable, secure, current, and aligned with its documented support model.

## Maintainer responsibilities

Maintainers should:

- Review and respond to issues and pull requests.
- Keep repository documentation current.
- Maintain appropriate branch protections or rulesets.
- Monitor dependency and security updates.
- Maintain repository automation.
- Keep repository ownership current.
- Ensure the support model remains accurate.
- Review repository health periodically.
- Escalate lifecycle concerns when a project is no longer sustainable.

## Ownership

Every active repository should have:

- An owning team.
- At least one active maintainer.
- A backup maintainer or documented succession path.
- Current `CODEOWNERS` entries.

Team-based ownership is preferred over reliance on a single individual.

If ownership becomes unclear, the repository should enter lifecycle review.

## Repository status

Maintainers should ensure the repository accurately communicates its current state.

Examples include:

- Officially supported.
- Community-supported.
- Experimental.
- Maintenance-only.
- Deprecated.
- Archived.

The repository's README and other public documentation should not imply a level of support that the owning team cannot provide.

See [Support Models](../governance/support-models.md).

## Issues and pull requests

Maintainers should periodically review:

- Open issues.
- Open pull requests.
- Stale requests.
- Unanswered contributor questions.
- Security-sensitive reports that may have been submitted incorrectly.

Not every issue requires immediate resolution, but long-running repositories should not accumulate unmanaged queues indefinitely.

Where practical:

- Close issues that are no longer relevant.
- Redirect product support requests to the appropriate channel.
- Label issues consistently.
- Explain when requests are out of scope.
- Encourage upstream contribution when appropriate.

## Releases

If the project produces releases, maintainers should define and document:

- Release ownership.
- Release cadence where relevant.
- Versioning approach.
- Release automation.
- Changelog or release note expectations.
- Compatibility expectations.

Avoid publishing releases that cannot reasonably be maintained.

## Documentation

Maintainers should keep documentation synchronized with project behavior.

Review:

- README.
- CONTRIBUTING.
- SECURITY.
- Installation instructions.
- Examples.
- Configuration guidance.
- API documentation.
- Migration guidance.
- Support expectations.

Broken or outdated documentation is a repository health issue.

## Automation

Review repository automation periodically, including:

- GitHub Actions.
- Dependency updates.
- Release automation.
- Documentation checks.
- Link validation.
- Security scanning.
- Issue automation.
- Scheduled workflows.

Remove workflows that are unused, broken, or no longer necessary.

See [Dependency Management](./dependency-management.md).

## Security

Maintainers should ensure:

- `SECURITY.md` is present and current.
- Vulnerability reports have a private reporting path.
- Dependency alerts are reviewed.
- Known vulnerabilities are assessed.
- Secrets are not stored in the repository.
- GitHub Actions use appropriate permissions.
- Unnecessary tokens and integrations are removed.

See [Security Readiness](./security-readiness.md).

## Repository health review

Active repositories should be reviewed periodically for:

- Maintainer activity.
- Commit activity.
- Contributor activity.
- Dependency health.
- Security posture.
- Documentation quality.
- Open issue and pull request backlog.
- Automation status.
- OpenSSF Scorecard results where applicable.
- Continued strategic or ecosystem value.

A period of inactivity should trigger review rather than automatic archival.

See [Repository Health](./repository-health.md).

## Maintainer succession

If a maintainer leaves the team, changes responsibilities, or can no longer maintain the project:

- Identify a replacement.
- Transfer required access.
- Update `CODEOWNERS`.
- Update repository documentation.
- Notify the owning team.
- Escalate if no successor exists.

A repository should not remain indefinitely dependent on an inactive maintainer.

See [Maintainer Succession](../governance/maintainer-succession.md).

## When maintenance is no longer sustainable

If the owning team can no longer reasonably maintain the repository, consider:

- Moving to community-supported status.
- Moving to maintenance-only status.
- Transferring ownership.
- Deprecating the project.
- Archiving the repository.

Do not leave an abandoned repository appearing actively supported.

## Related guidance

- [Repository Health](./repository-health.md)
- [Dependency Management](./dependency-management.md)
- [Security Readiness](./security-readiness.md)
- [OpenSSF Scorecard](./openssf-scorecard.md)
- [Repository Lifecycle](../governance/repository-lifecycle.md)
- [Support Models](../governance/support-models.md)
