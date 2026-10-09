# Development principles

This document defines how Zenith's open source projects are organized and developed. It applies to this catalog and is intended to be respected by every Zenith product repository. Rules specific to a product always live in that product's repository and take precedence over anything written here.

## Each product is an independent project

Every product is a standalone repository with its own identity, scope, and codebase. Products do not share a monorepo, and code sharing is never a requirement for contributing to or using a product. A change in one product must not force changes in another.

Independence also means independence of decisions: a product may choose the stack, license, and structure that fit its problem, even when another Zenith product chose differently.

## Each repository manages its own development cycle

The product repository owns:

- Its roadmap and the priorities of its maintainers.
- Its versioning scheme and its releases.
- Its dependencies and upgrade cadence.
- Its issue tracker and its definition of done.

There is no shared release calendar, no coordinated versioning between products, and no requirement that products adopt a common dependency version. A delay or a major change in one product says nothing about the others.

## Architectural decisions belong to the product repository

Discussion about the design, stack, or direction of a product happens in that product's issues and pull requests, with the people who maintain and use it. This catalog does not decide, endorse, or override technical choices for any product.

Decisions that affect users, such as breaking changes or dropped support, are documented in the product's own release notes and README.

## Contributions follow the product's technology and conventions

A contribution to a product must work within the technologies, structure, naming, and conventions already established in that repository. Contributors should not introduce patterns borrowed from another Zenith product without discussion in the repository where the change lands. The general workflow in [../CONTRIBUTING.md](../CONTRIBUTING.md) describes how to participate; the product defines how to build, test, and format its code.

## Documentation lives next to the product it describes

Product documentation — README, guides, API reference, deployment instructions — is maintained inside the product repository, where it changes together with the code.

This central catalog holds only catalog-level material: what Zenith is, which products exist, their verified status, and the general policies for contributing, security, and conduct. It links to product documentation instead of copying it, and it reports only data that can be verified in the repositories.

## Self-hosting is documented only when it is real

A product may state that it can be self-hosted only when its repository actually contains the instructions and requirements to do so. Until then, the catalog describes self-hosting for that product as undocumented, not as supported. See [self-hosting.md](self-hosting.md).

## Out of scope for Zenith as a whole

To avoid ambiguity, the following are explicitly not part of these principles:

- A mandatory monorepo or shared codebase across products.
- A single build process, framework, language, or test suite for all projects.
- A shared release schedule or coordinated versioning between products.
- Mandatory dependencies between products, in either direction.
- Central approval of a product's technical roadmap by this catalog repository.
