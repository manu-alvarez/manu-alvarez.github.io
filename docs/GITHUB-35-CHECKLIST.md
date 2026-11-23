# GitHub 35 — authoritative closure ledger

**Audit date:** 2026-11-23. **Owner:** manu-alvarez. **Scope:** all 35 repositories. **Policy:** only test-backed acceptance may close a repository. `Docs OK` and `CI OK` are scoped subtask completions, not full-project acceptance. Do not deploy to VPS as a side effect of repository work.

## Evidence-backed closures

- [x] `MSBross.me`: PR #1 merged; CI run https://github.com/manu-alvarez/MSBross.me/actions/runs/45277548898 (API, backend, four frontends, security scan passed). **Not an acceptance of FTP publication or full app behavior.**
- [x] `Agent-Sr-Smith`: PR #1 merged; full 197/197 tests, TypeScript, build in https://github.com/manu-alvarez/Agent-Sr-Smith/actions/runs/45278695989. **Not an acceptance of ZIP in a user browser.**
- [x] `CombiPro`: PR #1 merged (commit `8ae9cc225f684a71dbd8e95b361a27a32eeb2f82`); independent source restored from MSBrossAI, `npm ci`, TypeScript, audit and Vite build green in https://github.com/manu-alvarez/CombiPro/actions/runs/45281778022. **Browser/API acceptance remains pending.**
- [x] `MSBrossAI`: PR #1 merged (commit `e8ab6e6fe3c238015578d6bb1e370460ac0d3b2d`), 13/13 frontend matrix builds green in https://github.com/manu-alvarez/MSBrossAI/actions/runs/45282244889. Replaced broken automatic deployment triggers; Cloudflare is manual-only. **Application and manual deployment acceptance remain pending.**
- [x] `TaskFlowPro`: PR #1 merged (commit `05aa6292f8d526b9e719096dccfb1786a3380a08`), successful `npm ci`, TypeScript/Vite build and high-severity audit in https://github.com/manu-alvarez/TaskFlowPro/actions/runs/45283024241. **Browser CRUD/persistence acceptance remains pending.**
- [x] Documentation review: `manu-alvarez.github.io`, `ManuCodearts`, `varios-external` (previous audit; remaining live validation not completed).

## Complete inventory and next acceptance gates

