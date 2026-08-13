# Contributor Access

Public repositories should follow least-privilege principles when granting GitHub access.

Most contributors do not need direct write access to participate in a Dynatrace open source project. External and internal contributors should generally contribute through issues, forks, branches, and pull requests.

Elevated repository access should be granted only when there is a clear project need.

---

## Access principles

Repository access should follow these principles:

### Least privilege

Grant only the level of access required to perform the person's responsibilities.

### Role-based access

Where practical, use GitHub teams rather than granting permissions directly to individual users.

### Reviewable access

Repository permissions should be understandable and periodically reviewable.

### Temporary when appropriate

Access granted for a temporary responsibility should be removed when that responsibility ends.

### Ownership is not contribution

Being an active contributor does not automatically require or justify elevated repository permissions.

---

## Typical contribution model

For most contributors, the expected workflow is:

```text
Issue / Fork / Branch → Pull Request → Review → Merge
```

External contributors should normally contribute through forks and pull requests.

Dynatrace employees who are not maintainers should also use the repository's standard review process unless a documented workflow requires otherwise.

---

## Access levels

Repository access should be aligned with responsibility.

### Read

Appropriate for people who need visibility into non-public repository content where applicable but do not need to modify it.

For public repositories, read access generally does not need to be explicitly granted.

### Triage

May be appropriate for contributors who help with:

- Issue management.
- Labels.
- Discussions.
- Community triage.

Triage access does not normally require code merge permissions.

### Write

May be appropriate for active contributors who need to:

- Push branches.
- Manage issues.
- Participate in repository operations.

Write access should not be granted simply for convenience.

### Maintain

Appropriate for maintainers responsible for day-to-day repository management without requiring full administrative control.

### Admin

Admin access should be limited to people who need to manage:

- Repository settings.
- Access.
- Security configuration.
- Rulesets.
- Integrations.
- Repository transfer or deletion.

Admin access should be tightly controlled.

---

## Internal contributors

Dynatrace employees should not automatically receive write or admin access to public repositories.

Access should be based on:

- Project responsibility.
- Maintainer role.
- Operational need.
- Release responsibility.
- Required review or automation duties.

Where practical, internal access should be managed through GitHub teams.

---

## External contributors

External contributors should generally not require direct repository access.

Normal contribution mechanisms include:

- Forking the repository.
- Opening pull requests.
- Opening issues.
- Participating in Discussions.
- Reviewing public changes.

Direct write or maintain access may be appropriate for established external maintainers when:

- They have demonstrated sustained contribution.
- Their role requires elevated access.
- The project's governance supports external maintainership.
- Existing maintainers sponsor the access.
- Security and least-privilege considerations have been reviewed.

External maintainer access should be documented.

---

## Becoming a maintainer

Contributor access should not be treated as a substitute for a maintainer selection process.

A contributor may be considered for maintainer responsibilities based on:

- Sustained participation.
- Technical knowledge.
- Constructive review activity.
- Reliability.
- Understanding of project scope.
- Community behavior.
- Ability to support long-term maintenance.

The owning team or project governance model should approve maintainer access.

See [Maintainer Succession](./maintainer-succession.md).

---

## GitHub teams

Prefer team-based access where practical.

Teams can help:

- Make ownership visible.
- Simplify access reviews.
- Reduce dependence on individual accounts.
- Support maintainer succession.
- Apply consistent permissions across repositories.

Avoid creating broad teams with unnecessary access to large numbers of repositories.

Teams should have a clear purpose and owner.

---

## CODEOWNERS and access

`CODEOWNERS` identifies who should review changes, but it does not itself grant repository permissions.

Confirm that CODEOWNERS entries:

- Reference valid users or teams.
- Reflect current ownership.
- Have the required access.
- Are updated when ownership changes.

Avoid leaving former maintainers or inactive teams in `CODEOWNERS`.

---

## Administrative access

Admin access should be restricted to people who need to perform administrative tasks.

Examples include:

