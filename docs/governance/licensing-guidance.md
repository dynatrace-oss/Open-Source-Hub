# Open Source Licensing Guidance

This guidance helps Dynatrace project teams identify licensing considerations
before publishing, contributing, transferring, or redistributing open source
software.

It is intended to support consistent decision-making and help teams recognize
when additional review is required.

This document does not provide legal advice or independently authorize
publication.

---

## Purpose

Open source licensing determines how software may be used, modified,
redistributed, and combined with other software.

Before code is made public, project teams should understand:

- What license applies to the project.
- Whether Dynatrace has the right to publish the code.
- Whether third-party code introduces additional obligations.
- Whether customer or partner contributions affect ownership.
- Whether redistribution requirements apply.
- Whether existing license notices must be preserved.
- Whether additional review is required before publication.

Licensing questions should be resolved before public release.

---

## Guiding principle

A repository should not be published simply because the code is technically
ready.

The project team should also be able to answer:

> Do we have the right to publish and redistribute this code under the intended
> license?

If the answer is unclear, the project should be marked **Needs Review** until
the licensing question is resolved.

---

## Before publishing a repository

Before publication, identify:

- The intended open source license.
- Who created the code.
- Whether Dynatrace owns or controls the rights required to publish it.
- Whether third-party source code is included.
- Whether code was copied or adapted from another project.
- Whether the repository contains generated or vendored code.
- Whether customer or partner code is included.
- Whether the project is derived from an upstream project.
- Whether required copyright, attribution, or notice files are present.
- Whether dependencies create relevant redistribution obligations.

For an existing private repository, licensing review should include both the
current code and relevant repository history.

---

## Choosing a license

The project team should identify an appropriate open source license before
publication.

The Open Source Hub should not be used to invent or select a license when the
appropriate choice is unclear.

License selection may depend on:

- Project type.
- Intended users.
- Expected contribution model.
- Existing ecosystem conventions.
- Upstream requirements.
- Third-party components.
- Product or distribution context.
- Legal or contractual considerations.

If Dynatrace maintains an approved or preferred license list, project teams
should follow that guidance.

If no approved guidance applies, the project should be marked **Needs Review**
before publication.

---

## License file

Public repositories should include a clear license file when required.

The standard filename is typically:

```text
LICENSE
```

The license file should contain the full text of the applicable license.

Do not modify standard license text unless explicitly required and reviewed.

The repository README should clearly indicate the project's license where
appropriate.

---

## Third-party code

Third-party code requires additional attention.

Examples include:

- Copied source files.
- Vendored libraries.
- Forked code.
- Embedded examples.
- Generated code derived from third-party sources.
- Bundled binaries.
- Modified upstream code.

Before publication, determine:

- The original license.
- Whether redistribution is permitted.
- Whether modification is permitted.
- Whether attribution is required.
- Whether license text must be included.
- Whether copyright notices must be preserved.
- Whether source disclosure or other obligations apply.
- Whether the intended Dynatrace license is compatible with those obligations.

Do not remove third-party copyright or licensing notices unless there is a
documented reason to do so.

If compatibility or redistribution obligations are unclear, mark the project
**Needs Review**.

---

## Dependencies

Using an open source dependency does not automatically mean that the repository
must use the same license as that dependency.

However, dependencies may introduce obligations that need to be understood.

Consider:

- Runtime dependencies.
- Build dependencies.
- Bundled dependencies.
- Vendored dependencies.
- Container images.
- JavaScript packages.
- Go modules.
- Python packages.
- Java dependencies.
- Native libraries.

Pay particular attention when third-party components are redistributed as part
of the project's deliverables.

If a dependency is only referenced and installed separately by the user, the
licensing impact may differ from bundling or redistributing it.

When uncertain, seek review rather than making assumptions.

---

## Forks and upstream projects

When publishing a fork or modified upstream project, preserve the licensing
requirements of the original project.

Before publication:

- Identify the upstream project and license.
- Preserve required license and attribution files.
- Preserve required copyright notices.
- Document Dynatrace-specific modifications where appropriate.
- Confirm whether redistribution of the modified version is permitted.
- Evaluate whether contributing the change upstream is preferable to
  maintaining a long-lived fork.

A fork should not be relicensed unless the project has the legal right to do so.

See
[Upstream Contributions](../contributing/upstream-contributions.md).

---

## Customer-created code

Customer-created code should not automatically be moved into a Dynatrace
repository.

Before Dynatrace publishes or assumes ownership of customer-created code,
consider:

- Who owns the code.
- Whether the customer has granted Dynatrace sufficient rights.
- Whether third-party code is included.
- What license currently applies.
- Whether the customer can legally grant the required rights.
- Who will maintain the project after transfer.
- Whether Dynatrace should own the project at all.

If ownership or publication rights are unclear, the project requires review
before transfer or publication.

See
[Customer and Partner Guidance](../getting-started/customer-and-partner-guidance.md).

---

## Partner-created code

Partner-created integrations and tools should generally retain clear ownership
and support responsibility.

Before transferring or republishing partner-created code under Dynatrace:

- Confirm ownership.
- Confirm publication rights.
- Review the existing license.
- Identify third-party obligations.
- Determine whether relicensing is proposed.
- Confirm who will maintain the project.
- Clarify support expectations.

A desire for increased visibility or branding is not, by itself, sufficient
reason for Dynatrace to assume ownership.

---

## Contributions from external contributors

External contributions may introduce licensing and ownership considerations.

Projects should use the contribution process approved for their repository and
organization.

