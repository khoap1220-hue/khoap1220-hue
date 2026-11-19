# Khoa Phan (Phan Đăng Khoa) 👋

**Polyglot Systems, Web3 & AI/MCP Architect (`Rust` • `Go` • `TS` • `Python`) | 13 Merged Upstream PRs • 6 MIT GuardKits (`GPG-Signed`) | [`khoaphan.dev`](https://khoap1220-hue.github.io/)**

> *"I architect and ship production-grade primitives across **Rust**, **Go**, **TypeScript**, and **Python** — backed by deterministic unit & concurrency test suites (`cargo test`, `go test -race`), GPG-signed MIT developer GuardKits, and live-verifiable upstream open-source merges."*

I build high-reliability **Rust & WebAssembly cryptographic toolkits**, **fault-tolerant Go backends & indexers**, **idempotent TypeScript/Next.js Web3 & MCP SDKs**, and **defensive Python/FastAPI financial & streaming systems**.

![Rust](https://img.shields.io/badge/Rust_&_Wasm-000000?style=flat-square&logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go_1.22+-00ADD8?style=flat-square&logo=go&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python_/_FastAPI-3776AB?style=flat-square&logo=python&logoColor=white)
![Stellar Soroban](https://img.shields.io/badge/Stellar_/_Soroban_XDR-7D00FF?style=flat-square&logo=stellar&logoColor=white)
![Solana](https://img.shields.io/badge/Solana_/_Anchor-14F195?style=flat-square&logo=solana&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js_/_React_19-000000?style=flat-square&logo=next.js&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_/_SQLite-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![GPG Signed GuardKits](https://img.shields.io/badge/MIT_GuardKits-GPG_Signed-2ea44f?style=flat-square&logo=github&logoColor=white)

---

### 🕹️ Playable 3D Arcade Mini-Game & Pinned Open-Source Toolkits *(Click Arcade Screen to Play 60-FPS 3D Game!)*

<p align="center">
  <a href="https://khoap1220-hue.github.io/">
    <img src="https://raw.githubusercontent.com/khoap1220-hue/khoap1220-hue/main/assets/3d/hero-3d-command-center.svg?v=5" width="99%" alt="Playable 60-FPS 3D Mini-Game: POLYGLOT CORE DEFENDER 3D — Click to Play Live!" />
  </a>
</p>

<p align="center">
  <a href="https://khoap1220-hue.github.io/"><img src="https://img.shields.io/badge/🕹️_PLAY_LIVE_60--FPS_3D_MINI--GAME-Mouse_/_WASD_+_Retro_Synth_SFX-238636?style=for-the-badge" alt="Play 60-FPS 3D Mini-Game" /></a>
  <a href="https://github.com/khoap1220-hue/khoap1220-hue/blob/main/assets/3d/matrix-polyhedron-core.stl"><img src="https://img.shields.io/badge/🧊_OPEN_360°_WEBGL_3D_MODEL-.STL_CAD_Mesh_(196_Facets)-1f6feb?style=for-the-badge" alt="Open 360 WebGL STL Model" /></a>
</p>

<details>
  <summary>🎮 <b>Quick-Play Directly Inside This README (Zero Page Leave): "3:00 AM Production Incident Commander" (3 Boss Waves) — Click to Start!</b></summary>
  <br/>
  <blockquote>
    <b>🚨 BOSS WAVE 1 / 3 — THE 20x CONCURRENT WEBHOOK STORM:</b><br/>
    A payment gateway fires <b>20 identical transfer webhooks within 2 milliseconds</b> during a network retry storm. Your database balance ledger is about to credit the user 20 times! <b>Choose your defense weapon:</b>
  </blockquote>

  <details>
    <summary>👉 <b>[Option A]</b> Run <code>SELECT * FROM payments WHERE ref = ?</code> followed by <code>INSERT</code></summary>
    <blockquote>
      ❌ <b>GAME OVER (TOCTOU Race Condition!):</b> All 20 concurrent requests pass the <code>SELECT</code> check within the same 2ms window before the first <code>INSERT</code> commits. Balance credited 20×!<br/>
      🔄 <i>Try Option B below!</i>
    </blockquote>
  </details>

  <details>
    <summary>👉 <b>[Option B]</b> Deploy <b><code>ts-idempotent-webhook-guard</code></b> (In-Flight <code>Promise.all</code> Lock + JSONL Write-Ahead Log)</summary>
    <blockquote>
      🏆 <b>CRITICAL HIT (+2,500 XP • 2.5x COUNTER)!</b> Request #1 acquires the in-flight mutex and writes to the durable JSONL WAL; Requests #2–#20 immediately receive <code>{ duplicate: true }</code> in <code>0.08ms</code>!<br/><br/>
      <b>🔥 UNLOCKED BOSS WAVE 2 / 3 — THE SPLIT-PACKET SSE SECRET LEAK:</b><br/>
      An AI streaming endpoint splits an OpenAI secret key across two TCP chunks: Chunk 1 ends with <code>sk-proj-abc</code> and Chunk 2 starts with <code>1234567890...</code>. Per-chunk regex misses it! <b>Choose your next weapon:</b>

      <details>
        <summary>👉 <b>[Deploy 🐍 <code>py-stream-and-billing-guard</code>]</b> Cross-Chunk <code>SSEFrameAssembler</code> + Sliding-Window DLP</summary>
        <blockquote>
          🏆 <b>DOUBLE KILL (+5,000 XP)!</b> The W3C SSE frame assembler reconstructs split chunks across TCP boundaries and redacts the leaked token before flush!<br/><br/>
          <b>👑 FINAL BOSS WAVE 3 / 3 — THE TAMPERED STELLAR XDR LEDGER HEADER:</b><br/>
          A malicious RPC node feeds your indexer a 400-byte binary <code>LedgerHeader</code> XDR frame with a forged <code>previous_ledger_hash</code> link at sequence <code>#54,000,002</code>!

          <details>
            <summary>👉 <b>[Unleash 🦀 <code>soroban-xdr-proof-kit</code> + 🐹 <code>go-preflight-sql-guard</code>]</b> RFC 4506 Binary XDR + FIPS 180-4 SHA-256 Ancestry Proof</summary>
            <blockquote>
              🎉 <b>VICTORY — SOVEREIGN POLYGLOT ARCHITECT RANK UNLOCKED! (SCORE: 15,000 / 15,000 • 99.999% UPTIME)</b><br/>
              ✔ Forged XDR frame rejected in <code>0.12ms</code> via deterministic SHA-256 hash-link verification!<br/>
              👉 <b>Want real-time 60-FPS 3D action with Mouse/WASD aiming &amp; sound? <a href="https://khoap1220-hue.github.io/">Launch the full 3D WebGL/Canvas Arcade Game here ↗</a></b>
            </blockquote>
          </details>
        </blockquote>
      </details>
    </blockquote>
  </details>
</details>

<br/>

<p align="center">
  <a href="https://github.com/khoap1220-hue/soroban-xdr-proof-kit"><img src="https://raw.githubusercontent.com/khoap1220-hue/khoap1220-hue/main/assets/pins/soroban-xdr-proof-kit.svg?v=4" width="49%" alt="soroban-xdr-proof-kit" /></a>
  <a href="https://github.com/khoap1220-hue/go-preflight-sql-guard"><img src="https://raw.githubusercontent.com/khoap1220-hue/khoap1220-hue/main/assets/pins/go-preflight-sql-guard.svg?v=4" width="49%" alt="go-preflight-sql-guard" /></a>
</p>
<p align="center">
  <a href="https://github.com/khoap1220-hue/ts-idempotent-webhook-guard"><img src="https://raw.githubusercontent.com/khoap1220-hue/khoap1220-hue/main/assets/pins/ts-idempotent-webhook-guard.svg?v=4" width="49%" alt="ts-idempotent-webhook-guard" /></a>
  <a href="https://github.com/khoap1220-hue/py-stream-and-billing-guard"><img src="https://raw.githubusercontent.com/khoap1220-hue/khoap1220-hue/main/assets/pins/py-stream-and-billing-guard.svg?v=4" width="49%" alt="py-stream-and-billing-guard" /></a>
</p>
<p align="center">
  <a href="https://github.com/khoap1220-hue/solana-validator-ordering-post-alpenglow"><img src="https://raw.githubusercontent.com/khoap1220-hue/khoap1220-hue/main/assets/pins/solana-validator-ordering-post-alpenglow.svg?v=4" width="49%" alt="solana-validator-ordering-post-alpenglow" /></a>
  <a href="https://github.com/khoap1220-hue/Master-Lab"><img src="https://raw.githubusercontent.com/khoap1220-hue/khoap1220-hue/main/assets/pins/Master-Lab.svg?v=4" width="49%" alt="Master-Lab" /></a>
</p>

---

### 🏆 Pinned Career Proof — Verified Upstream Highlights *(Click-to-Verify in 5 Seconds)*

| # | Proof Category | Upstream Organization & Repo | Tech Stack | Delivered Engineering Solution | Verifiable Proof Link |
| :-: | :--- | :--- | :--- | :--- | :--- |
| **1** | **🟣 Merged Upstream Code** | **[Externalize-Labs/externalize](https://github.com/Externalize-Labs/externalize)** | `Rust` `WebAssembly` `Stellar XDR` | Exported cryptographic `proveAncestor` verifier to the WebAssembly package (`wasm-bindgen`), enforcing `certified_seq` bounds & full browser/Node test parity. | [🟣 **PR #39 Merged**](https://github.com/Externalize-Labs/externalize/pull/39) • [Commit `a927da3`](https://github.com/Externalize-Labs/externalize/commit/a927da3a82eb66089bfe3eba18f08a00eea8f65a) (`11/11 CI Green`) |
| **2** | **🟣 Merged Upstream Code** | **[anza-xyz/cargo-build-sbf](https://github.com/anza-xyz/cargo-build-sbf)** | `Rust` `Solana SBF` `Compiler` | Deduplicated SBF syscall symbol table by referencing canonical `solana_define_syscall::definitions::SYSCALLS` inside Anza's official Solana SBF Cargo builder. | [🟣 **PR #116 Merged**](https://github.com/anza-xyz/cargo-build-sbf/pull/116) (`Merged Nov 04, 2026`) |
| **3** | **🟣 Merged Upstream Code** | **[sorotrail/SoroBeacon](https://github.com/sorotrail/SoroBeacon)** & **[tldr-pages/tldr](https://github.com/tldr-pages/tldr)** | `Python` `OpenAPI` `Stellar CLI` | Generated typed Python client SDK from Soroban RPC OpenAPI spec (`#680`) & authored official `stellar-cli` smart contract reference (`#24925`, `64k+ ⭐`). | [🟣 **SoroBeacon #680 Merged**](https://github.com/sorotrail/SoroBeacon/pull/680) • [🟣 **tldr #24925 Merged**](https://github.com/tldr-pages/tldr/pull/24925) |
| **4** | **🟣 Credited in `main`** | **[BasedHardware/omi](https://github.com/BasedHardware/omi)** *(8k+ ⭐)* | `Python` `FastAPI` `Stripe API` | Boundary-case verification & ISO-4217 Zero-Decimal (`JPY`) Stripe subscription schedule safety explicitly credited by maintainer in merged PR `#23591`. | [🟣 **Credited in Main (#23591)**](https://github.com/BasedHardware/omi/pull/23591) |
| **5** | **🟡 Open PR (In Review)** | **[aibtcdev/x402-api](https://github.com/aibtcdev/x402-api)** & **[solana-foundation/program-examples](https://github.com/solana-foundation/program-examples)** | `TypeScript` `Cloudflare DO` `Solana PDA` | Migrated HTTP 402 payment middleware & polling Durable Object to typed `X402_RELAY` RPC binding (`#150`) + clarified PDA rent-payer balance invariants (`#760`). | [🟡 **x402-api #150 (Open)**](https://github.com/aibtcdev/x402-api/pull/150) • [🟡 **program-examples #760 (Open)**](https://github.com/solana-foundation/program-examples/pull/760) |
| **6** | **🟡 Open PR (CI Green)** | **[BAWES-Universe/studenthub](https://github.com/BAWES-Universe/studenthub)** & **[PayStell](https://github.com/PayStell/paystell-website)** | `PHP/Yii2` `Next.js` `AWS S3 / Stellar` | Enforced atomic `DB-save-before-S3-delete` Civil ID ordering (`#128`, `3/3 CI Gates`) & 4-step Stellar wallet withdrawal stepper with Ed25519/reserve guards (`#141`). | [🟡 **studenthub #128 (Open)**](https://github.com/BAWES-Universe/studenthub/pull/128) • [🟡 **PayStell #141 (Open)**](https://github.com/PayStell/paystell-website/pull/141) |

---

### 🎁 Featured Open-Source Community Toolkits *(Free & MIT Licensed — Built & Used Daily)*

I actively extract and publish my core engineering primitives as **free, zero-bloat MIT open-source libraries** (`LICENSE` verified across all 6 repositories) for the global developer community:

| # | Public Community Repository | Stack & CI Verification | What It Solves for the Community (and My Daily Production Stack) |
| :-: | :--- | :--- | :--- |
| **1** | **[`soroban-xdr-proof-kit`](https://github.com/khoap1220-hue/soroban-xdr-proof-kit)** | `Rust` `WebAssembly` `CLI` `MIT` | Pure-Rust **FIPS 180-4 SHA-256 engine**, **RFC 4506 binary `LedgerHeader` XDR decoder/serializer** (4-byte padding & RFC 5528 record marks), hash-link ancestry verifier, and History Archive checkpoint CLI. |
| **2** | **[`go-preflight-sql-guard`](https://github.com/khoap1220-hue/go-preflight-sql-guard)** | `Go 1.22+` `database/sql` `CLI` `MIT` | **`database/sql` connection pool & read-only SQL sanitizer**, **zero-CGo SQLite3 100-byte binary header & WAL inspector**, remote Postgres TLS DSN validator, degradation circuit breaker, and query cost tracker. |
| **3** | **[`ts-idempotent-webhook-guard`](https://github.com/khoap1220-hue/ts-idempotent-webhook-guard)** | `TypeScript` `Node.js` `CLI` `MIT` | **Concurrent `Promise.all` webhook idempotency lock** with durable **JSONL Write-Ahead Log (`FileWalIdempotencyStore`)**, constant-time **HMAC-SHA256 & Stripe replay-window verifier**, IPv4/IPv6 SSRF guard, and Luhn/JWT log redactor. |
| **4** | **[`py-stream-and-billing-guard`](https://github.com/khoap1220-hue/py-stream-and-billing-guard)** | `Python 3.10+` `FastAPI` `CLI` `MIT` | **W3C SSE cross-chunk stream framing normalizer & split-token leak scanner**, integer-only `divmod` **ISO-4217 0/2/3-decimal (`JPY`/`USD`/`KWD`) & basis-point proration guard**, and `SubscriptionSchedule` transition lock. |
| **5** | **[`solana-validator-ordering-post-alpenglow`](https://github.com/khoap1220-hue/solana-validator-ordering-post-alpenglow)** | `Python` `Rust` `Solana RPC` `MIT` | Quantitative telemetry & empirical statistical benchmark suite analyzing **Solana Mainnet validator transaction ordering** across Jito, Frankendancer, and Agave post-Alpenglow. |
| **6** | **[`Master-Lab`](https://github.com/khoap1220-hue/Master-Lab)** & **[`Phan-ng-Khoa`](https://github.com/khoap1220-hue/Phan-ng-Khoa)** | `TypeScript` `React 19` `Vite` `MIT` | Open-source **Multimodal AI Creative Workbench** and **Sketch-to-UI Design System & Accessibility Token Auditor**. |

---

### 🚀 Selected Open-Source Contributions *(13 Live Merged Upstream PRs 🟣 • 1 Credited in `BasedHardware/omi` Main 🟣 • Selected Open PRs in Review 🟡)*

| Repository | Stack | Engineering Scope & Contribution | Exact Status & Verification |
| :--- | :--- | :--- | :--- |
| **[Externalize-Labs/externalize](https://github.com/Externalize-Labs/externalize)** | `Rust` `WebAssembly` `Stellar XDR` | Export cryptographic `proveAncestor` verifier to the WebAssembly package with `certified_seq` parity & `wasm-bindgen` test suite (Merged by `@samjay8` at `a927da3`) | [PR #39 🟣 Merged](https://github.com/Externalize-Labs/externalize/pull/39) |
| **[anza-xyz/cargo-build-sbf](https://github.com/anza-xyz/cargo-build-sbf)** | `Rust` `Solana SBF` | Use `solana_define_syscall::definitions::SYSCALLS` instead of local copy in Solana's SBF Cargo toolchain | [PR #116 🟣 Merged](https://github.com/anza-xyz/cargo-build-sbf/pull/116) |
| **[sorotrail/SoroBeacon](https://github.com/sorotrail/SoroBeacon)** | `Python` `Soroban RPC` `OpenAPI` | `feat(clients)`: generate typed Python client SDK from the Soroban RPC OpenAPI specification | [PR #680 🟣 Merged](https://github.com/sorotrail/SoroBeacon/pull/680) |
| **[tldr-pages/tldr](https://github.com/tldr-pages/tldr)** | `Stellar CLI` `Documentation` | Official CLI command reference for `stellar-cli` smart contract deployment & network configuration (`64k+ ⭐ repository`) | [PR #24925 🟣 Merged](https://github.com/tldr-pages/tldr/pull/24925) |
| **[Wayfare-labs/wayfare](https://github.com/Wayfare-labs/wayfare)** | `Runbook` `Incident Response` | `docs`: add operational runbook for responding to a wrong published figure (`#730`) | [PR #860 🟣 Merged](https://github.com/Wayfare-labs/wayfare/pull/860) |
| **[MMM-pay/payflow-docs](https://github.com/MMM-pay/payflow-docs)** | `FinTech Docs` `WCAG A11y` | `docs`: add WCAG accessibility statement & compliance baseline | [PR #107 🟣 Merged](https://github.com/MMM-pay/payflow-docs/pull/107) |
| **[ritik4ever/stellar-stream](https://github.com/ritik4ever/stellar-stream)** | `TypeScript` `React` `A11y` | `feat(a11y)`: add ARIA accessibility audit helpers and keyboard navigation fixes (`#760`) | [PR #1436 🟣 Merged](https://github.com/ritik4ever/stellar-stream/pull/1436) |
| **[Farm-credit/stellar-app-os](https://github.com/Farm-credit/stellar-app-os)** | `TypeScript` `Stellar` | `feat(species)`: IUCN endangered species prioritisation engine & 3 merged feature modules | [PR #1797 🟣 Merged](https://github.com/Farm-credit/stellar-app-os/pull/1797) / [PR #1798 🟣 Merged](https://github.com/Farm-credit/stellar-app-os/pull/1798) / [PR #1799 🟣 Merged](https://github.com/Farm-credit/stellar-app-os/pull/1799) |
| **[ritik4ever/stellar-goal-vault](https://github.com/ritik4ever/stellar-goal-vault)** | `TypeScript` `Soroban` | `feat(discovery)`: campaign category browsing & multi-facet filter helpers across 3 merged PRs | [PR #1377 🟣 Merged](https://github.com/ritik4ever/stellar-goal-vault/pull/1377) / [PR #1378 🟣 Merged](https://github.com/ritik4ever/stellar-goal-vault/pull/1378) / [PR #1379 🟣 Merged](https://github.com/ritik4ever/stellar-goal-vault/pull/1379) |
| **[BasedHardware/omi](https://github.com/BasedHardware/omi)** | `Python` `FastAPI` `Stripe Billing` | Boundary-case verification for multi-currency Stripe subscription schedules explicitly credited by maintainer in `main` merge `#23591` | [🟣 Credited in Main (#23591)](https://github.com/BasedHardware/omi/pull/23591) |
| **[aibtcdev/x402-api](https://github.com/aibtcdev/x402-api)** | `TypeScript` `Cloudflare Workers` | `feat(x402)`: migrate payment middleware and polling Durable Object to `X402_RELAY` RPC binding | [PR #150 🟡 Open (In Review)](https://github.com/aibtcdev/x402-api/pull/150) |
| **[solana-foundation/program-examples](https://github.com/solana-foundation/program-examples)** | `Solana PDA` `Security Docs` | `docs(pda-rent-payer)`: clarify user balance check in README (`5/5 Greptile Score & CI Green`) | [PR #760 🟡 Open (In Review)](https://github.com/solana-foundation/program-examples/pull/760) |
| **[BAWES-Universe/studenthub](https://github.com/BAWES-Universe/studenthub)** | `PHP/Yii2` `TypeScript` `AWS S3` | Transactional DB-commit-before-S3-delete Civil ID flow & AWS MediaConvert credential hardening (`3/3 CI Gates Green`) | [PR #128 🟡 Open (CI Green)](https://github.com/BAWES-Universe/studenthub/pull/128) |
| **[PayStell/paystell-website](https://github.com/PayStell/paystell-website)** | `Next.js` `TypeScript` `Stellar SDK` | 4-step Stellar wallet withdrawal flow with Stepper UX, Ed25519 address validation, reserve guards, 2FA & ARIA accessibility | [PR #141 🟡 Open (CI Green)](https://github.com/PayStell/paystell-website/pull/141) |
| **[TheSolaAI/sola-application](https://github.com/TheSolaAI/sola-application)** | `Next.js` `TypeScript` `Solana Blinks` | Custom handsfree Solana `BlinkMessageItem` execution component & `getBlinks` AI tool integration (`@sourcery-ai LGTM`) | [PR #496 🟡 Open (Sourcery LGTM)](https://github.com/TheSolaAI/sola-application/pull/496) |
| **[openwallet-foundation-labs/sd-jwt-python](https://github.com/openwallet-foundation-labs/sd-jwt-python)** | `Python` `SD-JWT` `Cryptography` | `fix(verifier)`: enforce `exp`/`nbf`/`iat` claims and derive KB-JWT `alg` from JWK | [PR #30 🟡 Open (CI Clean)](https://github.com/openwallet-foundation-labs/sd-jwt-python/pull/30) |
| **[wraith-protocol/contracts](https://github.com/wraith-protocol/contracts)** | `Rust` `CKB` `Fuzzing` | `feat(ckb)`: add malformed-witness and type-script fuzz corpus | [PR #285 🟡 Open (CI Clean)](https://github.com/wraith-protocol/contracts/pull/285) |
| **[Altacon-Labs/RevMarket](https://github.com/Altacon-Labs/RevMarket)** | `Go / SQLite` `Indexer` | `feat(backend)`: index confirmed market events with durable SQLite checkpoints | [PR #42 🟡 Open (CI Clean)](https://github.com/Altacon-Labs/RevMarket/pull/42) |
| **[Miracle656/veil](https://github.com/Miracle656/veil)** | `Mobile` `TypeScript` | `feat(mobile)`: add four notification categories with server sync (`#1287`) | [PR #1350 🟡 Open (In Review)](https://github.com/Miracle656/veil/pull/1350) |

---

### 🛡️ Application & AI/ML Security Engineering *(Defensive Overview)*

In addition to feature and protocol engineering, I conduct defensive security auditing and build fail-closed safeguards across Web3 and AI/ML infrastructure *(adhering strictly to responsible disclosure — only defensive methodologies are summarized publicly)*:

- **Stream & Transport Framing Integrity:** Mitigating cross-chunk framing discrepancies (`CWE-444`) in Server-Sent Events (SSE) and streaming LLM proxies by enforcing full-frame reassembly before guardrail inspection.
- **Transactional Cloud & Financial State Safety:** Enforcing strict `DB-Commit-Before-External-Mutation` ordering (preventing premature cloud asset deletion or billing schedule corruption) and integer minor-unit math (`Zero-Decimal` & basis points).
- **Fail-Closed Authentication & Dependency Gates:** Hardening signature verification (`Ed25519` / `HMAC`), preventing SSRF on user-supplied webhook endpoints, and ensuring `bun/cargo/npm` security audit gates never fail open on unparseable output.

---

### 🔒 Commercial & Enterprise Systems Background *(Proprietary / Under NDA)*

Beyond my open-source repositories and community toolkits above, I have architected and operated **35+ proprietary production systems** under commercial and client NDAs:
- **Enterprise ERP, PropTech & Operations Platforms:** Local-first resource planning, construction/project management dashboards, and automated property management suites.
- **High-Concurrency FinTech & E-Commerce Fulfillment:** Sub-50ms idempotent banking webhook processors, atomic inventory ledgers, and automated warranty fulfillment engines.
- **Multimodal AI, Voice Synthesis & 3D Pipelines:** Neural TTS/ASR audio mastering (`-14 LUFS`), programmatic 3D/VRM generation, and high-speed desktop/browser RPA infrastructure.

---

### 🟢 Collaboration, Grants & Hiring Readiness *(For CTOs, Maintainers & Recruiters)*

| Engagement Track | Core Stack & Domain | Delivery Standard & Verification Guarantee | Response SLA |
| :--- | :--- | :--- | :---: |
| **1. Protocol Grants & Ecosystem Waves** | `Rust` `Soroban / Stellar XDR` `Solana / Anchor` `WebAssembly` | End-to-end RFC/XDR compliance, deterministic unit & integration suites (`cargo test` / `wasm-bindgen-test`), **GPG-Signed (`Verified`)** release commits. | **`< 2 Hours`** |
| **2. Paid Bounties & Production Trials** | `Go 1.22+` `TypeScript / Next.js` `Python / FastAPI` `PostgreSQL` | Clean single-commit atomic PRs, zero linter regressions, race-detector verified (`go test -race`), ready to merge within **4–6 hours** of assignment. | **`< 2 Hours`** |
| **3. Defensive Security & FinTech Audits** | `SSE / LLM Proxy Framing` `Stripe / Webhook Idempotency` `SSRF / Auth` | Reproducible containerized PoCs, fail-closed remediation patches, and strict responsible disclosure. | **`< 4 Hours`** |
| **4. Senior Systems / Web3 Engineering Roles** | `Distributed Systems` `Blockchain Indexers` `High-Throughput Backends` | Full-time remote, contract, or technical advisory across `UTC+7` / US / EU overlapping hours. | **`< 4 Hours`** |

- **Flagship Website:** [khoaphan.dev](https://khoap1220-hue.github.io/) • **GitHub:** [@khoap1220-hue](https://github.com/khoap1220-hue)
- **Open-Source Community Kits (`MIT`):** [`soroban-xdr-proof-kit`](https://github.com/khoap1220-hue/soroban-xdr-proof-kit/releases) • [`go-preflight-sql-guard`](https://github.com/khoap1220-hue/go-preflight-sql-guard/releases) • [`ts-idempotent-webhook-guard`](https://github.com/khoap1220-hue/ts-idempotent-webhook-guard/releases) • [`py-stream-and-billing-guard`](https://github.com/khoap1220-hue/py-stream-and-billing-guard/releases)
- **Location:** Vietnam (`UTC+7` — Global Remote Coverage)
