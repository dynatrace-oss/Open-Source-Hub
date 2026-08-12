# Upstream Contributions

Dynatrace should contribute improvements to upstream open source projects whenever doing so is practical and beneficial to the broader ecosystem.

Upstream contribution reduces unnecessary forks, improves interoperability, distributes maintenance responsibility, and helps ensure Dynatrace participates as a contributor rather than only as a consumer of open source.

## What is an upstream contribution?

An upstream contribution is a change submitted to the original or authoritative open source project rather than maintained only in a Dynatrace-owned fork or downstream implementation.

Examples include:

- Bug fixes.
- New instrumentation.
- Protocol improvements.
- OpenTelemetry enhancements.
- Performance improvements.
- Documentation.
- Compatibility improvements.
- Security improvements.
- New integrations.
- Test coverage.
- Standards-related functionality.

## Prefer upstream when possible

Before creating or maintaining a Dynatrace-specific implementation, ask:

1. Could this capability benefit other users of the upstream project?
2. Is the functionality within the scope of the upstream project?
3. Would upstream maintainers reasonably consider accepting it?
4. Would upstreaming reduce long-term maintenance for Dynatrace?
5. Would maintaining a separate fork create unnecessary divergence?

If the answer to these questions is generally yes, upstream contribution should be the preferred approach.

## When downstream work may be appropriate

A Dynatrace-specific implementation may be appropriate when:

- The functionality is specific to Dynatrace.
- The upstream project intentionally does not support the use case.
- An urgent customer or product requirement cannot wait for upstream review.
- The contribution is experimental and needs validation before being proposed upstream.
- Licensing or governance constraints prevent upstream acceptance.
- The upstream project is inactive or unable to accept changes.

When downstream work is necessary, teams should still evaluate whether the change can be upstreamed later.

## Avoid permanent forks by default

Forking may be useful for:

- Contributing changes upstream.
- Temporary experimentation.
- Testing patches.
- Maintaining a short-term downstream fix.

A fork should not automatically become a long-term Dynatrace project.

Long-lived forks create additional responsibility for:

- Security patches.
- Dependency updates.
- Merge conflicts.
- Compatibility.
- Releases.
- Documentation.
- Testing.
- Maintainer capacity.

If a long-lived fork is necessary, document:

- Why the fork exists.
- What differs from upstream.
- Who owns it.
- How upstream changes are synchronized.
- Whether changes are expected to return upstream.
- What conditions would allow the fork to be retired.

## Before contributing upstream

Review the upstream project's:

- Contribution guidelines.
- Governance model.
- Code of Conduct.
- CLA or DCO requirements.
- Issue and pull request process.
- Release model.
- Maintainer expectations.

For significant changes, engage upstream maintainers before investing substantial engineering effort.

## Engage early

For larger contributions, start with a proposal, issue, design discussion, or other process used by the upstream project.

Early engagement can help determine:

- Whether the contribution fits project scope.
- Whether maintainers support the direction.
- Whether a similar effort already exists.
- Which technical approach is preferred.
- Whether additional design review is required.

Avoid developing large features in isolation and presenting them upstream only after implementation is complete.

## Respect upstream governance

Dynatrace contributors should participate within the project's existing governance.

Do not assume that:

- Dynatrace's business priority creates an upstream priority.
- A contribution must be accepted because Dynatrace invested engineering effort.
- Maintainers must meet Dynatrace timelines.
- Dynatrace should receive special decision rights because it contributes code.

Build influence through sustained, constructive participation.

## Contribute maintainably

A successful upstream contribution should avoid unnecessary Dynatrace-specific assumptions.

Where practical:

- Design for broader ecosystem use.
- Use standard interfaces.
- Avoid vendor-specific configuration in generic components.
- Include tests.
- Include documentation.
- Follow upstream coding conventions.
- Consider ongoing maintenance requirements.

The goal is to create functionality the upstream community can reasonably own with Dynatrace as a participant.

## Contribute more than code

Strategic upstream participation can include:

- Issue triage.
- Code review.
- Documentation.
- Release support.
- Working groups.
- Governance participation.
- Specification development.
- Community education.
- Testing.
- Maintainer sponsorship.
- Conference and community participation.

Influence in open source usually comes from sustained participation rather than isolated pull requests.

## Strategic upstream projects

Dynatrace may identify upstream projects where deeper participation is strategically important.

Prioritization may consider:

- Importance to Dynatrace products.
- Customer adoption.
- Ecosystem relevance.
- Technical dependencies.
- Standards influence.
- Current Dynatrace contribution level.
- Risk of upstream changes.
- Opportunity for meaningful community participation.

Strategic status should not mean that every potential contribution receives unlimited investment.

Participation should have clear objectives and be reviewed periodically.

## Measuring upstream participation

Useful measures may include:

- Contributions submitted.
- Contributions accepted.
- Active Dynatrace contributors.
- Maintainer or reviewer roles.
- Upstream issues resolved.
- Releases supported.
- Specifications or working groups participated in.
- Downstream patches eliminated.
- Forks retired.
- Time required to maintain downstream divergence.

Contribution counts alone should not be treated as the primary measure of impact.

## When an upstream contribution is declined

A declined contribution does not automatically justify maintaining a permanent fork.

Consider:

- Revising the proposal.
- Adjusting the implementation.
- Finding a standards-based alternative.
- Maintaining the capability outside the upstream project.
- Re-evaluating whether the functionality is strategically necessary.

If Dynatrace maintains a downstream implementation, document the rationale and ownership.

## Security

Security-sensitive upstream contributions should follow the upstream project's private vulnerability disclosure process.

Do not publicly disclose a vulnerability through a pull request or issue before coordinated disclosure is appropriate.

## Employee participation

Dynatrace employees contributing upstream should clearly understand whether they are participating:

- As part of their Dynatrace role.
- As an upstream maintainer.
- As an individual contributor.

These roles may overlap, but contributors should avoid implying that an upstream project is controlled by Dynatrace unless that is actually the case.

See [Employee Contributions](./employee-contributions.md).

## Repository transfers

In some cases, a project may be better governed by:

- An upstream project.
- An open source foundation.
- A broader community organization.
- Another appropriate owner.

Where long-term ecosystem stewardship would be stronger outside Dynatrace, repository transfer may be preferable to indefinite Dynatrace ownership.

## Related guidance

- [Employee Contributions](./employee-contributions.md)
- [External Contributors](./external-contributors.md)
- [Where Does My Repository Belong?](../getting-started/where-does-my-repo-belong.md)
- [Repository Lifecycle](../governance/repository-lifecycle.md)
- [Support Models](../governance/support-models.md)
