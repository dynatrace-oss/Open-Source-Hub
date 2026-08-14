# Repository Lifecycle
![Dynatrace public repository lifecycle from proposal through transfer or archival](../../assets/images/repository-lifecycle.png)
Dynatrace public repositories should follow a deliberate lifecycle from proposal through retirement.

The lifecycle exists to make open sourcing easier while ensuring that public repositories remain understandable, owned, secure, and sustainable.

## Lifecycle stages

### 1. Propose

Determine:

- Why the repository should exist.
- Why it should be public.
- Intended audience.
- Owning team.
- Maintainers.
- Support model.
- Appropriate GitHub organization.
- Expected maintenance commitment.

### 2. Create

Create the repository using approved repository standards and templates.

Repositories intended for future public release should follow public requirements from the beginning.

Avoid creating a minimally configured private repository and postponing governance until publication.

### 3. Prepare

Before publication:

- Complete required documentation.
- Select an approved license.
- Review repository history.
- Configure ownership.
- Define support expectations.
- Configure security and dependency automation.
- Remove confidential or internal-only content.

### 4. Publish

Complete the publishing checklist and required reviews.

Publication changes the audience and risk profile of a repository. Making a private repository public should therefore be treated as a release, not simply a visibility-setting change.

### 5. Maintain

Maintainers are responsible for:

- Repository health.
- Security.
- Dependencies.
- Documentation.
- Releases where applicable.
- Issues and pull requests.
- Support expectations.
- Ownership continuity.

### 6. Transfer

Repositories may move:

- Between Dynatrace organizations.
- Into Dynatrace.
- To an external organization.
- To an upstream project or foundation.

Transfers require ownership, security, automation, licensing, and community review.

### 7. Archive

Archive a repository when active development has ended but historical content should remain publicly available.

Archival should normally be preferred over deletion for repositories with meaningful history or users.

### 8. Delete

Deletion is appropriate only when retaining the repository provides little value or creates unnecessary risk.

Examples include:

- Accidental repositories.
- Empty test repositories.
- Temporary repositories with no meaningful history.
- Unnecessary forks with no unique Dynatrace content.

## Required lifecycle metadata

Every active public repository should be able to answer:

- What is this project?
- Who owns it?
- Who maintains it?
- What is its support model?
- What is its lifecycle status?
- How are vulnerabilities reported?
- How are contributions handled?
- What happens if the current maintainers stop maintaining it?

## Lifecycle review

Lifecycle review may be triggered by:

- No meaningful activity for approximately 12 months.
- Loss of maintainers.
- Product retirement.
- Project replacement.
- Community inactivity.
- Major strategic changes.
- Security concerns.
- Long-term maintenance burden.
- Completion of an experimental project.

Inactivity should trigger review, not automatic archival.

A stable library or SDK may require little activity while still providing value.

## Possible review outcomes

A lifecycle review may result in:

- Continue active development.
- Increase strategic investment.
- Move to community support.
- Move to maintenance-only.
- Assign new maintainers.
- Transfer ownership.
- Deprecate.
- Archive.
- Delete.
