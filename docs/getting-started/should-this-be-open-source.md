# Should This Be Open Source?

Open sourcing a project creates an ongoing public commitment.

Before publishing code, documentation, tooling, examples, or other assets, determine whether open source is the right model.

## Open source may be appropriate when

A project:

- Solves a problem that exists beyond a single internal team.
- Benefits customers, partners, developers, or an external technical ecosystem.
- Can benefit from external collaboration.
- Supports an ecosystem important to Dynatrace.
- Provides reusable examples, tooling, SDKs, integrations, or reference implementations.
- Can be maintained publicly over time.
- Can be published without exposing confidential information or intellectual property.
- Has a clear owner and maintainer.

## Open source may not be appropriate when

A project:

- Exists only for internal operations.
- Contains internal infrastructure or architecture information.
- Contains customer information.
- Contains secrets or credentials.
- Depends heavily on internal-only systems.
- Has no team willing to maintain it.
- Has unclear ownership.
- Cannot legally be redistributed.
- Duplicates an existing upstream or Dynatrace project without a clear reason.
- Would create support expectations the owning team cannot meet.

## Questions to answer before proceeding

### Purpose

- What problem does this project solve?
- Who is the intended audience?
- Why should it be public?
- What value does publishing it create?

### Existing alternatives

- Does an existing Dynatrace repository already solve this problem?
- Does an upstream project exist where the work could be contributed instead?
- Would documentation or an example within an existing repository be sufficient?

Prefer contributing upstream where doing so provides equivalent or greater ecosystem value.

### Ownership

Identify:

- Owning team.
- Primary maintainer.
- Backup maintainer or succession path.

A public repository should not depend indefinitely on one individual's interest or availability.

### Support

Determine whether the project will be:

- Officially supported.
- Community-supported.
- Experimental.

See [Support Models](../governance/support-models.md).

### Sustainability

Consider:

- Expected maintenance effort.
- Dependency updates.
- Security response.
- Issue and pull request review.
- Releases.
- Documentation updates.
- Maintainer succession.

Publishing is the beginning of the repository lifecycle, not the end of the launch process.

## Decision

If open source is appropriate, continue to:

[New Repository Requirements](../publishing/new-repositories.md)

If the project already exists privately, continue to:

[Private-to-Public Transition](../publishing/private-to-public.md)
