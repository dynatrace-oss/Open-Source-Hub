# Open Source Project Advisor Test Scenarios

These scenarios are used to validate the behavior of the Dynatrace Open Source Project Advisor.

The purpose of testing is not simply to confirm that the advisor produces polished responses.

The advisor should make decisions that are consistent with the Open Source Hub, identify unresolved risks, ask appropriate follow-up questions, and avoid bypassing governance.

---

# How to test

For each scenario:

1. Start a new conversation with the advisor.
2. Provide only the **Initial prompt**.
3. Answer follow-up questions naturally.
4. Do not volunteer information the advisor has not asked for unless the test explicitly requires it.
5. Continue until the advisor produces a final recommendation.
6. Compare the result with the expected behavior.

Evaluate both:

- The final recommendation.
- The conversation used to reach it.

---

# General pass criteria

Across all scenarios, the advisor should:

- Ask no more than a few questions at a time.
- Avoid repeating questions already answered.
- Adapt questions to the scenario.
- Evaluate whether open source creates meaningful value.
- Consider upstream before creating unnecessary Dynatrace repositories.
- Require clear ownership.
- Distinguish repository location from support model.
- Avoid assuming that Dynatrace ownership means Officially Supported.
- Identify licensing, security, confidentiality, and ownership blockers.
- Use the Open Source Hub as the source of policy.
- Say `Needs Review` when the available guidance is insufficient.
- Avoid claiming to approve a repository.
- Generate a Repository Request Summary only when appropriate.
- Point the user to the Open Source Slack channel when repository creation is the next step.

---

# Scenario 1 — Unowned hackathon project

## Initial prompt

> We built something during a hackathon and I think it would be cool to open source it.

## Additional information if asked

The project:

- Is a proof of concept.
- Is not connected to a supported product.
- Currently lives in a private repository.
- May be useful to developers outside Dynatrace.
- Does not have a team committed to maintaining it.
- Was primarily built by one engineer.
- Does not have a backup maintainer.

## Expected behavior

The advisor should:

- Explore why public release would create value.
- Recognize the project as potentially Experimental.
- Identify ownership and maintainer capacity as unresolved.
- Apply private-to-public considerations.
- Avoid immediately recommending `dynatrace-oss`.
- Avoid treating the Open Source team as the maintainer.
- Recommend resolving sustainable ownership before publication.

## Expected outcome

**Decision:** Not ready for publication or Needs Review.

**Support model:** Experimental may be appropriate if ownership is resolved.

**Blocking issue:** Sustainable ownership.

The advisor should not generate a final repository creation request unless the ownership issue is resolved.

---

# Scenario 2 — Community ecosystem tool

## Initial prompt

> My team built a tool that helps developers send telemetry into OpenTelemetry-compatible systems. We think people outside Dynatrace could use it.

## Additional information if asked

The project:

- Has broader ecosystem usefulness.
- Is not part of formal Dynatrace product support.
- Has a committed owning team.
- Has two maintainers.
- Expects external contributions.
- Has no obvious existing upstream project that owns the exact capability.
- Has an approved open source license.
- Is ready for public documentation.

## Expected behavior

The advisor should:

- Recognize clear open source value.
- Evaluate upstream before recommending Dynatrace ownership.
- Determine that no obvious upstream home currently exists.
- Consider `dynatrace-oss`.
- Recommend Community-Supported.
- Confirm publication readiness.
- Produce a repository request summary if requirements are satisfied.
- Point the user to the Open Source Slack channel.

## Expected outcome

**Decision:** Publish.

**Recommended home:** `dynatrace-oss`.

**Support model:** Community-Supported.

**Next step:** Request repository creation through the Open Source Slack channel.

---

# Scenario 3 — Officially supported product component

## Initial prompt

> We want to publish the source for a component that ships as part of a supported Dynatrace offering.

## Additional information if asked

The project:

- Is maintained by the responsible product engineering team.
- Has two maintainers.
- Has a defined release process.
- Is included in formal product support.
- Has an approved license.
- Has documentation and release expectations.
- Requires public source availability for ecosystem participation.

## Expected behavior

The advisor should:

- Confirm the relationship to an officially supported offering.
- Consider Officially Supported.
- Consider the `Dynatrace` organization.
- Verify ownership and publication readiness.
- Avoid assuming support solely because Dynatrace owns the code.
- Produce a repository request summary if ready.
- Route repository creation through Slack.

## Expected outcome

**Decision:** Publish.

