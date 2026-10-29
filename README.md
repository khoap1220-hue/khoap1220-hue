### Hi, I'm Khoa Phan (`@khoap1220-hue`) 👋

**Systems, WebAssembly & Distributed Ledger Engineer** focused on deterministic cryptographic verification, Stellar History Archive / XDR tooling, and high-reliability backend infrastructure in **Rust**, **Go**, and **TypeScript**.

[![Rust](https://img.shields.io/badge/Rust-2021%20%2F%20Wasm-000000?style=flat-square&logo=rust)](https://github.com/khoap1220-hue/stellar-xdr-checkpoint-toolkit)
[![Go](https://img.shields.io/badge/Go-1.24-00ADD8?style=flat-square&logo=go)](https://github.com/khoap1220-hue/stellar-xdr-checkpoint-toolkit)
[![Stellar](https://img.shields.io/badge/Stellar-XDR%20%26%20Soroban-7D00FF?style=flat-square&logo=stellar)](https://github.com/Externalize-Labs/externalize/pull/39)
[![GPG Verified](https://img.shields.io/badge/Commits-GPG%20Verified-2ea44f?style=flat-square&logo=github)](https://github.com/khoap1220-hue)

---

### 🛠️ Core Engineering Domains

| Domain | Stack & Tooling | Focus Areas |
| :--- | :--- | :--- |
| **Cryptographic & Archive Verification** | `Rust`, `wasm-bindgen`, `stellar-xdr`, `SHA-256` | RFC 4506 XDR frame parsing, `LedgerHeaderHistoryEntry` ancestry hash chains, 64-ledger checkpoint alignment |
| **High-Throughput Archive Serving** | `Go 1.24`, `net/http`, `OpenAPI 3.0` | Immutable `.xdr.gz` checkpoint streaming, strong `ETag` (`If-None-Match` / `304`), bounded concurrency |
| **Smart Contracts & Full-Stack Web3** | `Soroban SDK`, `Anchor`, `Next.js`, `TypeScript` | Property-based cross-language layout verification, deterministic state transitions, zero-regression test suites |

---

### 📌 Selected Open-Source Contributions & Projects

| Project / Repository | Contribution Summary | Stack |
| :--- | :--- | :---: |
| [**`Externalize-Labs/externalize#39`**](https://github.com/Externalize-Labs/externalize/pull/39) *(Merged)* | Exported `proveAncestor` in the `externalize-wasm` WebAssembly package with Node.js & headless browser verification for contiguous `previous_ledger_hash` chains | `Rust` · `Wasm` |
| [**`khoap1220-hue/stellar-xdr-checkpoint-toolkit`**](https://github.com/khoap1220-hue/stellar-xdr-checkpoint-toolkit) | Deterministic Stellar History Archive checkpoint boundary arithmetic (`(cp + 1) % 64 == 0`), RFC 4506 XDR frame splitter, and Go HTTP immutable cache handlers | `Rust` · `Go` |
| [**`tldr-pages/tldr#24925`**](https://github.com/tldr-pages/tldr/pull/24925) *(52K+ ⭐)* | Authored the CLI documentation page for the official Stellar / Soroban CLI (`pages/common/stellar.md`) | `CLI` · `Docs` |
| [**`solana-foundation/program-examples#760`**](https://github.com/solana-foundation/program-examples/pull/760) | Documented caller authority verification invariants for `pda-rent-payer` across Anchor, Native Rust, and Pinocchio | `Rust` · `Solana` |
| [**`BAWES-Universe/studenthub#128`**](https://github.com/BAWES-Universe/studenthub/pull/128) | Eliminated hardcoded S3/MediaConvert credentials and hardened atomic upload validation ordering | `PHP` · `AWS S3` |

---

### ✅ Engineering Principles

- **Deterministic Verification First:** Every PR is backed by unit, boundary, and tamper-rejection tests (`cargo test --workspace`, `cargo clippy -- -D warnings`, `go test -race ./...`).
- **Minimal, Surgical Diffs:** Strict adherence to repository architecture, MSRV constraints, and GPG-verified commit provenance.
