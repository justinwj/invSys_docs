# Handoff 243: Training warehouse operator review setup

Date: 2026-11-15 Pacific. Predecessor: handoff 242.

## Goal and release outcome

Prepare Justin's hands-on 4be-A How-To/Diagnostic comparison under Architecture v4.11 D18-REPLAY-01 and Plan 022. Candidate and review sheet are ready; permission setup and human review remain open.

## Current verified state

Last verified 2026-11-15: draft code PR16 `work/d14-packaged-chain-coverage` is pushed at `c3f0c9e5d063be3433e1b511ee8a14af1f59ae0a` and its isolated worktree is tracked-clean. Draft docs PR5 branch `work/perplexity-handoff218` contains this handoff, Plan 022 and Controls 1.757; the pre-existing unrelated docs deletion, edit and untracked files remain untouched. Main code checkout retains Justin's unrelated `AGENTS.md` edit. One Excel process titled Book1 is open, started from Explorer; Justin has not identified whether it is the review session. Do not close, load packages into, or automate that instance until its ownership is confirmed.

The ignored `reports/runtime/4be-a-human-review-20261115/` contains a five-XLAM review copy and the sibling inventory template, all hash-matched to the unchanged current validation files. `TrainingHub` is empty. No Training warehouse or operational workbook was created or changed.

## Decisions and constraints

Justin chose **Create new Training warehouse**. D8-CREATE-01 requires a captured, signed-in source warehouse Admin session with `ADMIN_MAINT` before interactive Create; the destination has no Auth store yet. No source sign-in, credential or warehouse target has been supplied. The review sheet uses ordinary Receiving and Admin preference controls, separate guide-source and observed runs, and complete/incomplete comparisons. It records no human acceptance. Executable Run How-To remains separate.

## Evidence and traceability

The five copied XLAM hashes match PR4-BASE-18; the copied template matches the validation source. The candidate review sheet is `tests/integration/plan022_slice4be_operator_review.md` in code PR16. Read-only source inspection: `modWarehouseBootstrap` grants `ADMIN_MAINT` and `RECEIVE_POST` to the new user; `frmCreateDeleteUser` and `modAuthUserCommands` expose a six-choice mask without `ACTION_PATH_MAINT`; guide creation checks that separate capability in Core. Packaged guide tests use an explicit disposable Auth fixture grant. Symptom: new Training Admin cannot author a guide through ordinary UI -> missing user-side grant path -> D18's capability-gated authoring and D8's headless write authority. No behavioral RED/GREEN for a grant correction has begun.

## Do Not Repeat

Do not infer `ACTION_PATH_MAINT` from `ADMIN_MAINT`, edit a live Auth workbook, or count a fixture grant as user-side provisioning acceptance. Do not treat copied XLAMs or the empty hub as a completed warehouse.

## Assumptions to Re-verify

Recheck Excel ownership, candidate hashes, current PR heads and empty Training hub before setup. Confirm a source Admin sign-in before Create. No architecture amendment for the grant path has been approved.

## Open questions and blockers

Justin was asked whether Book1 is his review session and whether an explicitly disclosed grant only in the disposable Training fixture is acceptable for an early preview, with ordinary user-side provisioning still open. Both answers are pending. A Release 1 grant path needs a concrete architecture decision before implementation, then Plan/Controls synchronization and D13 packaged RED/GREEN.

## Immediate next action

After Justin identifies the Excel session and chooses the preview grant path, establish a captured source Admin sign-in and create the new Training warehouse through the packaged Admin Create form; keep guide authoring blocked or clearly fixture-scoped according to that choice.

## Critical references

Architecture v4.11 D8-CREATE-01/D18-REPLAY-01; Plan 022; Controls 1.757; code PR16/docs PR5; `modAdminCreateEntry.OpenFromRibbon`, `modWarehouseBootstrap.BootstrapWarehouseLocal`, `frmCreateDeleteUser`, `modAuthUserCommands`, `modGuideDraftSource`; local review `candidate.json` and operator review sheet.
