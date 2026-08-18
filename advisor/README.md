# Open Source Project Advisor

The Open Source Project Advisor is a guided AI experience for Dynatrace employees evaluating new or existing open source projects.

It uses the guidance in the Dynatrace Open Source Hub to help determine:

- Whether a project should be open source.
- Whether Dynatrace should own the project.
- Whether work should be contributed upstream.
- Which GitHub organization is the appropriate home.
- Which support model applies.
- Whether ownership and maintainer responsibility are sufficient.
- Whether the project is ready for publication.
- What remains before a repository request can be submitted.

## Operating model

```text
Idea
  ↓
Guided assessment
  ↓
Open source recommendation
  ↓
Publication readiness
  ↓
Repository request summary
  ↓
Governed approval and provisioning
```

The advisor does not approve or create repositories.

Its purpose is to support:

**Self-service decisioning → governed repository provisioning**

## Files

- [`instructions.md`](./instructions.md) — instructions used to configure the advisor.
- [`test-scenarios.md`](./test-scenarios.md) — scenarios used to validate advisor behavior.

## Knowledge source

The Open Source Hub is the authoritative source for repository governance and open source guidance.

Relevant guidance includes:

- [How Dynatrace Approaches Open Source](../docs/getting-started/how-dynatrace-approaches-open-source.md)
- [Should This Be Open Source?](../docs/getting-started/should-this-be-open-source.md)
- [Where Does My Repository Belong?](../docs/getting-started/where-does-my-repo-belong.md)
- [Repository Lifecycle](../docs/governance/repository-lifecycle.md)
- [Support Models](../docs/governance/support-models.md)
- [New Repository Requirements](../docs/publishing/new-repositories.md)
- [Private-to-Public Transition](../docs/publishing/private-to-public.md)
- [Publishing Checklist](../docs/publishing/publishing-checklist.md)
- [Repository Health](../docs/maintaining/repository-health.md)
- [Security Readiness](../docs/maintaining/security-readiness.md)

## Current implementation

The initial implementation uses a Claude Project with:

1. The relevant Open Source Hub documents added as Project Knowledge.
2. The contents of `instructions.md` added as Project Instructions.
3. `test-scenarios.md` used to validate recommendations before broader rollout.

Future versions may integrate with the repository request and provisioning workflow after the advisory experience has been validated.
