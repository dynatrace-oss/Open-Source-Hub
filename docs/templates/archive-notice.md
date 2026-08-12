# Archive Notice

Use this notice when a repository has been archived and is no longer actively maintained.

Place the notice near the top of the repository `README.md` so users can immediately understand the repository's status.

## Standard archive notice

> **Archived**
>
> This project is no longer actively maintained. The repository remains available for reference, but no additional features, fixes, or support should be expected.

## Archive notice with a replacement

> **Archived**
>
> This project is no longer actively maintained. Development has moved to [replacement project].
>
> This repository remains available for reference, but no additional features, fixes, or support should be expected. Users should migrate to the replacement project where possible.

## Deprecated before archival

Use this version when users should move away from the project before the repository is fully archived.

> **Deprecated**
>
> This project is no longer recommended for new implementations and is expected to be archived.
>
> Please use [replacement project] instead. Existing users should review the available migration guidance before transitioning.

## Maintenance-only before archival

Use this when active feature development has stopped but limited maintenance is still expected.

> **Maintenance Mode**
>
> This project is currently in maintenance mode. Critical fixes, security updates, or compatibility updates may be provided, but active feature development should not be expected.
>
> The project may be archived in the future if ongoing maintenance is no longer justified.

## Include a successor when one exists

If the repository has a clear successor, include:

- The successor project name.
- A link to the successor repository or documentation.
- Migration guidance where applicable.
- The date the repository entered archival or deprecation status, if useful.

Example:

> **Archived — August 2026**
>
> This project is no longer actively maintained.
>
> Development has moved to [Project Name](https://github.com/example/project).
>
> Existing users should review the [migration guide](LINK-TO-MIGRATION-GUIDE).
>
> This repository remains available for historical reference.

## Support expectations

Archived repositories should not imply continued support.

If the project was previously officially supported, clarify whether users should:

- Migrate to another supported project.
- Contact Dynatrace Support for an existing supported product.
- Refer only to historical documentation.

Example:

> This repository is archived and is no longer receiving updates. For currently supported functionality, see [replacement documentation].

## Before adding the archive notice

Confirm that:

- The owning team agrees with archival.
- Open issues and pull requests have been reviewed.
- A successor is identified where applicable.
- External documentation has been updated.
- Migration guidance is available where needed.
- Unnecessary automation and secrets have been removed.

See:

- [Archive Policy](../retiring/archive-policy.md)
- [Archive Checklist](../retiring/archive-checklist.md)
- [Repository Lifecycle](../governance/repository-lifecycle.md)
