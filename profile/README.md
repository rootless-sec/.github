<p align="center">
  <a href="https://github.com/rootless-sec">
    <img src="https://raw.githubusercontent.com/rootless-sec/.github/main/assets/avatar.png" alt="Rootless Security" width="72" height="72" />
  </a>
</p>

<h1 align="center">Rootless Security</h1>

<p align="center">
  Unprivileged systems software, protocol tooling, and standalone infrastructure.
</p>

---

Rootless Security builds tools that run in unprivileged userspace (UID 1000) without `sudo`, store state in embedded SQLite WAL, and inspect wire protocols deterministically.

### Projects

- **[relaygate](https://github.com/rootless-sec/relaygate)** (Go): Self-hosted webhook ingestion gateway, cryptographic signature verifier, and dead-letter queue replay engine in a single binary.
- **[tanuki](https://github.com/Mafifrizi/tanuki)** (Rust, Python): Tactical Identity and Kerberos operator for Linux workloads (RFC 4120, RFC 6113 FAST armoring, MS-PAC decoding).
- **[ARES](https://github.com/TifalAbdusyahid/ARES)** (Python, TypeScript): Operator-directed red-team engagement platform with scoped execution controls and encrypted vault storage.

### Maintainers & Security

Maintained by [@Mafifrizi](https://github.com/Mafifrizi) and [@TifalAbdusyahid](https://github.com/TifalAbdusyahid).

For security inquiries and vulnerability disclosures, see [SECURITY.md](https://github.com/rootless-sec/.github/blob/main/SECURITY.md) or contact `hazama3321@gmail.com`.
