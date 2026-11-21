# Handoff 256: Action Paths Search package identity and native probe

Date: 2026-11-20 Pacific. Predecessor: handoff 255.

## Goal and release outcome

Complete 4be-A under Architecture v4.11; D18-SEARCH-INPUT-01 still needs responsive native Search on the disposable NAS warehouse and final acceptance.

## Current verified state

Last verified 2026-11-20: code worker `C:\Users\Justin\repos\invSys_edit_receipts`, `work/d18-picker-save-repro` at `e4220745`, pushed to draft [code PR17](https://github.com/soetrain/invSys_fork/pull/17); only pre-existing untracked `tests/tooling/reports/` remains. Docs `work/perplexity-handoff218` at `9d604fb` before this handoff, draft [docs PR8](https://github.com/soetrain/invSys_docs/pull/8); preserve unrelated guidance 024 deletion, handoff 067 edit and untracked 023/024/025/WSAIFabricSvc files. Excel count was zero at the last check. No product source, XLAM, `deploy/current` or NAS file changed.

## Decisions and constraints

Approved D18-SEARCH-INPUT-01 is unchanged. The user-supplied `expert guidance docs/027 Action Paths Search Problem Response.md` is investigative advice, not a new contract. Excel's `OPEN`/`OPEN1` startup entries were temporarily changed from November 16 Admin/Operations copies to the November 20 validation copies with Excel closed; `OPEN2`–`OPEN4` already pointed there. Prior values are in ignored local `reports/runtime/action-search-startup-before-20261120.json` in the worker. Restore those two entries when the review no longer needs the candidate. Do not infer the earlier live package from startup entries alone.

## Evidence and traceability

The former registered Operations XLAM hashes to `8B634BE7…02D348AC`; its manifest names source `45d84ca8`, where `frmActionPaths.mSearch_Change` calls `RefreshPaths` per key. The November 20 candidate hashes to `7A174635…9B3266D` and filters the loaded snapshot locally. This is a strong package-mismatch hypothesis for Justin's slow review, pending actual loaded-workbook verification. The old and candidate Admin hashes also differ. See updated report 026.

The hidden packaged reader suite passed **136/136**, including a new no-auto-selected-row assertion, with natural Excel closure. The test-only native keyboard probe is committed behind `-CheckRecordingNativeSearch`; it has **not reached Search**. Three visible-host attempts stopped earlier at `modInventoryViewer.OpenInventoryViewer` with a captured Visual Basic `80010007` automation dialog, including after startup correction. The failed test-only Core insertion attempt was removed before commit. Modal captures and results are ignored under `reports/runtime/slice4be-viewer-published-read/`; no visible run qualifies as behavioral Search RED or GREEN. Cursor movement/restoration succeeded separately, but does not prove Excel automation. Justin corrected his earlier “not today” response and said he can retest; the exact candidate-session readiness reply is pending.

Symptom -> candidate causes -> rule -> required proof: slow native Search -> older Operations package is registered; visible harness separately fails before Search -> D18-SEARCH-INPUT-01 -> verify loaded five paths/hashes, then same-session native Search/Events timing and selection safety, followed by visible NAS operator confirmation.

## Do Not Repeat

Do not optimize parsing or bulk ListBox assignment from static suspicion: the reported library showed one recording, the working Viewer also uses per-row AddItem, and the hidden suite leaves no row automatically selected. Do not repeat the current visible-host command without first localizing its `80010007` setup failure. Keep PR17 and PR8 draft; no acceptance claim.

## Assumptions to Re-verify

Recheck Excel startup entries and actual loaded `Workbook.FullName`/hashes, console/RDP mode, current Excel build and both PR heads. The prior slow session's actual Operations path was never captured.

## Open questions and blockers

Does native Search become responsive with all five candidate XLAMs actually loaded? Why does the visible automation fixture fail at Viewer open? 4be-A, same-task How-To/Diagnostic/Compare, final B0, full-chain and Release 1 acceptance remain open.

## Immediate next action

Open one manual Excel session using the five registered November 20 candidate XLAMs, verify their actual loaded paths and hashes, then compare native Action Paths Search with Events Search in disposable WHT7025AE.

## Critical references

Architecture v4.11 D18-SEARCH-INPUT-01; Plan 022; Controls 1.786; report 026; guidance 027; `frmActionPaths.mSearch_Change`, `RefreshPaths`, `ReadSelection`; `Slice4beRecordingReader.ps1`, `Slice4beRecordingSearchNative.ps1`; code PR17; docs PR8.