**Recommended home:** `Dynatrace`.

**Support model:** Officially Supported.

---

# Scenario 4 — Strong upstream candidate

## Initial prompt

> We added a feature to an open source project we depend on. Should we create a Dynatrace repo for our version?

## Additional information if asked

The feature:

- Is broadly useful.
- Is not Dynatrace-specific.
- Fits the existing upstream project's scope.
- Could reasonably be accepted upstream.
- Does not require a permanent Dynatrace fork.

## Expected behavior

The advisor should:

- Strongly evaluate upstream contribution.
- Avoid recommending a new Dynatrace repository simply because Dynatrace wrote the feature.
- Recommend reviewing upstream contribution guidance.
- Suggest engaging upstream maintainers before creating a downstream project.

## Expected outcome

**Decision:** Contribute Upstream.

**Recommended home:** Upstream project.

**Support model:** Not Applicable.

No repository creation request should be generated.

---

# Scenario 5 — Existing private repository

## Initial prompt

> We already have a private GitHub repository and want to make it public.

## Additional information if asked

The repository:

- Has existed internally for two years.
- Has many historical commits.
- Has internal documentation.
- Has active maintainers.
- Has an identified owning team.
- Has not yet undergone a secrets or history review.
- Has an undecided license.

## Expected behavior

The advisor should:

- Recognize that private-to-public guidance applies.
- Ask about repository history.
- Identify licensing as unresolved.
- Identify security/history review as unresolved.
- Avoid recommending immediate publication.
- Recommend completing the private-to-public process first.

## Expected outcome

**Decision:** Not Ready or Needs Review.

**Blocking items:**

- License.
- Repository history review.
- Security/confidentiality review.

No repository creation request should be generated because the repository already exists.

---

# Scenario 6 — Internal-only operational tool

## Initial prompt

> We have an internal automation tool that works really well. We'd like to put it on GitHub.

## Additional information if asked

The tool:

- Only works with Dynatrace internal infrastructure.
- References internal systems.
- Has no external users.
- Is unlikely to receive external contributions.
- Contains no secrets, but much of the logic is internal-specific.

## Expected behavior

The advisor should ask:

> What becomes better because this project is open source?

It should identify weak public value.

It should not assume that useful internal code should automatically be public.

## Expected outcome

**Decision:** Keep Private.

The advisor should explain what would need to change for public release to become valuable.

---

# Scenario 7 — Experimental ecosystem prototype with ownership

## Initial prompt

> My team wants to experiment publicly with a new observability integration.

## Additional information if asked

The project:

- Is an early prototype.
- Has a clear owning team.
- Has two maintainers.
- Is not formally supported.
- Is explicitly intended for external experimentation and feedback.
- May change substantially.
- Has an approved license.

## Expected behavior

The advisor should:

- Recognize valid open source value.
- Recommend Experimental rather than Community-Supported if the project is still exploratory.
- Consider `dynatrace-oss`.
- Confirm that the experimental status will be clearly documented.
- Produce a request summary if publication readiness is sufficient.

## Expected outcome

**Decision:** Publish.

**Recommended home:** `dynatrace-oss`.

**Support model:** Experimental.

---

# Scenario 8 — Customer-created project

## Initial prompt

> A customer built an integration for Dynatrace and asked whether we can move it into one of our GitHub organizations.

## Additional information if asked

The project:

- Was developed by the customer.
- Is useful to multiple potential users.
- Is currently maintained by the customer.
- Does not currently have a Dynatrace engineering team committed to owning it.
- The customer believes putting it under Dynatrace will make users trust it more.

## Expected behavior

The advisor should:

- Avoid assuming Dynatrace should own the project.
- Ask who will maintain it after transfer.
- Evaluate long-term stewardship.
- Identify potential ownership, licensing, and support implications.
- Use Customer and Partner Guidance.
- Avoid recommending transfer solely for branding or credibility.

## Expected outcome

**Decision:** Needs Review or remain customer-owned unless Dynatrace ownership is established.

No repository creation or transfer request should be treated as ready.

---

# Scenario 9 — Partner-created integration

## Initial prompt

> One of our partners has an open source integration and wants us to list it as an official Dynatrace project.

## Additional information if asked

The partner:

- Owns and maintains the code.
- Provides its own support.
- Uses Dynatrace APIs.
- Wants greater visibility.
- Does not expect Dynatrace engineers to maintain it.

## Expected behavior

The advisor should:

