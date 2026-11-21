# Action Paths Search: native performance failure after packaged GREEN

Date: 2026-11-20 Pacific. Status: **open 4be-A usability blocker**. This is a diagnostic request, not a proposed contract change.

## Operator observation

On the disposable NAS review warehouse, **Action Paths > Search recordings** remains extremely slow to type into after the D18-SEARCH-INPUT-01 change. Justin reports that **Viewer > Events > Search** is fast and that the previously built picker is also responsive. No per-character timing, Excel CPU trace, or exact loaded-add-in inventory was captured during this observation. Do not label the final build visibly accepted.

## Contract and candidate

Architecture v4.11, approved **D18-SEARCH-INPUT-01**, requires immediate local filtering of recording headers loaded by authorized Open/Refresh. Each edit checks captured session/warehouse and clears selected evidence/actions, but makes no per-key Config or NAS journal read. Selection and Refresh recheck current policy. Plan 022 and Controls 1.785 recorded packaged GREEN with visible NAS usability still pending; this operator result makes that visible gate **RED**.

Code commit `aa44b245` is on draft [code PR17](https://github.com/soetrain/invSys_fork/pull/17). The isolated validation folder is `C:\Users\Justin\repos\invSys_edit_receipts\deploy\validation-action-search-final-20261120\`. Its `invSys.Operations.xlam` SHA-256 is `7A174635017618DDCC54B6F03D831780FA16B3F9D117F05E27962D97C9B3266D`; `deploy/current` has a different Operations hash, `882DABBDFF327C1B280CD4D13428577969B89ECBC576AE89C6263FC117ABB9C8`. **The exact Operations XLAM loaded in Justin's slow session has not been independently verified.**

## What the existing evidence proves

- Prior-package actual-handler RED: **123 PASS / 4 behavioral FAIL**. The old `mSearch_Change` called Core `ListPaths` on each edit, validating policy and rereading journal headers.
- New isolated candidate: **130/130 packaged GREEN**, five explicit XLAM compiles, cold-start reference check, layout and integrity regressions, natural Excel exit. The test sets `txtPathSearch.Value` through the packaged form adapter and exercises its real `Change` handler. It verifies no per-key policy read and that filtering still works when the disposable journal files are temporarily absent. Evidence: ignored local `reports/runtime/slice4be-viewer-published-read/f3256936b0ec44b9a7e4bfe935c61bf2/` in the worker.
- These checks **do not measure native keyboard delivery, focus, repaint, RDP effects, or key-to-visible-result latency**. They do not establish that the operator loaded the new package. Static maintenance did not show dynamic-call growth: 391 components, 6762 procedures, 9 literal/45 unresolved dynamic calls, 193 duplicate-body groups.

## Source path to examine

In `src/Operations/Forms/frmActionPaths.frm`, `mSearch_Change` (near line 276) calls `ContextValid`, `ClearSelectedRecording`, then `FilterLoadedPaths`. `FilterLoadedPaths` (near line 132) clears the MSForms ListBox and repopulates matching rows from `mLoadedRows` on each edit. `mPaths_Change` is suppressed while `mLoading` is true. `ClearSelectedRecording` can close dependent forms and clear selected evidence on the first edit after a selection. `modActivity.CaptureContext` uses the in-memory sign-in/target state and path-string comparison; the inspected path has no direct Config or journal read. A hidden or indirect cost has **not** been ruled out by native timing.

Comparators in the same Operations XLAM: `frmInventoryViewer.mTxtSearch_Change` calls local `RenderRows` and is reported fast. `frmGuideActionPicker.mSearch_Change` calls `RefreshChoices` and is also reported fast. Their existence argues against assuming that all MSForms list rebuilding, Core calls, or NAS use is intrinsically slow. No causal conclusion follows without timings in the same operator session.

## Questions for expert review

1. Confirm the five loaded XLAM full paths and hashes inside the slow Excel session. Is `invSys.Operations.xlam` the isolated `7A174635…` candidate, with no older registered copy supplying `frmActionPaths`?
2. Measure one native keypress from input delivery to visible list update, and separately time `ContextValid`, `ClearSelectedRecording`, `FilterLoadedPaths` (including ListBox Clear/AddItem and repaint), and any event reentry. Compare first key after a selection with later keys. Capture counts and timings only; do not log typed text or operational rows.
3. Repeat comparable keypresses in Action Paths Search, Viewer Events Search, and the working picker under the same Excel/session/display state. Record loaded row counts and whether RDP or console is active.
4. Identify the first measured slow boundary, then propose a **focused native-keyboard RED** through the packaged form and a correction that preserves D18-SEARCH-INPUT-01's session, policy, evidence-clearing and Refresh rules. Re-run native NAS usability and retained packaged regressions before accepting a fix.

Do not infer a new search contract or promote `deploy/current` from the 130/130 packaged result. The underlying slow boundary is unresolved.

## 2026-11-20 startup-registration follow-up

Read-only inspection found Excel startup slots `OPEN` and `OPEN1` pointing to the November 16 review copies of Admin and Operations, while `OPEN2`–`OPEN4` pointed to the November 20 Core and Domain candidate. The registered Operations file hashes to `8B634BE75820C186A8A42EF434CDCFC681BC8857086A56A3DE424ECC02D348AC`; its local candidate manifest names source commit `45d84ca8`. At that commit, `frmActionPaths.mSearch_Change` calls `RefreshPaths` on each edit, which calls Core `ListPaths`. The registered November 20 Operations file instead hashes to `7A174635017618DDCC54B6F03D831780FA16B3F9D117F05E27962D97C9B3266D` and filters the loaded snapshot locally. This is a concrete, plausible explanation for the slow review, **not proof of the exact workbook loaded in Justin's earlier Excel session**.

With Excel closed, the two old startup entries were saved to ignored local `reports/runtime/action-search-startup-before-20261120.json` in the worker and temporarily changed to the November 20 candidate paths. All five startup slots now name that same candidate folder. `deploy/current`, the NAS and package files were untouched. The next manual Excel session must verify the actual five loaded workbook paths/hashes before a native Search conclusion. Restore the saved entries when the review no longer needs the candidate.

A new test-only assertion that programmatic Search leaves no row selected passed in the existing hidden-host reader suite: **136/136**, natural Excel closure. It rules out automatic selection in that fixture. A separate native-keyboard probe is staged behind an explicit test switch but has **not reached Search**. Three visible-host attempts stopped in `modInventoryViewer.OpenInventoryViewer` before the probe with a captured Visual Basic `80010007` automation dialog; one attempt also stopped earlier on a test-only probe insertion error that was removed. The visible failures persisted after the startup entries were corrected. Their cause is unconfirmed and they are not behavioral Search RED. No product source was changed.
