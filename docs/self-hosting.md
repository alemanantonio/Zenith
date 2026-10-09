# Self-hosting

## What self-hosting means

Self-hosting means running a product on infrastructure you control — your own servers, a machine at home, or a cloud account you manage — instead of relying exclusively on a service operated by someone else.

Self-hosting typically gives you control over data location, upgrade timing, customization, and long-term cost. It also gives you responsibilities: installation, updates, backups, security patching, and availability. Whether that trade-off is possible depends entirely on each product, because a product must publish its code, its requirements, and its deployment instructions before anyone can run it.

Zenith's products are independent projects. Self-hosting support is therefore decided and documented per product, never for the brand as a whole.

## Current status of Zenith products

As of 2026-10-09, none of the Zenith product repositories contains installation, container, or deployment documentation. This catalog does not claim that any Zenith product can be self-hosted today.

| Product | Self-hosting documentation | Where it will live |
| --- | --- | --- |
| [Zenith-SaaS](https://github.com/alemanantonio/Zenith-SaaS) | Not available | In the product repository, once published |
| [Zenith-Inventario](https://github.com/alemanantonio/Zenith-Inventario) | Not available | In the product repository, once published |
| [Zenith-Dashboard](https://github.com/alemanantonio/Zenith-Dashboard) | Not available | In the product repository, once published |
| Zenith-Web | Not applicable | Repository not publicly accessible |
| [Zenith](https://github.com/alemanantonio/Zenith) (this catalog) | Not applicable | Contains no runnable software |

It is also not yet documented whether any of these products is a hosted service that cannot be deployed by users, or software intended to be installed. That statement itself is part of the documentation each product owes its users.

## Where self-hosting documentation belongs

Self-hosting instructions are maintained in the product's own repository, alongside its code, so they can be updated in the same change that alters deployment behavior. Typical locations, once a product supports self-hosting:

- The product's `README.md`, with a short installation summary.
- A `docs/` directory with a deployment guide.
- Container or deployment definitions (for example a Dockerfile or compose file), only if the product actually ships them.
- Release notes, describing anything that affects existing installations when upgrading.

This catalog links to those documents. It does not reproduce commands, environment variables, or infrastructure requirements, because those details change with each release and belong to the product.

## Information each product must publish before self-hosting is advertised

A product is ready to be listed as self-hostable in this catalog when its repository documents:

- Supported operating systems and architectures.
- Required runtimes and versions, and required external services such as databases or object storage.
- Configuration: environment variables, configuration files, secrets, and their defaults.
- Build and installation steps, from a clean machine to a running instance.
- Data persistence: what must be backed up and where it is stored.
- The upgrade path between versions, including migrations.
- Reverse proxy and TLS expectations, if the product serves HTTP.
- Rough resource requirements.
- Known limitations and security considerations for exposed deployments.
- The license terms that apply to self-hosting the product.

Until a product documents these points, the honest status is "not documented", and this catalog will report it that way.

## If you want to self-host a Zenith product today

- Check the product repository first: if documentation exists, it is there, not here.
- If nothing is published, you can open an issue in the product's repository asking for deployment documentation, following [../CONTRIBUTING.md](../CONTRIBUTING.md).
- Do not infer deployment steps from partial files, and do not assume that an empty repository can be installed.

## For maintainers

When a product gains self-hosting support, publish the documentation in the product repository, then update this file and the product's entry in [projects.md](projects.md), changing its status from "not documented" to the verified capability, with a link to the instructions. Keep this catalog factual: only claim what the product repository can demonstrate.
