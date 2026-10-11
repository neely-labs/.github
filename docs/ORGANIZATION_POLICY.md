# Neely Labs organization policy

## Identity and ownership

Neely Labs is the open-source and experimental software studio of Neely
Solutions LLC. Neely Solutions LLC owns organization-created project assets and
copyright unless a repository states otherwise. Outside contributions remain
under the repository's inbound-equals-outbound open-source license model.

Neely Labs is operated separately from the LLC's client services practice, but
it is not a separate legal entity or liability boundary.

## Client-work boundary

Client code, client data, contractual work product, credentials, and confidential
information do not enter Neely Labs by default. Movement between the client and
Labs contexts requires an explicit rights, confidentiality, history, license,
Actions, secrets, Pages, and deployment review.

## Repository lifecycle

Repositories are created privately and published intentionally. Before
publication, confirm:

- ownership and contributor rights;
- an explicit license;
- clean history with no credentials or client material;
- README, maturity, maintenance, and support expectations;
- private vulnerability reporting and applicable security features;
- CI and the appropriate protection tier; and
- deployment, domain, secret, and environment ownership.

Abandoned work is archived before deletion. Transfers receive the same review as
publication plus a destination-specific access and deployment review.

## Access and automation

Access is least-privilege and team-scoped. Destructive organization and
repository actions remain owner-only. Durable automation uses GitHub Apps, OIDC,
or scoped workflow tokens instead of shared bot accounts and long-lived classic
personal access tokens.

Third-party Actions require explicit approval and immutable commit-SHA pins.
The stable maintained-repository merge gate is named `PR Verify`; repository-
specific deployment gates are added only after they exist and pass.

Private repositories must not enable paid GitHub Code Security or CodeQL.
Repository templates and bootstrap scripts must not add a CodeQL workflow or
enable paid security products. A future change requires the owner's explicit
approval. Keep free dependency graphs, Dependabot alerts and security updates.
The public baseline retains free CodeQL, secret scanning, and push protection.

## Review cadence

Review organization membership, third-party applications, Blacksmith repository
scope, Actions publishers, personal access tokens, security coverage, and
repository rules monthly. Drift is reported for review and is never silently
repaired.
