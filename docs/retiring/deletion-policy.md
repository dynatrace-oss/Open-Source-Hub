# Repository Deletion Policy

Repository deletion is a permanent action and should be used more cautiously than archival.

Dynatrace public repositories should generally be **archived rather than deleted** when they contain meaningful project history, releases, contributors, users, or documentation value.

Deletion is appropriate when keeping the repository provides little or no ongoing value, or when continued public availability creates unnecessary legal, security, operational, or governance risk.

## When deletion may be appropriate

A repository may be considered for deletion when it:

- Was created accidentally.
- Was created only for temporary testing.
- Contains no meaningful project history.
- Is empty or effectively unused.
- Duplicates another repository without meaningful unique history.
- Is an unnecessary fork with no Dynatrace-specific changes.
- Was created for a short-lived process that no longer exists.
- Contains content that should not remain publicly accessible.
- Presents legal, security, confidentiality, or intellectual property concerns that cannot be adequately addressed through normal remediation.
- Has been replaced and provides no continuing historical or community value.

Deletion should not be used simply because a repository is inactive.

See [Repository Archive Policy](./archive-policy.md) when the repository has historical or ongoing reference value.

## Archive or delete?

Use the following questions before choosing deletion.

### Does the repository have meaningful history?

Examples include:

- Releases.
- Issues.
- Pull requests.
- Contributors.
- Forks.
- Stars.
- Packages.
- Documentation links.
- External users.

If yes, **archive is usually preferable**.

### Is the repository referenced externally?

Check for:

- Product documentation.
- Blog posts.
- Tutorials.
- Customer documentation.
- Package managers.
- Community discussions.
- CI/CD configurations.
- Other repositories.

If external references exist, determine whether they must be updated before deletion.

### Does anyone still depend on it?

Consider:

- Product teams.
- Customers.
- Partners.
- Internal automation.
- External integrations.
- Package consumers.
- Community contributors.

Do not delete a repository until known dependencies have been evaluated.

### Is there a successor?

If another repository replaces the project, consider archiving the original repository and linking users to the successor instead of deleting it.

### Is there a security or legal reason to remove it?

If the repository contains information that should not remain public, deletion may be necessary.

However, deleting the repository may not fully remove:

- Forks.
- Clones.
- Published packages.
- Cached content.
- Previously downloaded artifacts.
- Copies in external systems.

Follow the appropriate security, legal, or incident-response process when sensitive information has been exposed.

## Before deletion

Complete the following review.

### Ownership

- Confirm the current or most recent owning team.
- Confirm the maintainers.
- Identify the person or team requesting deletion.
- Document why deletion is being requested.

### Repository activity

Review:

- Recent commits.
- Open issues.
- Open pull requests.
- Releases.
- Tags.
- Packages.
- Discussions.
- Contributors.
- Forks.

### Dependencies

Identify whether the repository is referenced by:

- Other Dynatrace repositories.
- GitHub Actions.
- Build pipelines.
- Deployment automation.
- Documentation.
- Package managers.
- External services.
- Customer or partner integrations.

### External users

Where practical, assess whether users or contributors are still relying on the project.

A repository with external users should generally receive deprecation or archival notice before removal unless immediate deletion is required for security or legal reasons.

## Backup and retention

Before deleting a repository, determine whether its contents or history must be retained.

Where appropriate, preserve:

- Git history.
- Releases.
- Important issues or pull requests.
- Documentation.
- Governance records.
- Decision records.

Backups should be stored in an approved location appropriate to the reason for retention.

Do not create an unmanaged private copy solely to avoid completing the lifecycle decision.

## Packages and releases

Repository deletion may affect related artifacts.

Before deletion, review:

- GitHub Releases.
- GitHub Packages.
- Container images.
- Language package registries.
- Marketplace listings.
- Download links.

Determine whether artifacts should:

- Remain available.
- Be deprecated.
- Be redirected.
- Be removed.

Package consumers should not unexpectedly lose access because the source repository was deleted without considering distribution dependencies.

## Automation and integrations

Before deletion, review and remove or update:

- GitHub Actions.
- Webhooks.
- GitHub Apps.
- Deploy keys.
- Repository secrets.
- Environment secrets.
- External service integrations.
- Scheduled jobs.
- CI/CD references.

Ensure that deleting the repository will not break unrelated automation.

## Documentation and links

Before deletion:

- Update Dynatrace documentation.
- Update links from other repositories.
- Update internal guidance.
- Update external landing pages where applicable.
- Update references to successor projects.

If the repository has been publicly referenced, consider using an archival period before deletion so users have time to migrate.

## Community communication

When a repository has an active or historical external community, communicate the lifecycle change where practical.

Communication may include:

- A README notice.
- A final release notice.
- A GitHub Discussion or Issue.
- Documentation updates.
- Migration guidance.

For repositories with meaningful community history, archival is usually preferable because it preserves these references.

## Approval

Deletion requires confirmation that:

- The owning team agrees with deletion, or ownership has been determined to be abandoned.
- Known dependencies have been reviewed.
- Archival has been considered.
- Required security, legal, or governance review has occurred where applicable.
- Required backups have been completed.
- Relevant documentation has been updated.

High-impact or unclear deletion requests should be escalated for repository lifecycle review before action is taken.

## Deletion checklist

- [ ] Repository owner or owning team has been identified.
- [ ] Reason for deletion is documented.
- [ ] Archive versus delete decision has been reviewed.
- [ ] Open issues have been reviewed.
- [ ] Open pull requests have been reviewed.
- [ ] Releases and tags have been reviewed.
- [ ] Packages have been reviewed.
- [ ] Forks and contributors have been considered.
- [ ] Known internal dependencies have been reviewed.
- [ ] Known external dependencies have been reviewed.
- [ ] External documentation links have been reviewed.
- [ ] Required migration guidance has been provided.
- [ ] Required backups have been completed.
- [ ] Repository secrets have been reviewed.
- [ ] Webhooks and integrations have been reviewed.
- [ ] CI/CD and automation references have been removed or updated.
- [ ] Security or legal review has been completed where necessary.
- [ ] Required lifecycle approval has been received.
- [ ] Repository inventory has been updated.

## After deletion

After the repository is deleted:

- Record the deletion date.
- Record the reason for deletion.
- Record the approving team or owner.
- Update the public repository inventory.
- Confirm that related automation still functions.
- Confirm documentation no longer points to the deleted repository.

## Related guidance

- [Repository Lifecycle](../governance/repository-lifecycle.md)
- [Archive Policy](./archive-policy.md)
- [Archive Checklist](./archive-checklist.md)
