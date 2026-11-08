<p align="center">
  <a href="https://github.com/rootless-sec">
    <img src="https://raw.githubusercontent.com/rootless-sec/.github/main/assets/avatar.png" alt="Rootless Security" width="80" height="80" />
  </a>
</p>

<h1 align="center">Rootless Security</h1>

<p align="center">
  Unprivileged security tooling, protocol verification engines, and standalone systems software.
</p>

---

Most security and operational tools assume root privileges, heavy runtime dependencies, and external database servers to do basic work.

We build tools that do the opposite: self-contained binaries and clean packages that run as standard users, store state in embedded engines like SQLite, and inspect wire protocols deterministically.

### Projects

- **[relaygate](https://github.com/rootless-sec/relaygate)**: Self-hosted webhook ingestion gateway, cryptographic signature verifier, and dead-letter queue replay engine in a single Go binary with an embedded management UI.
- **[tanuki](https://github.com/Mafifrizi/tanuki)**: Unprivileged Active Directory and Kerberos operator for Linux, implementing RFC 4120, RFC 6113 FAST armoring, and MS-PAC decoding.
- **[ARES](https://github.com/TifalAbdusyahid/ARES)**: Red-team engagement automation platform with strict execution scoping and encrypted vault storage.

### Principles

- **Unprivileged by design**: Runs under standard user accounts without `sudo`, setuid binaries, or elevated privileges.
- **Embedded persistence**: Zero external database servers. Local state uses embedded SQLite in Write-Ahead Logging (WAL) mode.
- **Deterministic protocols**: Constant-time cryptographic verification and strict parser bounds on wire payloads.

### Maintainers

Maintained by [@Mafifrizi](https://github.com/Mafifrizi) and [@TifalAbdusyahid](https://github.com/TifalAbdusyahid).

To report a vulnerability, see [SECURITY.md](https://github.com/rootless-sec/.github/blob/main/SECURITY.md) or contact `hazama3321@gmail.com`.