| # | Repository | Current scope status | Outstanding closure gate |
|---:|---|---|---|
| 1 | [Agent-Sr-Smith](https://github.com/manu-alvarez/Agent-Sr-Smith) | CI OK; global pending | Zip and browser acceptance |
| 2 | [CalendarioMaya-ManoElectricaAzul](https://github.com/manu-alvarez/CalendarioMaya-ManoElectricaAzul) | Pending | Calendar calculations and published UI |
| 3 | [CombiPro](https://github.com/manu-alvarez/CombiPro) | Source restored, TypeScript/build/audit OK; global pending | Browser/API acceptance, confirm canonical ownership and reconcile duplicate copies |
| 4 | [Conspiracy-Projects](https://github.com/manu-alvarez/Conspiracy-Projects) | Pending | UI and navigation smoke |
| 5 | [Dream_OS](https://github.com/manu-alvarez/Dream_OS) | Pending | Run existing tests and execution smoke |
| 6 | [Edelweiss-Cumple](https://github.com/manu-alvarez/Edelweiss-Cumple) | Pending | Game/assets browser smoke |
| 7 | [FoZ-SoundPro](https://github.com/manu-alvarez/FoZ-SoundPro) | 6/6 technical tests, archive SHA-256 OK; Pages deployment under re-verification | Manual audio/browser interaction and live site acceptance |
| 8 | [IAPutaOS](https://github.com/manu-alvarez/IAPutaOS) | Pending | CI and integrations |
| 9 | [InfoCool](https://github.com/manu-alvarez/InfoCool) | Python/Next.js CI OK, PR #1 merged | Browser workflows and external-service acceptance |
| 10 | [jartos-de-tu-pelo](https://github.com/manu-alvarez/jartos-de-tu-pelo) | Pending | Frontend and publication |
| 11 | [LIVEKIT](https://github.com/manu-alvarez/LIVEKIT) | Insecure JWT fallback removed, PR #1 merged | Token endpoint abuse controls, media integration and browser acceptance |
| 12 | [LogiSearch](https://github.com/manu-alvarez/LogiSearch) | Pending | Search and persistence |
| 13 | [LogiTrack-Warehouse-System](https://github.com/manu-alvarez/LogiTrack-Warehouse-System) | Pending | Functional scope and acceptance |
| 14 | [manu-alvarez.github.io](https://github.com/manu-alvarez/manu-alvarez.github.io) | Docs OK; global pending | Live portfolio link checks |
| 15 | [ManuCodearts](https://github.com/manu-alvarez/ManuCodearts) | Docs OK; global pending | Public links/assets checks |
| 16 | [MCP-agent-memory](https://github.com/manu-alvarez/MCP-agent-memory) | SDK compatibility fixed, 164 tests pass, PR #1 merged | Eleven skipped external integration cases and live MCP acceptance |
| 17 | [Mequi3D](https://github.com/manu-alvarez/Mequi3D) | Pending | 3D viewer/assets browser smoke |
| 18 | [MOKO-TOOLS](https://github.com/manu-alvarez/MOKO-TOOLS) | Pending | Tool workflows and acceptance |
| 19 | [MSB](https://github.com/manu-alvarez/MSB) | Partial | 8 pending app routes and app catalog smoke |
| 20 | [msb-iaputa-backend](https://github.com/manu-alvarez/msb-iaputa-backend) | Pending | API and CI tests |
| 21 | [msb-livekit-backend](https://github.com/manu-alvarez/msb-livekit-backend) | JWT secret hardening and regression CI OK; PR #1 merged | Real token issuance/auth, provider connection, browser acceptance |
| 22 | [msb-traductor-backend](https://github.com/manu-alvarez/msb-traductor-backend) | Input contracts and TypeScript build OK; PR #1 merged | Real translation service and error-case acceptance |
| 23 | [MSBross.me](https://github.com/manu-alvarez/MSBross.me) | CI OK; global pending | Functional acceptance and safe FTP rollback |
| 24 | [MSBrossAI](https://github.com/manu-alvarez/MSBrossAI) | CI 13/13 OK; global pending | Source-of-truth matrix, per-app smoke and verified manual deployment |
| 25 | [MY-UNIVERSAL-AI-OS](https://github.com/manu-alvarez/MY-UNIVERSAL-AI-OS) | Partial | CI, runtime/MCP/RAG contract acceptance; do not deploy VPS |
| 26 | [NexusFlow-Framework](https://github.com/manu-alvarez/NexusFlow-Framework) | Pending | Core execution and framework acceptance |
| 27 | [PromptCombo](https://github.com/manu-alvarez/PromptCombo) | Pending | CI and UI acceptance |
| 28 | [SERVER-DEV](https://github.com/manu-alvarez/SERVER-DEV) | Partial | Infrastructure source-of-truth, deploy/secret safety |
| 29 | [SKILL-skill-forge](https://github.com/manu-alvarez/SKILL-skill-forge) | COMPLETE: official validation + 12/12 skill + MCP JSON-RPC 8/8 E2E, PR #1 merged | None for documented local generator contract |
| 30 | [Sr.Smith](https://github.com/manu-alvarez/Sr.Smith) | Partial | Reconcile Agent-Sr-Smith + ZIP acceptance |
| 31 | [Tarot-Maya](https://github.com/manu-alvarez/Tarot-Maya) | Pending | Card data and navigation |
| 32 | [tarot-rws](https://github.com/manu-alvarez/tarot-rws) | Pending | Resource integrity and Tarot-Maya relationship |
| 33 | [TaskFlowPro](https://github.com/manu-alvarez/TaskFlowPro) | CI OK; global pending | Browser CRUD/persistence acceptance and reconcile integrated version |
| 34 | [TuEnergiaMaya](https://github.com/manu-alvarez/TuEnergiaMaya) | Pending | Calculations, static resources, published smoke |
| 35 | [varios-external](https://github.com/manu-alvarez/varios-external) | Docs OK; global pending | External references check |


## November 24 verification update

- [x] `SKILL-skill-forge`: complete local generator acceptance E2E. PR https://github.com/manu-alvarez/SKILL-skill-forge/pull/1 ; run https://github.com/manu-alvarez/SKILL-skill-forge/actions/runs/45283136224 ; official Agent Skills checks, skill scaffold, MCP JSON-RPC, adversarial checks.
- [x] `FoZ-SoundPro`: 6/6 technical gates and portable ZIP/sha verified https://github.com/manu-alvarez/FoZ-SoundPro/actions/runs/45283327786 ; official live URL https://manu-alvarez.github.io/FoZ-SoundPro/ provided by owner. Pages deployment after PR #1 failed to find artifact metadata; PR #2 fixes stabilization and needs new Pages run verification. HTTP availability and browser UX not yet independently verified.
- [x] `InfoCool`: PR https://github.com/manu-alvarez/InfoCool/pull/1 merged; fixed 5 missing frontend dependencies and unsupported Next experimental config; Python tests + Next production build https://github.com/manu-alvarez/InfoCool/actions/runs/45285501885.
- [x] `LIVEKIT` and `msb-livekit-backend`: JWT signing secret no longer defaults to hard-coded value; respective PR #1 merged; token access policy still outstanding.
- [x] `msb-traductor-backend`: PR #1 merged; typed HTTP request validation, deterministic tests + build https://github.com/manu-alvarez/msb-traductor-backend/actions/runs/45282738029.
- [x] `MCP-agent-memory`: PR #1 merged; compatible MCP SDK and bounded rank fallback; https://github.com/manu-alvarez/MCP-agent-memory/actions/runs/45283930173 (164 passed, 11 skipped).
- [x] `MSB`: PR #3 merged; cross-repo build matrix verifies `Conspiracy-Projects`, `LogiSearch`, `Tarot-Maya`, `jartos-de-tu-pelo`: https://github.com/manu-alvarez/MSB/actions/runs/45284907362. Their user/browser functionality remains unverified.

## Canonical source boundaries under review

- `MSB`: GitHub Pages dashboard and `servicios.json`, not a universal source of every frontend.
- `MSBross.me`: Nominalia PHP gateway, frontend build/deploy pipeline. FTP deploy remains manual and non-atomic; no deployment was executed by the CI closure.
- `MSBrossAI/www`: prior audit found near-identical published web content; compare final files before edits.
- `SERVER-DEV`: infrastructure and deployment configuration; must not assume this repository's copies of frontends are current.
- `CombiPro`: independent repository now contains a passing standalone build sourced from a pinned MSBrossAI revision; both legacy copies still exist and require reconciliation after browser/API acceptance.
- `Agent-Sr-Smith` and `Sr.Smith` are separate repositories. One CI passing does not prove parity.

## Closure contract (applies independently to each repository)

- [ ] Verify documented purpose, canonical source, entrypoints, run/build commands and required non-secret config.
- [ ] Run relevant deterministic unit/contract tests, production build, and smoke tests appropriate for the component; record links or output.
- [ ] Verify links, external services and deployment assumptions without touching production unexpectedly.
- [ ] Fix defects at the root with a minimal, reviewed change; never remove security checks simply to make CI green.
- [ ] Merge a validated PR and record commit SHA and test evidence in this ledger.
- [ ] Mark repository `COMPLETE` only after its own requirements and outputs are validated; distinguish tests from deployed acceptance.

## Execution priority

1. Resolve shared-source divergence: `CombiPro`, `MSBrossAI`, `SERVER-DEV`, and `MSB` routing.
2. Verify ZIP/tooling generators and runtimes: `Sr.Smith`, `Agent-Sr-Smith`, `MY-UNIVERSAL-AI-OS`, `MCP-agent-memory`, `NexusFlow-Framework`, `SKILL-skill-forge`.
3. Validate public apps and backends in deterministic batches, then static/personal web projects.

**Current verified full-project closures: 1/35 (`SKILL-skill-forge`, local contract).** This intentionally excludes scoped green checks and documentation from full-project completion.