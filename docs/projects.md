# Zenith product catalog

This document catalogs each Zenith project in detail: its purpose, the problem it addresses, its verified functionality and technologies, its development status, and where to find its code, issues, releases, and documentation.

All data below was verified on 2026-10-09 against the public repositories of [github.com/alemanantonio](https://github.com/alemanantonio) using the GitHub API. Facts marked as pending have not been confirmed anywhere in a public repository and must not be treated as available.

## Summary of verified repository state

| Repository | Created | Commits and files | Releases | Documentation | License |
| --- | --- | --- | --- | --- | --- |
| [Zenith](https://github.com/alemanantonio/Zenith) | 2026-09-29 | Catalog documentation in this repository | None | This catalog | Not published |
| [Zenith-SaaS](https://github.com/alemanantonio/Zenith-SaaS) | 2026-10-09 | None | None | None | Not published |
| [Zenith-Inventario](https://github.com/alemanantonio/Zenith-Inventario) | 2026-10-09 | None | None | None | Not published |
| [Zenith-Dashboard](https://github.com/alemanantonio/Zenith-Dashboard) | 2026-10-09 | None | None | None | Not published |
| Zenith-Web | Not applicable | Repository not publicly accessible (HTTP 404 at verification) | Unknown | Unknown | Unknown |

"No license published" means the repository does not currently contain a license file, so no permission to use, modify, or redistribute its code is granted explicitly. Each product must publish its own license before it can be described as open source.

## Zenith (this repository)

**Purpose:** Central catalog and entry point for the Zenith open source projects. It presents the brand, the products, and the general contribution, security, and conduct policies.

**Problem it addresses:** Visitors and contributors have no single place to discover which projects belong to Zenith, what state they are in, and where to go next.

**Verified functionality:** The repository contains catalog documentation only (this file, the root documents, and the `docs/` directory). It contains no application code.

**Verified technologies:** Markdown and GitHub's repository features. Nothing else applies.

**Development status:** The repository existed with no published commits at verification time; the catalog documents are its first content.

**Links:** [Repository](https://github.com/alemanantonio/Zenith) | [Issues](https://github.com/alemanantonio/Zenith/issues) | [Releases](https://github.com/alemanantonio/Zenith/releases) (none published) | [Contributing](../CONTRIBUTING.md) | [Security](../SECURITY.md) | [Code of conduct](../CODE_OF_CONDUCT.md)

**Installation and self-hosting:** Not applicable. This repository has nothing to install.

This repository does not track the roadmaps of the products; those are maintained in each product's own repository.

## Zenith-SaaS

**Purpose:** Software as a service product of the brand. (Description provided by the project owner; not yet corroborated by published code.)

**Problem it addresses:** Pending. No public document states which user problem the product solves or who its users are.

**Verified functionality:** None published. No code, README, or documentation exists in the repository to confirm any feature.

**Verified technologies:** None. No source code or dependency manifest is available to inspect.

**Development status:** The repository was created on 2026-10-09 and was empty at verification time: no commits, no files, no releases.

**Links:** [Repository](https://github.com/alemanantonio/Zenith-SaaS) | [Issues](https://github.com/alemanantonio/Zenith-SaaS/issues) (enabled) | [Releases](https://github.com/alemanantonio/Zenith-SaaS/releases) (none published) | Documentation: not available | License: not published

**Installation and self-hosting:** Not documented. Whether the product is a hosted service, deployable software, or both is not stated anywhere yet. The information required before self-hosting can be recommended is listed in [self-hosting.md](self-hosting.md).

This product maintains its own development cycle. Roadmap, versions, releases, and issues are managed in its repository and are not coordinated with the other Zenith products.

## Zenith-Inventario

**Purpose:** Inventory management system. (Description provided by the project owner; not yet corroborated by published code.)

**Problem it addresses:** Pending. No public document specifies the inventory workflows, the scale, or the users it targets.

**Verified functionality:** None published. The repository contains no code or documentation to confirm any feature.

**Verified technologies:** None. No source code or dependency manifest is available to inspect.

**Development status:** The repository was created on 2026-10-09 and was empty at verification time: no commits, no files, no releases.

**Links:** [Repository](https://github.com/alemanantonio/Zenith-Inventario) | [Issues](https://github.com/alemanantonio/Zenith-Inventario/issues) (enabled) | [Releases](https://github.com/alemanantonio/Zenith-Inventario/releases) (none published) | Documentation: not available | License: not published

**Installation and self-hosting:** Not documented. Inventory systems usually depend on a database and on deployment decisions that are not yet described. See the pending list in [self-hosting.md](self-hosting.md).

This product maintains its own development cycle. Roadmap, versions, releases, and issues are managed in its repository and are not coordinated with the other Zenith products.

## Zenith-Dashboard

**Purpose:** Dashboard and integrated tools. (Description provided by the project owner; not yet corroborated by published code.)

**Problem it addresses:** Pending. It is not documented which data the dashboard displays or which tools it integrates.

**Verified functionality:** None published. The repository contains no code or documentation to confirm any feature.

**Verified technologies:** None. No source code or dependency manifest is available to inspect.

**Development status:** The repository was created on 2026-10-09 and was empty at verification time: no commits, no files, no releases.

**Links:** [Repository](https://github.com/alemanantonio/Zenith-Dashboard) | [Issues](https://github.com/alemanantonio/Zenith-Dashboard/issues) (enabled) | [Releases](https://github.com/alemanantonio/Zenith-Dashboard/releases) (none published) | Documentation: not available | License: not published

**Installation and self-hosting:** Not documented. The relationship between this product and the other Zenith products, if any, is not described yet. See the pending list in [self-hosting.md](self-hosting.md).

This product maintains its own development cycle. Roadmap, versions, releases, and issues are managed in its repository and are not coordinated with the other Zenith products.

## Zenith-Web

**Purpose:** Public website of the Zenith brand. (Description provided by the project owner.)

**Problem it addresses:** Pending. No public repository is available to confirm.

**Verified functionality:** None. A request to `https://github.com/alemanantonio/Zenith-Web` returned HTTP 404 on 2026-10-09, so the repository is either private or does not exist under that name.

**Verified technologies:** None.

**Development status:** Unknown. The repository does not appear in the list of public repositories of the account.

**Links:** Repository link cannot be verified. Do not publish a link to it until the repository is public and confirmed.

**Installation and self-hosting:** Not applicable until the repository is accessible. A brand website is also typically deployed rather than self-hosted by users; state clearly what applies once the repository exists.

## Information pending per product

For each product repository (except this catalog), the following must be added in the product's own repository before this catalog can describe it as usable:

- A `README.md` stating what the product does, for whom, and its current maturity.
- A license file.
- Verified functionality and technology data, so this catalog can replace the "pending" entries above.
- Installation or deployment instructions, or an explicit statement that the product is a hosted service and cannot be self-hosted.
- At least one release or an explicit statement of how the product is consumed before its first release.

When a product adds this information, update its section here and the summary table at the top of this file. Keep the central catalog short: link to the product's documentation instead of copying it.