- Managing repository permissions.
- Configuring rulesets.
- Managing GitHub Apps.
- Transferring repositories.
- Archiving repositories.
- Deleting repositories.
- Managing security settings.

Day-to-day maintainers may not need admin access.

---

## Machine and automation access

Repository access may also be granted to:

- GitHub Apps.
- Bots.
- Service accounts.
- CI/CD systems.
- Release automation.

Automation should use:

- The minimum required permissions.
- Managed credentials.
- Appropriate token scopes.
- GitHub Apps instead of personal credentials where practical.

Avoid using personal access tokens as long-term shared automation credentials when an appropriate managed alternative exists.

Review machine access periodically.

---

## Personal accounts

Repository access should be associated with identifiable individual accounts or approved automation identities.

Do not share GitHub credentials between maintainers.

Access should be attributable to the person or system performing the action.

---

## Access reviews

Repository permissions should be reviewed periodically and when:

- A maintainer changes roles.
- A team changes ownership.
- A contributor becomes inactive.
- A repository is transferred.
- A project changes support model.
- A security incident occurs.
- A repository enters maintenance-only or archival review.

Review:

- Admins.
- Maintainers.
- Write access.
- External collaborators.
- GitHub teams.
- GitHub Apps.
- Deploy keys.
- Machine accounts.

Remove access that is no longer justified.

---

## Access during repository transfer

Transfers may change how GitHub teams and organization permissions apply.

Before and after transfer:

- Review current collaborators.
- Identify required destination teams.
- Reapply appropriate permissions.
- Update `CODEOWNERS`.
- Review external collaborators.
- Validate automation identities.

See [Repository Transfers](../publishing/repository-transfers.md).

---

## Access during maintainer succession

When maintainer responsibility changes:

- Grant the successor required access.
- Confirm they can review and merge changes.
- Confirm release access where needed.
- Update GitHub teams.
- Update `CODEOWNERS`.
- Remove obsolete permissions.

Do not remove the previous maintainer's access until required knowledge and operational responsibility have been transferred, unless immediate removal is required for security reasons.

See [Maintainer Succession](./maintainer-succession.md).

---

## Access for archived repositories

Archived repositories generally should not require ongoing write or maintain access.

Before archival:

- Review collaborators.
- Remove unnecessary elevated access.
- Remove unused machine access.
- Review GitHub Apps and webhooks.
- Remove unnecessary credentials or deploy keys.

Retain only access needed for appropriate administrative or governance purposes.

---

## Access checklist

When granting elevated access:

- [ ] The project need is documented or understood.
- [ ] The minimum required access level has been selected.
- [ ] Team-based access has been considered.
- [ ] Maintainer approval has been received where appropriate.
- [ ] External collaborator implications have been reviewed.
- [ ] Security implications have been considered.
- [ ] Access duration has been considered.
- [ ] `CODEOWNERS` has been updated if necessary.

When removing access:

- [ ] Current project responsibilities have been confirmed.
- [ ] Replacement ownership exists where necessary.
- [ ] Release responsibilities have been transferred.
- [ ] Automation dependencies have been reviewed.
- [ ] `CODEOWNERS` has been updated.
- [ ] Team membership has been updated.
- [ ] Machine or token access has been reviewed.

---

## Access issues

If repository access is unclear or no current team can determine who should have elevated permissions, treat the issue as a governance and ownership problem rather than simply granting additional access.

Confirm:

1. Who owns the repository.
2. Who maintains it.
3. What support model applies.
4. What access is actually required.

If ownership cannot be resolved, initiate a repository lifecycle review.

---

## Related guidance

- [Maintainer Succession](./maintainer-succession.md)
- [Repository Lifecycle](./repository-lifecycle.md)
- [Support Models](./support-models.md)
- [Maintainer Guide](../maintaining/maintainer-guide.md)
- [Repository Transfers](../publishing/repository-transfers.md)
- [Security Readiness](../maintaining/security-readiness.md)