Before accepting contributions, maintainers should understand:

- Whether a contributor agreement applies.
- Whether a Developer Certificate of Origin or equivalent process applies.
- Whether contribution terms are documented.
- Whether the contribution includes third-party code.
- Whether the contributor has the right to submit the code.

Do not assume that a pull request automatically grants all rights required for
redistribution.

See
[External Contributors](../contributing/external-contributors.md).

---

## Contribution licensing

Repositories should clearly communicate how contributions are licensed.

Where appropriate, contribution guidance should explain that contributions are
provided under the repository's applicable licensing terms or other approved
contribution terms.

Do not create new contribution licensing language without appropriate review.

---

## Copyright notices

Some projects or third-party components may require copyright notices to be
preserved.

Do not remove copyright notices from third-party code without a documented
basis.

Where project-specific copyright guidance exists, follow that guidance
consistently.

---

## NOTICE files

Some licenses or dependencies may require attribution or notice information in
addition to the main license file.

A repository may therefore require:

```text
NOTICE
```

or equivalent attribution documentation.

Whether a NOTICE file is required depends on the project's license,
dependencies, and distribution model.

Do not create or remove NOTICE content solely by assumption.

If requirements are unclear, seek review.

---

## Examples and documentation

Code samples and documentation can also contain licensable material.

Review:

- Example source code.
- Configuration files.
- Tutorials.
- Embedded snippets.
- Images.
- Diagrams.
- Sample datasets.
- Copied documentation.
- Third-party logos or branding.

Do not assume that non-production content is exempt from licensing or usage
requirements.

---

## Generated code

Generated code may still carry licensing obligations depending on its source.

Before publishing generated code, consider:

- What generated it.
- Whether the input source has licensing restrictions.
- Whether the generator applies notices or headers.
- Whether generated output includes third-party material.

If ownership of generated output is unclear, seek review.

---

## Repository history

For private-to-public transitions, licensing review should consider repository
history where relevant.

Past commits may contain:

- Third-party code that has since been removed.
- Copied files.
- Customer or partner content.
- License-incompatible material.
- Internal-only assets.

Removing content from the current branch does not necessarily remove it from
Git history.

See
[Private-to-Public Transition](../publishing/private-to-public.md).

---

## When review is required

Mark the project **Needs Review** when any of the following apply:

- The appropriate license is unclear.
- Ownership of the code is unclear.
- Third-party code is included and obligations are uncertain.
- Relicensing is proposed.
- Customer or partner code is involved.
- The repository contains code from multiple licensing sources.
- Redistribution rights are unclear.
- A dependency may impose additional distribution obligations.
- Copyright or attribution requirements are unclear.
- A fork uses a license the team does not understand.
- Contribution rights are unclear.
- Contractual terms may affect publication.
- The project includes material that Dynatrace may not own.

Do not publish until the unresolved question has been addressed through the
appropriate Dynatrace review process.

---

## What this guidance does not do

This guidance does not:

- Provide legal advice.
- Approve a license.
- Authorize public release.
- Determine license compatibility in complex cases.
- Override upstream license requirements.
- Override contractual obligations.
- Grant Dynatrace rights to third-party, customer, or partner code.
- Replace required Legal or other organizational review.

The purpose of this document is to help teams recognize common licensing
questions early and arrive at the appropriate review with sufficient context.

---

## Publication checklist

Before publication, confirm:

- [ ] The intended license has been identified.
- [ ] The project team understands who owns the code.
- [ ] Dynatrace has the rights required to publish the code.
- [ ] Third-party code has been identified.
- [ ] Relevant third-party licenses have been reviewed.
- [ ] Required attribution and copyright notices are preserved.
- [ ] Any required NOTICE content has been identified.
- [ ] Customer or partner ownership questions have been resolved.
- [ ] Fork or upstream licensing obligations have been reviewed.
- [ ] Contribution licensing expectations are understood.
- [ ] No unresolved licensing questions remain.

If any item cannot be confirmed, mark the project **Needs Review**.

---

## Repository request information

When licensing is relevant to a new repository or publication request, teams
should be prepared to provide:

**Proposed license:**  
[License or "Needs Review"]

**Code ownership:**  
[Dynatrace / upstream / customer / partner / mixed / unknown]

**Third-party code included:**  
Yes / No / Unknown

**Fork or derivative work:**  
Yes / No

**Customer or partner code included:**  
Yes / No

**Relicensing proposed:**  
Yes / No

**Unresolved licensing questions:**  
[Describe any open questions]

This information helps reviewers identify issues before publication rather than
after the repository becomes public.

---

## Related guidance

- [Should This Be Open Source?](../getting-started/should-this-be-open-source.md)
- [Customer and Partner Guidance](../getting-started/customer-and-partner-guidance.md)
- [Repository Lifecycle](./repository-lifecycle.md)
- [New Repository Requirements](../publishing/new-repositories.md)
- [Private-to-Public Transition](../publishing/private-to-public.md)
- [Publishing Checklist](../publishing/publishing-checklist.md)
- [Repository Transfers](../publishing/repository-transfers.md)
- [External Contributors](../contributing/external-contributors.md)
- [Upstream Contributions](../contributing/upstream-contributions.md)
- [Security Readiness](../maintaining/security-readiness.md)

---

## Guiding principle

Licensing should be considered before publication, not after it.

When the answer is clear, document it.

When the answer is unclear, stop and seek review.

Open source publication should be intentional, legally supportable, and
understandable to the people who use and contribute to the project.
