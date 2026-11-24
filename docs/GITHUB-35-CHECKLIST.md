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
| 1 | [Agent-Sr-Smith](https://github.com/manu-alvarez/Agent-Sr-Smith) | CANONICAL; portable agent and MCP/RAG consolidated, [PR #2](https://github.com/manu-alvarez/Agent-Sr-Smith/pull/2) merged; CI validated | [Pages deploy successful](https://github.com/manu-alvarez/Agent-Sr-Smith/actions/runs/45289328588) and [main CI green](https://github.com/manu-alvarez/Agent-Sr-Smith/actions/runs/45289328717); real browser ZIP/LLM acceptance pending |
| 2 | [CalendarioMaya-ManoElectricaAzul](https://github.com/manu-alvarez/CalendarioMaya-ManoElectricaAzul) | Expo config/export verified; PR #1 merged | Calendar mathematics and native/browser acceptance |
| 3 | [CombiPro](https://github.com/manu-alvarez/CombiPro) | Source restored, TypeScript/build/audit OK; global pending | Browser/API acceptance, confirm canonical ownership and reconcile duplicate copies |
| 4 | [Conspiracy-Projects](https://github.com/manu-alvarez/Conspiracy-Projects) | Production build reproducible | UI/navigation/browser acceptance |
| 5 | [Dream_OS](https://github.com/manu-alvarez/Dream_OS) | Static asset integrity OK | Offline PWA, storage, import/export and UI acceptance |
| 6 | [Edelweiss-Cumple](https://github.com/manu-alvarez/Edelweiss-Cumple) | 6 HTML asset checks OK; map/RSVP placeholders removed, PR #1 merged | Venue/contact unavailable; user/browser interaction acceptance |
| 7 | [FoZ-SoundPro](https://github.com/manu-alvarez/FoZ-SoundPro) | 6/6 technical tests, archive SHA-256 OK; Pages deployment under re-verification | Manual audio/browser interaction and live site acceptance |
| 8 | [IAPutaOS](https://github.com/manu-alvarez/IAPutaOS) | Current main CI verified (run 23364371028) | API/frontend integrated browser acceptance |
| 9 | [InfoCool](https://github.com/manu-alvarez/InfoCool) | Python/Next.js CI OK, PR #1 merged | Browser workflows and external-service acceptance |
| 10 | [jartos-de-tu-pelo](https://github.com/manu-alvarez/jartos-de-tu-pelo) | Production build reproducible | UI and publication acceptance |
| 11 | [LIVEKIT](https://github.com/manu-alvarez/LIVEKIT) | JWT fallback removed; bounded guest-token issuance (15/IP/5min) merged in [PR #2](https://github.com/manu-alvarez/LIVEKIT/pull/2) and CI passed | Shared edge rate limit on multi-worker deployment; media integration and browser acceptance |
| 12 | [LogiSearch](https://github.com/manu-alvarez/LogiSearch) | Production build reproducible | Search/persistence browser acceptance |
| 13 | [LogiTrack-Warehouse-System](https://github.com/manu-alvarez/LogiTrack-Warehouse-System) | Portable PDF 2-page generation and script syntax CI OK; PR #1 merged | Trello live-board workflow acceptance |
| 14 | [manu-alvarez.github.io](https://github.com/manu-alvarez/manu-alvarez.github.io) | Docs OK; global pending | Live portfolio link checks |
| 15 | [ManuCodearts](https://github.com/manu-alvarez/ManuCodearts) | Docs OK; global pending | Public links/assets checks |
| 16 | [MCP-agent-memory](https://github.com/manu-alvarez/MCP-agent-memory) | SDK compatibility fixed, 164 tests pass, PR #1 merged | Eleven skipped external integration cases and live MCP acceptance |
| 17 | [Mequi3D](https://github.com/manu-alvarez/Mequi3D) | Static asset integrity OK | Interactive 3D viewer/browser acceptance |
| 18 | [MOKO-TOOLS](https://github.com/manu-alvarez/MOKO-TOOLS) | Next.js dependency/build CI verified; PR #1 merged | Tool-catalog accuracy and browser acceptance |
| 19 | [MSB](https://github.com/manu-alvarez/MSB) | Partial | 8 pending app routes and app catalog smoke |
| 20 | [msb-iaputa-backend](https://github.com/manu-alvarez/msb-iaputa-backend) | Current main CI verified (run 23630357694) | API/environment acceptance and frontend contract |
| 21 | [msb-livekit-backend](https://github.com/manu-alvarez/msb-livekit-backend) | JWT secret hardening and bounded guest-token issuance (15/IP/5min) merged in [PR #2](https://github.com/manu-alvarez/msb-livekit-backend/pull/2); CI passed | Shared edge rate limit on multi-worker deployment; real token/provider/browser acceptance |
| 22 | [msb-traductor-backend](https://github.com/manu-alvarez/msb-traductor-backend) | Input contracts and TypeScript build OK; PR #1 merged | Real translation service and error-case acceptance |
| 23 | [MSBross.me](https://github.com/manu-alvarez/MSBross.me) | CI OK; global pending | Functional acceptance and safe FTP rollback |
| 24 | [MSBrossAI](https://github.com/manu-alvarez/MSBrossAI) | CI 13/13 OK; global pending | Source-of-truth matrix, per-app smoke and verified manual deployment |
| 25 | [MY-UNIVERSAL-AI-OS](https://github.com/manu-alvarez/MY-UNIVERSAL-AI-OS) | Main quality and extended-quality CI verified | Runtime/MCP/RAG external acceptance; NO VPS deploy |
| 26 | [NexusFlow-Framework](https://github.com/manu-alvarez/NexusFlow-Framework) | Python tooling and portable PDF generation CI OK; PR #1 merged | Trello integrations and actual operational acceptance |
| 27 | [PromptCombo](https://github.com/manu-alvarez/PromptCombo) | Current main CI and Pages verified (run 41735664235) | Browser UI, artifacts and published page smoke |
| 28 | [SERVER-DEV](https://github.com/manu-alvarez/SERVER-DEV) | Verified SSH host identity required, deployment static CI OK; PR #1 merged | Canonical ownership, backup/rollback and eventual deployment gates (NO VPS yet) |
| 29 | [SKILL-skill-forge](https://github.com/manu-alvarez/SKILL-skill-forge) | COMPLETE: official validation + 12/12 skill + MCP JSON-RPC 8/8 E2E, PR #1 merged | None for documented local generator contract |
| 30 | [Sr.Smith](https://github.com/manu-alvarez/Sr.Smith) | LEGACY private duplicate; advanced modules migrated into Agent-Sr-Smith and README redirected | Physical archive/deletion not available through connected GitHub actions; historical backup retained |
| 31 | [Tarot-Maya](https://github.com/manu-alvarez/Tarot-Maya) | Production build reproducible | Card data and navigation/browser acceptance |
| 32 | [tarot-rws](https://github.com/manu-alvarez/tarot-rws) | Static asset integrity OK | Card content, reading interactions and Tarot-Maya relationship |
| 33 | [TaskFlowPro](https://github.com/manu-alvarez/TaskFlowPro) | CI OK; global pending | Browser CRUD/persistence acceptance and reconcile integrated version |
| 34 | [TuEnergiaMaya](https://github.com/manu-alvarez/TuEnergiaMaya) | Current main validate/deploy CI verified | Calculation correctness and published browser smoke |
| 35 | [varios-external](https://github.com/manu-alvarez/varios-external) | Docs OK; global pending | External references check |


## November 24 verification update

- [x] `SKILL-skill-forge`: complete local generator acceptance E2E. PR https://github.com/manu-alvarez/SKILL-skill-forge/pull/1 ; run https://github.com/manu-alvarez/SKILL-skill-forge/actions/runs/45283136224 ; official Agent Skills checks, skill scaffold, MCP JSON-RPC, adversarial checks.
- [x] `FoZ-SoundPro`: 6/6 technical gates and portable ZIP/sha verified https://github.com/manu-alvarez/FoZ-SoundPro/actions/runs/45283327786 ; official live URL https://manu-alvarez.github.io/FoZ-SoundPro/ provided by owner. Pages deployment after PR #1 failed to find artifact metadata; PR #2 fixes stabilization; new run https://github.com/manu-alvarez/FoZ-SoundPro/actions/runs/45285808445 completed successfully. HTTP availability and browser UX not yet independently verified.
- [x] `InfoCool`: PR https://github.com/manu-alvarez/InfoCool/pull/1 merged; fixed 5 missing frontend dependencies and unsupported Next experimental config; Python tests + Next production build https://github.com/manu-alvarez/InfoCool/actions/runs/45285501885.
- [x] `LIVEKIT` and `msb-livekit-backend`: JWT signing secret no longer defaults to hard-coded value; respective PR #1 merged; token access policy still outstanding.
- [x] `msb-traductor-backend`: PR #1 merged; typed HTTP request validation, deterministic tests + build https://github.com/manu-alvarez/msb-traductor-backend/actions/runs/45282738029.
- [x] `MCP-agent-memory`: PR #1 merged; compatible MCP SDK and bounded rank fallback; https://github.com/manu-alvarez/MCP-agent-memory/actions/runs/45283930173 (164 passed, 11 skipped).
- [x] `MSB`: PR #3 merged; cross-repo build matrix verifies `Conspiracy-Projects`, `LogiSearch`, `Tarot-Maya`, `jartos-de-tu-pelo`: https://github.com/manu-alvarez/MSB/actions/runs/45284907362. Their user/browser functionality remains unverified.

- [x] `Edelweiss-Cumple` PR #1 merged: fixed invalid map/RSVP placeholders and 15 Nov 2026 weekday, six HTML pages checked in https://github.com/manu-alvarez/Edelweiss-Cumple/actions/runs/45286260724. Actual venue/phone not provided, so no fabricated links.
- [x] `MSB` PR #4 merged: static asset matrix for `Edelweiss-Cumple`, `Dream_OS`, `tarot-rws` and `Mequi3D`; all four checks passed after source fix (run https://github.com/manu-alvarez/MSB/actions/runs/45286046206).

- [x] Source-head-matched quality evidence (no needless rerun): `IAPutaOS` https://github.com/manu-alvarez/IAPutaOS/actions/runs/23364371028 ; `msb-iaputa-backend` https://github.com/manu-alvarez/msb-iaputa-backend/actions/runs/23630357694 ; `PromptCombo` https://github.com/manu-alvarez/PromptCombo/actions/runs/41735664235 ; `MY-UNIVERSAL-AI-OS` https://github.com/manu-alvarez/MY-UNIVERSAL-AI-OS/actions/runs/45176055249 ; `TuEnergiaMaya` https://github.com/manu-alvarez/TuEnergiaMaya/actions/runs/37633745083. All checked against their exact current main SHA; external acceptance not inferred.

- [x] `Sr.Smith`: https://github.com/manu-alvarez/Sr.Smith/pull/3 merged; [run 45286666495](https://github.com/manu-alvarez/Sr.Smith/actions/runs/45286666495) web application and agent engine jobs both passed. Compared against `Agent-Sr-Smith`: 445 identical file blobs, 13 differing shared files and separate unique modules; source ownership needs a deliberate decision.
- [x] `NexusFlow-Framework`: https://github.com/manu-alvarez/NexusFlow-Framework/pull/1 merged; [run 45286877862](https://github.com/manu-alvarez/NexusFlow-Framework/actions/runs/45286877862) generated PDF in clean runner, read by pypdf; live Trello changes intentionally not executed.
- [x] `LogiTrack-Warehouse-System`: https://github.com/manu-alvarez/LogiTrack-Warehouse-System/pull/1 merged; [run 45287236066](https://github.com/manu-alvarez/LogiTrack-Warehouse-System/actions/runs/45287236066) generated 2-page PDF on runner, scripts checked without Trello mutation.

- [x] `CalendarioMaya-ManoElectricaAzul`: [PR #1](https://github.com/manu-alvarez/CalendarioMaya-ManoElectricaAzul/pull/1) merged; [Expo CI](https://github.com/manu-alvarez/CalendarioMaya-ManoElectricaAzul/actions/runs/45285530669) succeeds, independent calculation and mobile acceptance pending.
- [x] `MOKO-TOOLS`: [PR #1](https://github.com/manu-alvarez/MOKO-TOOLS/pull/1) merged; [Next.js CI](https://github.com/manu-alvarez/MOKO-TOOLS/actions/runs/45287259661) succeeds, catalog and browser acceptance pending.
- [x] `SERVER-DEV`: [PR #1](https://github.com/manu-alvarez/SERVER-DEV/pull/1) merged; [deployment safety CI](https://github.com/manu-alvarez/SERVER-DEV/actions/runs/45287963319) passed. Manual VPS workflows now reject missing pinned `VPS_SSH_KNOWN_HOSTS`; no SSH or deployment executed. A correctly trusted host key must be supplied independently before any future authorized deploy.

- [x] `LIVEKIT` and `msb-livekit-backend`: guest token abuse mitigation merged on both `main` branches (PR #2 each), HTTP 429 and `Retry-After` added; token policy and route contract tests passed in [LIVEKIT CI](https://github.com/manu-alvarez/LIVEKIT/actions/runs/45293212224) and [backend CI](https://github.com/manu-alvarez/msb-livekit-backend/actions/runs/45293205133). Per-process limits are not a substitute for shared edge rate limiting. Production untouched.
- [x] `manu-alvarez.github.io`: portfolio README reflects official Agent-Sr-Smith and FoZ Pages, documentation links and canonical ownership; commit `c99f0b14d3bb11d60d4007bd17ddcec813f8cad7`.

## Canonical source boundaries under review

- `MSB`: GitHub Pages dashboard and `servicios.json`, not a universal source of every frontend.
- `MSBross.me`: Nominalia PHP gateway, frontend build/deploy pipeline. FTP deploy remains manual and non-atomic; no deployment was executed by the CI closure.
- `MSBrossAI/www`: prior audit found near-identical published web content; compare final files before edits.
- `SERVER-DEV`: infrastructure and deployment configuration; must not assume this repository's copies of frontends are current.
- `CombiPro`: independent repository now contains a passing standalone build sourced from a pinned MSBrossAI revision; both legacy copies still exist and require reconciliation after browser/API acceptance.
- `Agent-Sr-Smith` is the canonical repository publishing GitHub Pages. `Sr.Smith` is a private historical duplicate marked as retired; advanced runtime modules migrated via [Agent-Sr-Smith PR #2](https://github.com/manu-alvarez/Agent-Sr-Smith/pull/2) with [full CI success](https://github.com/manu-alvarez/Agent-Sr-Smith/actions/runs/45289184117). Public Pages and real browser acceptance remain independently gated. The GitHub connector does not expose repository archival/deletion; do not misrepresent physical removal.

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