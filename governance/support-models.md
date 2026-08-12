# Support Models

Every public Dynatrace repository must clearly communicate what level of support users should expect.

A repository's GitHub organization does not, by itself, define its support model.

## Officially supported

An officially supported repository is associated with a Dynatrace capability for which an established support commitment exists.

Typical examples may include:

- Product SDKs.
- Supported deployment components.
- Official integrations.
- Product distributions.

### Requirements

Officially supported repositories should have:

- Named engineering or product ownership.
- Named maintainers.
- Defined supported versions where applicable.
- A documented release process.
- A security disclosure process.
- Clear documentation.
- An established support channel.

GitHub Issues should not be presented as a substitute for Dynatrace Support unless explicitly intended.

### Recommended README language

> This project is maintained by Dynatrace. For product support, use the applicable Dynatrace support channel. GitHub Issues may be used for repository-specific bugs, feature requests, or contribution discussions as described below.

---

## Community-supported

Community-supported repositories are publicly maintained but are not covered by standard Dynatrace product support.

They may be maintained by:

- Dynatrace employees.
- Community maintainers.
- Customer Success teams.
- Developer advocates.
- Partners.
- Mixed internal/external communities.

### Requirements

Community-supported repositories should have:

- Named maintainers.
- Clear contribution pathways.
- Clear support disclaimers.
- SECURITY.md.
- Appropriate license.
- A clear scope.

Community-supported does not mean abandoned.

### Recommended README language

> This project is community-supported and is not covered by standard Dynatrace product support. Issues and contributions are welcome through this repository. Support and response times are provided on a best-effort basis.

---

## Experimental

Experimental repositories contain:

- Proofs of concept.
- Research.
- Prototypes.
- Demonstrations.
- Event projects.
- Incubating projects.
- Early technical exploration.

### Requirements

Experimental repositories should document:

- Purpose.
- Owner.
- Intended audience.
- Limitations.
- Production-readiness expectations.
- Review or expiration date.

### Recommended README language

> This repository contains experimental work and is provided for evaluation, learning, or demonstration purposes. It is not intended for production use and may change or be discontinued without notice.

---

## Maintenance-only

A maintenance-only repository continues to serve users but is no longer receiving significant feature development.

Maintenance may include:

- Security fixes.
- Critical bug fixes.
- Dependency updates.
- Compatibility updates.
- Packaging or release maintenance.

### Recommended README language

> This project is currently in maintenance mode. Critical fixes and compatibility updates may be provided, but active feature development should not be expected.

---

## Deprecated

A deprecated repository should no longer be selected for new implementations.

A replacement should be identified when possible.

### Recommended README language

> This project has been deprecated and is no longer recommended for new implementations. Please use [replacement project] instead.

---

## Archived

Archived repositories are retained for historical or reference purposes but are no longer maintained.

### Recommended README language

> This project is no longer actively maintained. The repository remains available for reference, but no additional features, fixes, or support should be expected.
