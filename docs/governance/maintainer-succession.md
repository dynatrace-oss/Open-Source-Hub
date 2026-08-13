# Maintainer Succession

Every active public repository should have clear and sustainable maintainer ownership.

Maintainer succession is the process for transferring repository responsibility when a maintainer changes roles, leaves a team, leaves Dynatrace, or can no longer actively support the project.

The goal is to prevent repositories from becoming dependent on a single person or appearing actively maintained when no responsible maintainer remains.

---

## Why maintainer succession matters

A repository without active maintainers can create:

- Unreviewed pull requests.
- Unanswered issues.
- Delayed security response.
- Stale dependencies.
- Broken automation.
- Unclear release ownership.
- Confusion about support expectations.
- Increased risk of abandonment.

Maintainer succession should be planned before ownership becomes unclear.

---

## Minimum ownership expectations

Every active repository should have:

- A clearly identified owning team.
- At least one active maintainer.
- A backup maintainer or documented succession path.
- Current `CODEOWNERS` entries.
- A support model that reflects actual maintainer capacity.

Where practical, repository ownership should be team-based rather than dependent on a single individual.

---

## When succession should be triggered

Maintainer succession should be reviewed when:

- A maintainer changes teams.
- A maintainer changes roles.
- A maintainer leaves Dynatrace.
- A maintainer is no longer able to support the project.
- The owning team changes.
- The repository is transferred.
- Pull requests or issues are consistently waiting for maintainer action.
- Repository ownership becomes unclear.
- A lifecycle review identifies insufficient maintainer capacity.

Succession should also be considered proactively for projects that rely heavily on one maintainer.

---

## Maintainer responsibilities during transition

Where possible, the outgoing maintainer should help transfer:

- Repository context.
- Technical knowledge.
- Release processes.
- Automation ownership.
- Security responsibilities.
- External community relationships.
- Upstream relationships.
- Known technical debt.
- Current issues and pull requests.
- Future roadmap context.

The goal is to transfer operational knowledge, not only GitHub permissions.

---

## Identifying a successor

A successor should be someone who:

- Has appropriate technical knowledge or can reasonably develop it.
- Understands the project's purpose.
- Has capacity to maintain the repository.
- Has support from the owning team.
- Understands the repository's support model.
- Can participate in issue and pull request review.
- Can respond to repository health and security concerns.

For strategic or high-impact repositories, avoid relying on a single successor where possible.

---

## Team-based ownership

Where practical, prefer GitHub teams over individual accounts for repository ownership and review responsibilities.

For example:

```text
@Dynatrace/example-maintainers
```

is generally preferable to:

```text
@individual-user
```

Team-based ownership can reduce disruption when individuals change roles.

Individual maintainers may still be listed where useful, but the repository should not depend solely on one person's account.

---

## CODEOWNERS

Review `CODEOWNERS` whenever maintainer responsibility changes.

Update entries that reference:

- Former maintainers.
- Teams that no longer own the project.
- Individuals who have changed roles.
- Groups that no longer exist.

Confirm that new owners can actually review the paths assigned to them.

A valid `CODEOWNERS` file should reflect current responsibility, not historical ownership.

---

## Repository permissions

During succession, review:

- Admin access.
- Maintain access.
- Write access.
- GitHub teams.
- External collaborators.
- Deploy keys.
- GitHub Apps.
- Machine accounts.

Remove access that is no longer needed and grant the minimum permissions required by the new maintainer model.

See [Contributor Access](./contributor-access.md).

---

## Security responsibilities

Maintainer succession should include transfer of security responsibilities.

Confirm that the new maintainer or owning team understands:

- How vulnerabilities are reported.
- Who receives security reports.
- How security issues are triaged.
- Who coordinates remediation.
- How releases are published.
- Which credentials or automation are security-sensitive.

Security ownership should not remain with a person who no longer maintains the repository.

---

## Release ownership

If the repository publishes releases, document:

- Who can publish releases.
- How releases are created.
- Which automation is involved.
- Where release credentials are managed.
- How package publishing works.
- Any signing or provenance requirements.

Verify that the successor can complete the release process before removing the previous maintainer's access.

---

## Community relationships

Some maintainers hold important relationships with:

- External contributors.
- Upstream maintainers.
- Open source foundations.
- Partner communities.
- Customers using the project.

Where relevant, include these relationships in the transition.

A maintainer change should not unnecessarily disrupt established community collaboration.

---

## When no successor can be identified

If no qualified or available successor exists, do not leave the repository appearing normally maintained.

The owning team should complete a lifecycle review and consider:

- Recruiting additional maintainers.
- Moving to community-supported status.
- Moving to maintenance-only status.
- Transferring the repository.
- Deprecating the project.
- Archiving the repository.

See [Repository Lifecycle](./repository-lifecycle.md).

---

## Abandoned ownership

A repository may be considered at risk when:

- The owning team no longer exists.
- Named maintainers are inactive.
- No one can approve pull requests.
- Security ownership is unclear.
- Releases can no longer be produced.
- No team accepts responsibility for the project.

These repositories should be prioritized for lifecycle review.

Inactivity alone should not automatically result in archival, but unresolved ownership is a significant governance concern.

---

## Succession checklist

### Ownership

- [ ] Owning team has been confirmed.
- [ ] Outgoing maintainer has been identified.
- [ ] Successor maintainer has been identified.
- [ ] Backup maintainer or succession path exists.
- [ ] Support model remains accurate.

### Access

- [ ] New maintainer permissions have been granted.
- [ ] Former maintainer permissions have been reviewed.
- [ ] GitHub team membership has been updated.
- [ ] `CODEOWNERS` has been updated.
- [ ] External collaborator access has been reviewed.

### Knowledge transfer

- [ ] Repository purpose has been reviewed.
- [ ] Current roadmap or priorities have been reviewed.
- [ ] Open issues and pull requests have been reviewed.
- [ ] Release process has been documented.
- [ ] Automation has been reviewed.
- [ ] Dependencies and known technical debt have been reviewed.
- [ ] Security responsibilities have been transferred.
- [ ] Relevant upstream or community relationships have been transferred.

### Validation

- [ ] New maintainer can approve or merge pull requests.
- [ ] New maintainer can manage releases where required.
- [ ] Required automation still works.
- [ ] Repository documentation reflects current ownership.
- [ ] Public repository inventory has been updated.

---

## After succession

After the transition:

- Update maintainer documentation.
- Update `CODEOWNERS`.
- Remove obsolete access.
- Update the public repository inventory.
- Confirm the repository support model.
- Monitor the transition for unresolved ownership gaps.

Succession is complete when the repository has sustainable ownership, not simply when GitHub permissions have changed.

---

## Related guidance

- [Repository Lifecycle](./repository-lifecycle.md)
- [Support Models](./support-models.md)
- [Contributor Access](./contributor-access.md)
- [Maintainer Guide](../maintaining/maintainer-guide.md)
- [Repository Health](../maintaining/repository-health.md)