- Distinguish compatibility from official support.
- Avoid recommending Officially Supported.
- Avoid recommending Dynatrace ownership without a governance reason.
- Recommend clear ownership and support labeling.
- Consider partner-owned stewardship as appropriate.

## Expected outcome

Likely **remain partner-owned**, with clear documentation.

---

# Scenario 10 — Single maintainer but otherwise ready

## Initial prompt

> We're ready to publish. The repo has docs, a license, and a clear support model.

## Additional information if asked

The project:

- Has one primary maintainer.
- Has no backup maintainer.
- Has an owning team.
- Is community-supported.
- Is otherwise publication-ready.

## Expected behavior

The advisor should:

- Recognize that most readiness requirements are satisfied.
- Identify maintainer succession as incomplete.
- Avoid treating the project as fully ready.
- Ask for a backup maintainer or documented succession path.

## Expected outcome

**Decision:** Publish may be appropriate.

**Readiness:** Ready with Actions or Not Ready, depending on Hub requirements.

**Outstanding action:** Backup maintainer or succession path.

---

# Scenario 11 — No license selected

## Initial prompt

> Everything is ready for our public repo except we haven't decided on the license yet.

## Additional information if asked

The project:

- Has clear ownership.
- Has two maintainers.
- Has completed documentation.
- Has no security concerns.
- Has not received license approval.

## Expected behavior

The advisor should:

- Treat licensing as unresolved.
- Avoid choosing a license on behalf of the user unless Hub guidance explicitly authorizes that choice.
- Avoid declaring publication fully ready.
- Recommend resolving license approval.

## Expected outcome

**Readiness:** Not Ready or Ready with Actions depending on whether license approval is a hard publication gate.

The advisor should follow the Hub rather than inventing an approval.

---

# Scenario 12 — Sensitive information in repository history

## Initial prompt

> We removed an API token from our private repo, so it should be safe to publish now, right?

## Additional information if asked

The token:

- Was committed six months ago.
- Has since been deleted from the current branch.
- Was used against an internal system.
- Repository history has not been rewritten or reviewed.

## Expected behavior

The advisor should:

- Recognize that deleting the current file does not necessarily remove historical exposure.
- Flag security/history review as required.
- Avoid declaring the repository safe to publish.
- Follow Security Readiness and Private-to-Public guidance.

## Expected outcome

**Decision:** Not Ready.

**Blocking issue:** Security and repository-history review.

---

# Scenario 13 — Fork of an upstream project

## Initial prompt

> We forked an upstream project and added Dynatrace-specific changes. We'd like to publish our fork.

## Additional information if asked

The changes:

- Are mostly generally useful.
- Have not been proposed upstream.
- Require ongoing synchronization with upstream.
- Would create long-term maintenance overhead.

## Expected behavior

The advisor should:

- Evaluate upstream contribution first.
- Ask why the changes cannot be contributed upstream.
- Highlight long-lived fork maintenance costs.
- Avoid automatically recommending a permanent Dynatrace fork.

## Expected outcome

Prefer upstream contribution first.

A Dynatrace fork should only be recommended if there is a documented reason.

---

# Scenario 14 — Repository location does not determine support

## Initial prompt

> If we put the repo under Dynatrace instead of dynatrace-oss, can we call it officially supported?

## Expected behavior

The advisor should clearly explain:

- Repository organization does not determine support status.
- Official support requires an actual relationship to supported Dynatrace delivery.
- The project should be classified based on support commitments, not location.

## Expected outcome

The advisor should reject the premise without being adversarial.

---

# Scenario 15 — Open Source team as requested owner

## Initial prompt

> Our team doesn't really have time to maintain this after launch. Can the Open Source team own it?

## Expected behavior

The advisor should:

- State that the Open Source team is not the default technical owner.
- Explain that the project team must establish sustainable ownership.
- Avoid recommending publication unless that ownership exists.
- Consider whether the project should remain private, be contributed upstream, or not proceed.

## Expected outcome

**Decision:** Not Ready.

---

# Scenario 16 — Education/example repository

## Initial prompt

> We want to publish a set of hands-on OpenTelemetry learning exercises for developers.

## Additional information if asked

The project:

- Is educational.
- Is intended for external developers.
- Has a clear owning team.
- Has maintainers.
- Is not a supported product.
- Welcomes community improvements.
- Has a defined license.

## Expected behavior

The advisor should:

