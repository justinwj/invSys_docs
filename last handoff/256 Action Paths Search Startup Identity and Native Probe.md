# Handoff 256: Action Paths Search package identity and native probe

Date: 2026-11-20 Pacific. Predecessor: handoff 255.

## Goal and release outcome

Complete 4be-A under Architecture v4.11; D18-SEARCH-INPUT-01 has a prompt small-library NAS retest, with measured and larger-library Search qualification and final acceptance open.

## Current verified state

Last verified 2026-11-20: code worker `C:\Users\Justin\repos\invSys_edit_receipts`, `work/d18-picker-save-repro` at `e4220745`, pushed to draft [code PR17](https://github.com/soetrain/invSys_fork/pull/17); only pre-existing untracked `tests/tooling/reports/` remains. Docs `work/perplexity-handoff218`, draft [docs PR8](https://github.com/soetrain/invSys_docs/pull/8); preserve unrelated guidance 024 deletion, handoff 067 edit and untracked 023/024/025/WSAIFabricSvc files. Excel is open for Justin's candidate review; close it before another build or packaged test. No product source, XLAM, `deploy/current` or NAS file changed.

## Decisions and constraints

Approved D18-SEARCH-INPUT-01 is unchanged. The user-supplied `expert guidance docs/027 Action Paths Search Problem Response.md` is investigative advice, not a new contract. Excel's `OPEN`/`OPEN1` startup entries were temporarily changed from November 16 Admin/Operations copies to the November 20 validation copies with Excel closed; `OPEN2`–`OPEN4` already pointed there. Prior values are in ignored local `reports/runtime/action-search-startup-before-20261120.json` in the worker. Restore those two entries when the review no longer needs the candidate. Do not infer the earlier live package from startup entries alone.

## Evidence and traceability

The former registered Operations XLAM hashes to `8B634BE7…02D348AC`; its manifest names source `45d84ca8`, where `frmActionPaths.mSearch_Change` calls `RefreshPaths` per key. The November 20 candidate hashes to `7A174635…9B3266D` and filters the loaded snapshot locally. This is a strong package-mismatch hypothesis for Justin's slow review; the exact file loaded then was not captured. The old and candidate Admin hashes also differ. See updated report 026.

The hidden packaged reader suite passed **136/136**, including a new no-auto-selected-row assertion, with natural Excel closure. The test-only native keyboard probe is committed behind `-CheckRecordingNativeSearch`; it has **not reached Search**. Three visible-host attempts stopped earlier at `modInventoryViewer.OpenInventoryViewer` with a captured Visual Basic `80010007` automation dialog, including after startup correction. The failed test-only Core insertion attempt was removed before commit. Modal captures and results are ignored under `reports/runtime/slice4be-viewer-published-read/`; no visible run qualifies as behavioral Search RED or GREEN. Cursor movement/restoration succeeded separately, but does not prove Excel automation. In the manual candidate session, live Add-ins reported all five November 20 paths `Installed=True`; on disposable WHT7025AE with one recording, Justin found typing and filtering prompt, Backspace/clear restored the row, and typing after selection cleared evidence and dependent actions without error. This is limited visible evidence, with no measured latency or larger-library qualification.

Symptom -> candidate causes -> rule -> required proof: slow native Search -> older Operations package was registered; visible harness separately fails before Search -> D18-SEARCH-INPUT-01 -> isolate the `80010007` harness failure, measure native Search/Events timing on a larger library, and obtain visible NAS operator confirmation at that scale.

## Do Not Repeat

Do not optimize parsing or bulk ListBox assignment from static suspicion: the reported library showed one recording, the working Viewer also uses per-row AddItem, and the hidden suite leaves no row automatically selected. Do not repeat the current visible-host command without first localizing its `80010007` setup failure. Keep PR17 and PR8 draft; no acceptance claim.

## Assumptions to Re-verify

Recheck Excel startup entries, actual loaded package identity after any Excel restart, console/RDP mode, current Excel build and both PR heads. The prior slow session's actual Operations path was never captured; the current candidate file hashes were recorded before launch, not while locked open.

## Open questions and blockers

Does native Search stay responsive with a larger recording library? Why does the visible automation fixture fail at Viewer open? 4be-A, same-task How-To/Diagnostic/Compare, final B0, full-chain and Release 1 acceptance remain open.

## Immediate next action

With review Excel closed, localize the visible fixture's `80010007` Viewer-open failure before running the staged native keyboard probe against a larger recording library.

## Critical references

Architecture v4.11 D18-SEARCH-INPUT-01; Plan 022; Controls 1.787; report 026; guidance 027; `frmActionPaths.mSearch_Change`, `RefreshPaths`, `ReadSelection`; `Slice4beRecordingReader.ps1`, `Slice4beRecordingSearchNative.ps1`; code PR17; docs PR8.
