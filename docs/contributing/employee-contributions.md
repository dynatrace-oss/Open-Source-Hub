# Employee Contributions

Dynatrace employees are encouraged to contribute to open source projects when those contributions support Dynatrace technology, customers, the broader ecosystem, or the health of projects Dynatrace depends on.

This guidance applies to contributions made by Dynatrace employees to:

- Dynatrace-owned public repositories.
- Third-party open source projects.
- Foundation-hosted projects.
- Upstream dependencies used by Dynatrace.
- Open source projects where Dynatrace participates as a contributor or maintainer.

## Before contributing

Before making a contribution, determine:

- Whether the contribution is part of your Dynatrace work.
- Whether the repository is owned by Dynatrace or an external project.
- Whether the contribution includes Dynatrace intellectual property.
- Whether the project requires a Contributor License Agreement (CLA), Developer Certificate of Origin (DCO), or other contributor agreement.
- Whether the change should be contributed upstream rather than maintained as a Dynatrace-specific fork.
- Whether additional legal, security, or product review is required.

When in doubt, consult the appropriate internal owner before contributing.

## Contributions to Dynatrace repositories

Employees contributing to Dynatrace public repositories should follow the same contribution process expected of external contributors unless the repository documents a different maintainer workflow.

This includes:

- Following `CONTRIBUTING.md`.
- Using pull requests for changes.
- Completing required reviews.
- Passing required automated checks.
- Following repository-specific testing requirements.
- Updating documentation where appropriate.
- Following the repository's security reporting process.

Maintainer or administrator access should not be used to bypass normal review requirements without a documented reason.

## Contributions to external projects

When contributing to a third-party or upstream open source project:

- Follow the project's contribution guidelines.
- Respect its governance and maintainer decisions.
- Use the contribution mechanisms established by the project.
- Complete required CLA or DCO processes.
- Avoid presenting Dynatrace preferences as requirements of the upstream project.
- Work collaboratively with existing maintainers and contributors.

Dynatrace participation should strengthen the upstream community rather than create unnecessary downstream divergence.

## Prefer upstream contributions

When functionality or fixes can reasonably benefit the broader project, contribute them upstream.

Prefer upstream contributions when:

- Fixing defects in a dependency.
- Adding generally useful capabilities.
- Improving interoperability.
- Improving OpenTelemetry or other ecosystem standards.
- Improving documentation used broadly by the community.
- Removing the need for a Dynatrace-specific patch or fork.

Maintaining private or downstream modifications should be the exception when an upstream contribution is practical.

See [Upstream Contributions](./upstream-contributions.md).

## Identity and representation

When contributing as part of your Dynatrace role, be clear about your affiliation where appropriate.

Do not imply that:

- Your personal opinion represents an official Dynatrace position unless authorized.
- Dynatrace officially supports an external project merely because employees contribute to it.
- An upstream maintainer decision represents a Dynatrace commitment.

Follow applicable Dynatrace communication and brand guidance.

## Intellectual property

Do not contribute:

- Proprietary Dynatrace source code that has not been approved for public release.
- Confidential information.
- Customer information.
- Credentials or secrets.
- Internal architecture details that are not approved for publication.
- Third-party material that Dynatrace does not have the right to contribute.

Code developed internally should not be moved into a public repository solely through a pull request without completing the appropriate public-release process.

See [Private-to-Public Transition](../publishing/private-to-public.md).

## Security

Do not publicly disclose known or suspected vulnerabilities through:

- GitHub Issues.
- Pull requests.
- Discussions.
- Public chat channels.

Follow the security reporting and incident-response processes applicable to the repository or upstream project.

## Dependencies and licensing

Before introducing a new dependency:

- Confirm that its license is appropriate.
- Consider maintenance activity.
- Review security posture where appropriate.
- Avoid unnecessary dependencies.
- Follow repository-specific dependency requirements.

Do not copy code from other projects without verifying that its license permits the intended use.

## Use of personal repositories

Avoid using personal repositories as the permanent home for Dynatrace-owned open source projects.

Experiments may begin outside a Dynatrace organization where appropriate, but projects intended to represent or be maintained by Dynatrace should follow the repository publishing and transfer process.

See [Where Does My Repository Belong?](../getting-started/where-does-my-repo-belong.md).

## Maintainer responsibilities

Employees acting as maintainers should:

- Review contributions consistently.
- Communicate project scope clearly.
- Respond respectfully to contributors.
- Keep repository ownership current.
- Maintain documentation.
- Manage dependencies and automation.
- Follow security requirements.
- Escalate lifecycle concerns when the project can no longer be sustainably maintained.

Maintainer status creates an ongoing responsibility, not simply merge access.

## Leaving a team or changing roles

If you are a named maintainer and your responsibilities change:

- Identify a successor.
- Update `CODEOWNERS`.
- Transfer required permissions.
- Update repository documentation.
- Notify the owning team.
- Escalate if no replacement maintainer can be identified.

See [Maintainer Succession](../governance/maintainer-succession.md).

## Related guidance

- [External Contributors](./external-contributors.md)
- [Upstream Contributions](./upstream-contributions.md)
- [Repository Lifecycle](../governance/repository-lifecycle.md)
- [Support Models](../governance/support-models.md)
- [Private-to-Public Transition](../publishing/private-to-public.md)
