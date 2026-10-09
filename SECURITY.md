# Security policy

This document explains how to report security vulnerabilities in Zenith projects and what to expect once a report is received. It applies to the repositories listed in the [product catalog](docs/projects.md).

## Reporting a vulnerability

Security vulnerabilities must not be reported in public issues, discussions, pull requests, or social media.

Report them privately, using one of these channels:

1. **GitHub private vulnerability reporting**, when it is enabled on the affected repository. If the "Report a vulnerability" option appears in the repository's Security tab, use it.
2. **A private contact published by the maintainers**, when one is listed in this file or in the affected repository's README.

**Pending:** no dedicated security contact has been published yet. Until one is available, use private vulnerability reporting on the affected repository when the option exists. If it does not, open a plain issue requesting a private contact channel, without including any vulnerability details, and the maintainers will reply with instructions.

## What to include in a report

Include as much of the following as you can:

- The affected repository, and the version, tag, or commit where the vulnerability occurs.
- A description of the vulnerability and its potential impact.
- Steps to reproduce, including any required configuration or data.
- Proof of concept, exploit code, or screenshots, if available.
- Suggested fixes or mitigations, if you have them.
- Whether the vulnerability has been disclosed anywhere else, and where.

Reports that allow a maintainer to reproduce the problem are acted on first.

## What must not be published

Do not include the following in public issues, pull requests, commit messages, or screenshots:

- Credentials, API keys, tokens, or connection strings.
- Personal data of users, clients, or third parties.
- Details of an exploitable vulnerability before a fix or coordinated disclosure is agreed.
- Infrastructure information such as internal hostnames, IP addresses, or private endpoints.

When logs or screenshots are needed, redact sensitive values before posting them.

## How reports are handled

Zenith projects are maintained in spare capacity, and no response time, fix deadline, or remediation guarantee is defined. In general:

- Reports are read and triaged as capacity allows.
- If the report is accepted, maintainers will coordinate with the reporter on disclosure and, when possible, on a fix and credit.
- If the report cannot be reproduced or is out of scope, the reporter will be told so when communication is possible.
- Severity, priority, and release decisions are made in the affected product's repository.

The reporter is asked to keep the issue confidential until maintainers confirm a fix or agree on a disclosure date.

## Scope

This policy covers vulnerabilities in the code and configuration of the repositories in the [catalog](docs/projects.md). It does not cover:

- Vulnerabilities in third-party dependencies, which should be reported to the corresponding project, though maintainers appreciate being informed so they can upgrade.
- Products or services that are not published in a Zenith repository.
- General bug reports, which belong in the repository's public issue tracker (see [CONTRIBUTING.md](CONTRIBUTING.md)).
