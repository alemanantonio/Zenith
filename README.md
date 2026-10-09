# Zenith

Español: [es/README.md](es/README.md)

Zenith is a software brand that offers development services and maintains a set of products developed in the open. This repository is the central catalog for Zenith's open source projects: it explains what Zenith is, lists the available products, and links to the repository, documentation, and support channels of each one.

Every product is developed independently in its own repository, where its code, architecture, dependencies, versions, releases, issues, and roadmap live. This catalog is an entry point to those projects. It does not duplicate or replace the documentation maintained inside each product.

## Open source approach

Zenith publishes its products as public repositories so that anyone can inspect the code, report problems, propose changes, and, where a product supports it, run the software on their own infrastructure.

In practice, this means:

- Each product repository is the source of truth for its code, documentation, issues, and releases.
- Status reported in this catalog is limited to what can be verified in those repositories. Features that have not been published are not described as available.
- Licenses, release notes, and installation instructions are defined per repository, not for the brand as a whole.

## Products

Repository status verified on 2026-10-09 against the public repositories of [github.com/alemanantonio](https://github.com/alemanantonio).

| Product | Description | Verified status | Repository |
| --- | --- | --- | --- |
| **Zenith** | Central catalog and entry point for the Zenith open source projects. | Catalog documentation only; no product code. | [alemanantonio/Zenith](https://github.com/alemanantonio/Zenith) |
| **Zenith-SaaS** | Software as a service product. | Repository created. | [alemanantonio/Zenith-SaaS](https://github.com/alemanantonio/Zenith-SaaS) |
| **Zenith-Inventario** | Inventory management system. | Repository created. | [alemanantonio/Zenith-Inventario](https://github.com/alemanantonio/Zenith-Inventario) |
| **Zenith-Dashboard** | Dashboard and integrated tools. | Repository created. | [alemanantonio/Zenith-Dashboard](https://github.com/alemanantonio/Zenith-Dashboard) |
| **Zenith-Web** | Public website of the Zenith brand. | Repository created. | [alemanantonio/Zenith-Web](https://github.com/alemanantonio/Zenith-Web) |

Descriptions come from the project owner and have not yet been corroborated by published code. Per-product detail is maintained in [docs/projects.md](docs/projects.md).

### Installation instructions

Installation and usage instructions are linked here only when they exist in the corresponding product repository. None are published at the moment. See [docs/self-hosting.md](docs/self-hosting.md) for the status of self-hosting documentation.

## Documentation

| Document | Contents |
| --- | --- |
| [docs/projects.md](docs/projects.md) | Detailed catalog: purpose, verified functionality, technologies, status, and links per product. |
| [docs/development-principles.md](docs/development-principles.md) | Principles that govern how Zenith's repositories are organized and developed. |
| [docs/self-hosting.md](docs/self-hosting.md) | Introduction to self-hosting and the documentation each product must provide. |
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to report issues, propose changes, and contribute across the Zenith repositories. |
| [SECURITY.md](SECURITY.md) | How to report vulnerabilities responsibly. |
| [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) | Expected behavior in Zenith project spaces. |

## Contributing

Contributions are made to the product repository they affect, not to this catalog. Before opening an issue or a pull request, identify the repository that owns the code or documentation you want to change; the general workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md), and development-specific instructions are kept inside each product repository.

## Principles

- **Product independence.** Each repository is an independent project with its own codebase, decisions, and identity. There is no shared monorepo and no required code sharing between products.
- **Maintainability.** Changes stay within the scope of a single product and follow the conventions already established there.
- **Transparency.** Development happens in public: issues, decisions, and releases are recorded in the repository where the product is developed.
- **Self-hosting when supported.** A product documents self-hosting instructions only when it genuinely supports running on infrastructure you control.

These principles are described in full in [docs/development-principles.md](docs/development-principles.md).

## Status of this catalog

Repository availability, links, and status in this document were checked against the GitHub API on 2026-10-09. Update that date whenever the catalog is revised, and remove entries that no longer reflect the state of the repositories.