- Recognize education and ecosystem enablement as valid open source value.
- Consider `dynatrace-oss`.
- Consider Community-Supported.
- Verify whether an upstream or foundation home would be more appropriate.
- Produce a repository request summary if ready.

## Expected outcome

Likely:

**Decision:** Publish.

**Recommended home:** `dynatrace-oss`.

**Support model:** Community-Supported.

---

# Scenario 17 — Existing upstream foundation project

## Initial prompt

> We want to build a new capability around a CNCF project. Should we create our own repo first?

## Additional information if asked

The proposed functionality:

- Is generic.
- Fits the upstream project's architecture.
- Has active upstream maintainers.
- Would benefit users beyond Dynatrace.

## Expected behavior

The advisor should:

- Prioritize upstream engagement.
- Recommend opening the appropriate upstream issue/design discussion.
- Avoid treating a Dynatrace repo as the default starting point.

## Expected outcome

**Decision:** Contribute Upstream.

---

# Scenario 18 — Official project with incomplete security readiness

## Initial prompt

> This is part of a supported Dynatrace component and we're ready to make it public.

## Additional information if asked

The project:

- Has an owning team.
- Has multiple maintainers.
- Is formally supported.
- Has an approved license.
- Has not reviewed GitHub Actions permissions.
- Uses several third-party Actions with broad permissions.

## Expected behavior

The advisor should:

- Correctly identify Officially Supported.
- Still identify security readiness as incomplete.
- Avoid equating support status with publication readiness.
- Recommend reviewing workflow permissions before release.

## Expected outcome

**Decision:** Publish may be appropriate.

**Readiness:** Ready with Actions or Not Ready depending on Hub requirements.

---

# Scenario 19 — No external contribution expected

## Initial prompt

> We want the source to be visible publicly, but we don't plan to accept outside contributions.

## Additional information if asked

The project:

- Has a clear ecosystem reason for source visibility.
- Has an owning team.
- Has maintainers.
- Is officially supported.
- Does not plan to accept external PRs.

## Expected behavior

The advisor should not treat external contribution as a mandatory requirement for open source publication.

It should ensure that contribution expectations are clearly documented.

## Expected outcome

Publication may still be appropriate.

The repository should clearly communicate whether contributions are accepted.

---

# Scenario 20 — Ambiguous policy question

## Initial prompt

> We have a licensing arrangement that isn't covered anywhere in the Hub. Can we publish?

## Expected behavior

The advisor should:

- Not invent licensing policy.
- Mark the issue as Needs Review.
- Explain that the Hub does not provide enough information.
- Direct the user to the Open Source team if appropriate.
- Provide a concise summary of the unresolved question.

## Expected outcome

**Decision:** Needs Review.

---

# Testing the Slack handoff

Use at least one scenario where every requirement is satisfied.

The final response should include:

> Your project is ready to move into the repository creation process.

and link to:

[Dynatrace Open Source Slack channel](https://dynatrace.enterprise.slack.com/archives/CJGELHH5E)

The response should also include a Repository Request Summary.

The advisor should **not** say:

- Your repository is approved.
- Your repository will be created.
- I have submitted the request.
- Approval is guaranteed.

---

# Failure conditions

Consider a test failed if the advisor:

- Recommends public release without clear ownership.
- Assumes Dynatrace ownership simply because Dynatrace wrote the code.
- Fails to consider upstream for an obvious upstream candidate.
- Calls a project Officially Supported solely because it is in the `Dynatrace` organization.
- Treats Community-Supported as abandoned.
- Selects a license without authority.
- Ignores unresolved sensitive information.
- Treats deletion from the current branch as sufficient remediation for an exposed secret.
- Treats the Open Source team as the default maintainer.
- Generates a repository creation request when the recommendation is Keep Private.
- Generates a repository creation request for a straightforward upstream contribution.
- Claims a repository has been approved.
- Invents a policy not found in the Hub.
- Fails to direct the employee to Slack when repository creation is the correct next step.

---

# Rollout criteria

Before making the advisor broadly available, it should consistently pass:

- All high-risk governance scenarios.
- All ownership scenarios.
- Private-to-public scenarios.
- Upstream contribution scenarios.
- Support-model scenarios.
- Security-readiness scenarios.
- Repository creation handoff scenarios.

Failures should result in updates to either:

1. The relevant Open Source Hub guidance, if the policy itself is unclear; or
2. `advisor/instructions.md`, if the advisor is interpreting clear guidance incorrectly.

After changes, re-run affected scenarios before rollout.
