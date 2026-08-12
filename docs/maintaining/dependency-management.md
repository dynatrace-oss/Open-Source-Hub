# Dependency Management

Public repositories should manage dependencies in a way that reduces security risk, maintenance burden, and unnecessary technical debt.

Dependency management is an ongoing maintainer responsibility.

## Before adding a dependency

Before introducing a new dependency, consider:

- Is the dependency necessary?
- Is the project actively maintained?
- Is the license appropriate?
- Does the dependency have known security concerns?
- Is the dependency widely used or well understood?
- Can existing project capabilities meet the same need?
- What maintenance burden will the dependency create?

Avoid adding dependencies for minor functionality that can be implemented safely and maintainably without them.

## Dependency ownership

The owning team is responsible for understanding and maintaining dependencies used by the repository.

This includes:

- Direct dependencies.
- Build dependencies.
- Runtime dependencies.
- GitHub Actions.
- Container base images.
- Generated dependencies where applicable.

## Automated updates

Repositories should use automated dependency update tooling where appropriate.

Examples may include:

- Dependabot.
- Renovate.
- Ecosystem-specific update tools.

Automated updates should:

- Create reviewable pull requests.
- Run normal tests and validation.
- Avoid automatically merging high-risk changes without appropriate controls.

Automation should reduce maintenance work, not bypass review.

## Security updates

Known vulnerable dependencies should be reviewed promptly.

Maintainers should determine:

- Whether the vulnerable dependency is actually used.
- Whether the vulnerable code path is reachable.
- Whether an upgrade is available.
- Whether a temporary mitigation is required.
- Whether downstream users need to be informed.

Security alerts should not remain indefinitely unreviewed.

## Unsupported dependencies

Avoid relying on dependencies that are:

- Abandoned.
- End-of-life.
- No longer receiving security updates.
- Incompatible with supported runtime versions.

When an important dependency becomes unsupported:

1. Identify alternatives.
2. Evaluate migration impact.
3. Plan replacement.
4. Communicate compatibility changes where necessary.

## Version pinning

Use version constraints appropriate to the ecosystem and risk.

Avoid:

- Unbounded dependency versions.
- Referencing mutable branches for production dependencies.
- Relying on unreviewed latest versions.

GitHub Actions should use appropriately pinned versions consistent with security requirements.

## Forked dependencies

If Dynatrace maintains a fork of a dependency, document:

- Why the fork exists.
- What differs from upstream.
- Who owns the fork.
- How upstream changes are incorporated.
- Whether changes can be contributed upstream.
- What would allow the fork to be retired.

Prefer upstream contributions over indefinite downstream divergence.

See [Upstream Contributions](../contributing/upstream-contributions.md).

## License review

Dependencies must use licenses compatible with the repository and its intended distribution.

Do not assume that because a dependency is publicly available it can automatically be used in every context.

Follow applicable Dynatrace legal and open source review processes.

## Dependency inventory

Where practical, repositories should make dependencies discoverable through:

- Package manifests.
- Lock files.
- SBOM generation.
- Dependency graphs.
- Automated scanning.

For security-sensitive or distributed artifacts, consider maintaining a software bill of materials.

## Container dependencies

For containerized projects:

- Use maintained base images.
- Avoid unnecessary packages.
- Keep images updated.
- Review known vulnerabilities.
- Pin images appropriately.
- Rebuild when security updates become available.

## GitHub Actions as dependencies

Third-party GitHub Actions are dependencies and should be reviewed accordingly.

Consider:

- Publisher reputation.
- Maintenance activity.
- Required permissions.
- Version pinning.
- Whether the Action executes third-party code.
- Whether a simpler native workflow can replace it.

Avoid granting broad token permissions to workflows unnecessarily.

## Dependency review cadence

Dependency health should be included in repository health reviews.

Review:

- Available updates.
- Security alerts.
- Unsupported versions.
- Update automation.
- Failed dependency pull requests.
- Abandoned dependencies.

## Related guidance

- [Repository Health](./repository-health.md)
- [Security Readiness](./security-readiness.md)
- [OpenSSF Scorecard](./openssf-scorecard.md)
- [Upstream Contributions](../contributing/upstream-contributions.md)
