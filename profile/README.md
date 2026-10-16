<p align="center">
  <a href="https://github.com/rootless-sec">
    <img src="https://raw.githubusercontent.com/rootless-sec/.github/main/assets/avatar.png" alt="Rootless Security" width="96" height="96" />
  </a>
</p>

<h1 align="center">Rootless Security</h1>

<p align="center">
  Self-hosted infrastructure, protocol verification engines, and unprivileged security tooling.
</p>

---

Rootless Security is an engineering collective founded by [@Mafifrizi](https://github.com/Mafifrizi) and [@TifalAbdusyahid](https://github.com/TifalAbdusyahid). We build standalone systems software and offensive security tools that run without elevated host privileges, external database servers, or heavy runtime dependencies.

Our work focuses on three areas: webhook and message ingestion infrastructure, Active Directory and Kerberos wire-level protocol tooling on Linux, and automated red-team operations with strict OPSEC controls. Every tool in this organization is designed to ship as a self-contained binary or standard-library package that operators can audit and deploy on a single host.

### Repositories

| Repository | Scope | Stack | Maintainers |
| :--- | :--- | :--- | :--- |
| **[relaygate](https://github.com/rootless-sec/relaygate)** | Webhook ingestion gateway, cryptographic signature verifier, and dead-letter replay engine with an embedded web console | Go, SQLite (WAL), React, TypeScript | [@Mafifrizi](https://github.com/Mafifrizi), [@TifalAbdusyahid](https://github.com/TifalAbdusyahid) |
| **[tanuki](https://github.com/Mafifrizi/tanuki)** | Unprivileged Active Directory and Kerberos operator for Linux (RFC 4120, RFC 6113 FAST armoring, MS-PAC decoding) | Rust, Python stdlib | [@Mafifrizi](https://github.com/Mafifrizi) |
| **[ARES](https://github.com/TifalAbdusyahid/ARES)** | Red-team engagement automation and OPSEC workflow orchestration | Python, TypeScript | [@TifalAbdusyahid](https://github.com/TifalAbdusyahid) |

### Engineering Standards

All projects under Rootless Security follow the same operational rules:

1. No root or `sudo` requirement at runtime. Tools operate within unprivileged user namespaces and standard file permissions.
2. Zero external infrastructure for core persistence. Where local state is needed, we use embedded SQLite in Write-Ahead Logging (WAL) mode with pure-Go or native drivers.
3. Explicit cryptographic and protocol verification. Signatures, tokens, and wire payloads are validated with constant-time comparisons and strict parser bounds before dispatch.

### Maintainers

| Maintainer | Role | GitHub |
| :--- | :--- | :--- |
| **Mafifrizi** | Systems Architecture & Identity Protocols | [@Mafifrizi](https://github.com/Mafifrizi) |
| **Tifal Abdusyahid** | Security Automation & Fullstack Engineering | [@TifalAbdusyahid](https://github.com/TifalAbdusyahid) |

### Security Disclosures

To report a vulnerability in any Rootless Security repository, see [SECURITY.md](https://github.com/rootless-sec/.github/blob/main/SECURITY.md) or contact `hazama3321@gmail.com`.
