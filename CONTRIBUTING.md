# Contributing to Zenith

Zenith is a set of independent open source projects. This document explains how to participate in them. It describes a general workflow only: each product defines its own build process, stack, tooling, and test requirements inside its own repository, and those definitions take precedence over anything written here.

## Identify the right repository

Every product lives in its own repository. Contributions belong to the repository that owns the affected code or documentation:

| If you want to... | Start here |
| --- | --- |
| Report a problem or propose a feature for a product | The product's repository (see the [catalog](docs/projects.md)) |
| Improve the catalog, contribution, security, or conduct documents | [alemanantonio/Zenith](https://github.com/alemanantonio/Zenith) |
| Report a problem in more than one product | Separate issues, one per repository |

If you are unsure where something belongs, open an issue in the repository that seems closest and say so. Maintainers can move the discussion or tell you where it fits. Do not open the same issue in several repositories.

## Before you start

1. Read the README of the target repository. It should describe the product, its current state, and any development setup.
2. Search the existing issues and pull requests of that repository to avoid duplicating work.
3. Check whether the repository has its own `CONTRIBUTING.md`, coding standards, or development guide. If it does, follow it instead of this document.
4. For large changes, open an issue first to confirm the scope before investing time in an implementation.

## Reporting bugs

Open an issue in the product's repository and include:

- The repository and, if applicable, the version, tag, or commit where the problem occurs.
- Steps to reproduce the problem, as concretely as possible.
- What you expected and what actually happened.
- Your environment: operating system, runtime and version, browser, or other relevant details.
- Logs, screenshots, or error messages that help reproduce the problem. Remove credentials, tokens, and personal data first (see [SECURITY.md](SECURITY.md)).

A good bug report can be reproduced by someone else without asking follow-up questions.

## Proposing improvements

Use issues to propose:

- A defect you have confirmed.
- A specific, scoped improvement to existing behavior.
- Documentation gaps you have found.

Describe the problem the change solves and who it affects. Ideas that are not tied to a concrete problem are harder to evaluate. Roadmaps, versions, and priorities are decided in each product's repository, so expect the discussion to happen there.

## Issue guidelines

- One problem or one proposal per issue.
- Use a clear, specific title: what is wrong or what should change, not "bug" or "help".
- Provide the context requested above; issues that cannot be understood or reproduced are hard to act on.
- Keep the discussion in the issue, on topic and factual.
- Do not post security vulnerabilities in public issues. Follow [SECURITY.md](SECURITY.md).

## Pull request guidelines

- Fork the target repository and branch from its default branch.
- Keep each pull request limited to a single change or a small set of related changes. Unrelated fixes belong in a separate pull request.
- Explain what the change does and why, and link the issue it addresses.
- Follow the code style, structure, and conventions already present in that repository. Do not reformat, rename, or refactor code outside the scope of the change.
- Add or update documentation and tests when the repository's own guidelines require them.
- Expect review. Respond to feedback or explain why you disagree.

## Quality requirements

Every change should be:

- **Understandable.** The title, description, and code make the intent clear without prior context.
- **Scoped.** It touches only what it needs to. Refactors, dependency upgrades, and new features are separate contributions.
- **Consistent.** It matches the conventions of the repository it targets.
- **Complete.** It does not leave broken builds, dead references, or documentation that contradicts the change.

## Respecting each product's decisions

Products differ on purpose. Stack choices, architecture, naming, and trade-offs made in a product repository are deliberate decisions of that project. Contribute within them rather than importing the conventions of another Zenith product or of your own projects. If you disagree with a direction, raise it in an issue and argue the case; do not use a pull request to force a different approach.

## Finding product-specific instructions

Development setup is documented per product, next to the product:

- Start with the product's `README.md`.
- Look for a `CONTRIBUTING.md`, `docs/` directory, or development guide in that repository.
- Check the repository's issues and project board for active work.

This catalog does not publish build commands, dependency lists, or test instructions on behalf of the products, because those details belong to each repository and change with it.

## What this document does not define

To be explicit: there is no single build process, framework, language, linter, or test suite shared by all Zenith projects. This document intentionally does not specify one. Consult the repository you are contributing to.
