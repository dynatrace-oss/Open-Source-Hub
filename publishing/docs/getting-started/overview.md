# Open Source at Dynatrace: Overview

Dynatrace participates in open source as a contributor, maintainer, consumer, and ecosystem partner.

The Open Source Hub provides a consistent way to create, publish, maintain, support, and retire public open source repositories managed by Dynatrace.

Its goal is to make open sourcing easier to do well by giving teams clear standards, reusable guidance, and predictable lifecycle expectations.

## Who this guidance is for

This guidance is intended for:

- Dynatrace employees creating or maintaining public repositories.
- Teams preparing private repositories for public release.
- Maintainers responsible for public project health.
- Customers and partners contributing to community-supported projects.
- External contributors working with Dynatrace open source repositories.

## What this Hub covers

The Hub provides guidance for the full public repository lifecycle:

**Propose → Create → Prepare → Publish → Maintain → Transfer → Archive → Delete**

It includes standards for:

- Repository creation.
- Private-to-public transitions.
- Repository transfers.
- Support models.
- Repository ownership.
- Contributor access.
- Security disclosures.
- Maintainer succession.
- Archival and deletion.

It also provides reusable:

- Repository templates.
- README guidance.
- Contribution guidance.
- Security guidance.
- Support disclaimers.
- Publishing checklists.
- Archive checklists.

## Core principles

### Open source should have a purpose

A public repository should exist because it creates meaningful value for users, contributors, customers, partners, or an external ecosystem.

Creating a repository is not, by itself, an open source strategy.

Before creating something new, consider whether the work would be more useful:

- In an existing Dynatrace repository.
- In an existing external project.
- As an upstream contribution.
- As documentation or examples within an established project.

### Public from the beginning

If a repository is expected to become public, public repository standards should be considered when it is created.

Teams should not wait until publication to address:

- Licensing.
- Documentation.
- Security.
- Ownership.
- Support expectations.
- Contribution models.

Designing for public use early reduces publication delays and unnecessary remediation.

### Ownership is required

Every active public repository should have:

- An owning team.
- An accountable maintainer.
- A succession path.
- A defined support model.

Open source repositories should not depend indefinitely on the availability or interest of one individual.

### Support expectations should be explicit

A public Dynatrace repository is not automatically covered by standard Dynatrace product support.

Projects may be:

- Officially supported.
- Community-supported.
- Experimental.
- Maintenance-only.
- Deprecated.
- Archived.

The repository must make its support status easy for users to understand.

### Contribute upstream where it makes sense

Creating a Dynatrace-specific repository is not always the best outcome.

Where practical, teams should consider whether the work can be contributed directly to an existing upstream project.

Upstream contribution can:

- Reduce long-term maintenance.
- Improve interoperability.
- Strengthen ecosystems that Dynatrace depends on.
- Avoid unnecessary forks.
- Make improvements available to a broader community.

### Sustainability matters

Publishing a project creates ongoing responsibilities.

Before publication, teams should consider:

- Maintenance capacity.
- Security response.
- Dependency updates.
- Issue and pull request review.
- Releases.
- Documentation.
- Community expectations.
- Maintainer succession.

If those responsibilities can no longer be sustained, the repository should move through lifecycle review rather than remain indefinitely without clear ownership.

## Where to start

### I have an idea for a new project

Start with:

[Should This Be Open Source?](should-this-be-open-source.md)

Then determine:

[Where Does My Repository Belong?](where-does-my-repo-belong.md)

### I already have a private repository

See:

[Private-to-Public Transition](../publishing/private-to-public.md)

### I am creating a new repository

See:

[New Repository Requirements](../publishing/new-repositories.md)

### I need to understand support expectations

See:

[Support Models](../governance/support-models.md)

### I think a repository should be retired

See:

[Repository Archive Policy](../retiring/archive-policy.md)

## Need help?

If you are unsure which path applies, open an Open Source Hub request before creating or publishing the repository.

Early review is preferable to remediation immediately before launch.
