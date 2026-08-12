# Repository Template

Dynatrace provides a standard repository template to help teams create public repositories with a consistent baseline for documentation, governance, security, and contribution readiness.

Use the existing repository template when creating a new repository that is intended to become public.

> **Template:** Replace the link below with the location of the approved Dynatrace repository template.
>
> [Use the Dynatrace Repository Template]((https://github.com/dynatrace-oss/oss-repository-template))

## When to use the template

Use the repository template when:

- Creating a new public open source repository.
- Creating a private repository that is expected to become public later.
- Rebuilding or standardizing an existing repository before publication.
- Establishing a new community-supported or experimental project.

If a repository already exists, do not recreate it solely to use the template. Instead, compare the repository against the current requirements and add or update the required files and settings.

See:

- [New Repository Requirements](../../publishing/new-repositories.md)
- [Private-to-Public Transition](../../publishing/private-to-public.md)
- [Publishing Checklist](../../publishing/publishing-checklist.md)

## What the template is intended to provide

The template should establish a consistent starting point for public repositories, including the files and configuration needed to support:

- Clear project purpose.
- Repository ownership.
- Contribution guidance.
- Security reporting.
- Licensing.
- Support expectations.
- GitHub collaboration workflows.
- Repository automation.

The template is a starting point, not a substitute for repository-specific review.

## Required customization

After creating a repository from the template, update all placeholder content before publication.

At minimum, review and customize the following.

### README

Update the README to describe:

- What the project does.
- Who it is for.
- Project status.
- Support model.
- Getting-started instructions.
- Contribution pathway.
- Security reporting pathway.
- License.

See [README Requirements](../templates/readme-template.md).

### Ownership

Confirm:

- Owning team.
- Primary maintainer.
- Backup maintainer or succession path.
- CODEOWNERS entries.

Do not leave template owners or placeholder teams in the repository.

### Support model

Select and document the appropriate support model:

- Officially supported.
- Community-supported.
- Experimental.

If the project later moves into maintenance-only, deprecated, or archived status, update the repository documentation accordingly.

See [Support Models](../governance/support-models.md).

### License

Confirm that the repository contains the approved license for the project.

Do not assume the default template license is appropriate for every project.

### Security

Review and customize `SECURITY.md`.

Ensure that:

- The approved vulnerability reporting channel is listed.
- Security reports are not directed to public GitHub Issues.
- Version-specific support information is accurate where applicable.

See [Security Guidance](../templates/security-template.md).

### Contribution guidance

Update `CONTRIBUTING.md` to reflect the actual contribution workflow.

Document where applicable:

- Development setup.
- Testing expectations.
- Pull request requirements.
- Issue workflow.
- Code style.
- Documentation expectations.
- Sign-off, CLA, or DCO requirements.

Remove contribution instructions that do not apply.

### CODEOWNERS

Update `CODEOWNERS` to reflect the teams responsible for reviewing and maintaining the repository.

Prefer team ownership over individual accounts where practical.

### GitHub configuration

Review all inherited repository settings and automation, including:

- Branch protections or rulesets.
- GitHub Actions.
- Workflow token permissions.
- Dependabot or other dependency automation.
- Issue templates.
- Pull request templates.
- Release automation.
- Repository topics.
- Repository description.

Template defaults should not be assumed to be correct for every repository.

## Template placeholders

Before publication, search the repository for:

- Placeholder project names.
- Example owners.
- Example team names.
- Placeholder support language.
- Placeholder URLs.
- Example security contacts.
- TODO markers.
- Template-specific comments.

No placeholder content should remain in a published repository unless it is intentionally part of the project.

## Additional files

The template provides a baseline.

Some repositories may need additional documentation, such as:

- Architecture documentation.
- Maintainer guide.
- Governance model.
- Release process.
- Compatibility matrix.
- Changelog.
- Roadmap.
- Migration guidance.
- API documentation.

Add these when they materially help users or maintainers understand and operate the project.

## Before publication

Creating a repository from the standard template does **not** automatically make it ready for public release.

Before publishing, complete the:

[Publishing Checklist](../../publishing/publishing-checklist.md)

The owning team remains responsible for the technical content, ownership, support model, security readiness, and long-term maintenance of the repository.
