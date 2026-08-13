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
