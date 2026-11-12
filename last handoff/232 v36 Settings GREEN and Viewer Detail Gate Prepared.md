# Handoff 232: v36 Settings GREEN and Event Viewer detail gate prepared

Date: 2026-11-12 Pacific. Predecessor: handoff 231.

## Goal and release outcome

Complete Release 1 Slice 4be-A under Architecture v4.11 D18 and Plan 022. Settings now has current-package GREEN; Event Viewer detail and broader acceptance remain open.

## Current verified state

Last verified 2026-11-12: code `main` is `6d247543` with Justin's unrelated `AGENTS.md` change untouched. Draft code PR14 is clean at `b8f94241`. Execution worker `C:\Users\Justin\repos\invSys_edit_receipts` is clean and detached at `b8f94241` for the prepared v37 check; restore `work/d8-inv-edit-receipts` (`550d9ff0`) after the run or if abandoned. Docs PR5 branch `work/perplexity-handoff218` has Plan 022 and Controls **1.744**. Other user docs changes remain untouched. Excel is closed. The owner's shift ends **21:08 UTC**.

## Decisions and constraints

- The five validation XLAMs and product contracts are unchanged. v36's one-run approval is consumed. v35 never dispatched because its fixed cutoff passed before approval.
- A new v37 Event Viewer detail run requires its own approval. The first approval question incorrectly translated **20:45 UTC** as 1:45 PM Pacific. A corrected question states **12:45 PM Pacific**; only an answer to that corrected question authorizes dispatch. No retry, assisted Excel close, process kill or input rebinding.
- The `soetrain` docs branch `work/perplexity-handoff218` points to an older PR6 tree. Docs PR5's current head is the `justinwj` fork branch. Do not merge the older branch into the current docs work.

## Evidence and traceability

- v36 PR4-BASE-10 visible packaged Settings/policy/detail/preference: **202/202 exact PASS**, worker exit 0, controller `StopReason=null`, restart proof and both Excel native exits verified, no extra Excel, settings restored, 539 pins preserved, no process termination, no modal intervention, delayed audit zero Excel faults. Run 6.49 minutes on Excel 16.0.20527.20196. The negative stdout-quiet-to-first-Excel-exit metric is inapplicable because the first Excel exits before later checks. Evidence: `reports/runtime/settings-policy-v36-pr4-base-10-20261112`.
- v37 Event Viewer detail controller is test-only in ignored runtime; its 90 exact identities derive from the 2026-10-12 passing visual run on an older candidate. It exercises packaged selected detail, multiline/long text, native cursor scroll/typing and screenshots on the current five XLAMs. Manifest `68338D11...`, expected `A29D43C0...`, launcher `DFA7A2E7...`; parser zero errors, checks-only passed 539 pins / 90 identities without Excel. Exact hashes, scope and command: `reports/runtime/viewer-detail-v37-pr4-base-10-20261112/codex-viewer-detail-v37.md`. No v37 dispatch or authorization file exists.
- Plan 022 and Controls 1.744 are committed and pushed on docs PR5's fork head. v36 is standalone Settings evidence, not 4be-A or Release 1 acceptance.

## Do Not Repeat

Do not rerun v32-v36, dispatch expired v35, treat v34's controller failure as product RED, or use the erroneous 1:45 PM translation. Do not merge the older `soetrain` docs working branch.

## Assumptions to Re-verify

Recheck corrected v37 approval, cutoff, clean detached worker, no Excel, desktop/cursor readiness, five XLAM hashes, 539 pins, launcher hash and no dispatch before the run.

## Open questions and blockers

v37 current-package Event Detail evidence; Viewer published reads/groups/refresh, guide transfer, other Admin/Operations, retained formatting, broad Inventory, human Receiving B0, live role, full chain and visible operator acceptance. Execute slowdown and Microsoft-reported Excel exit defect remain separate.

## Immediate next action

If the corrected approval arrives before **20:45 UTC**, rerun v37 checks-only and dispatch one hands-off visible Event Detail run; otherwise leave runtime paused and restore the worker branch.

## Critical references

Architecture v4.11 D18 and Event Detail scrolling decision; Plan 022 PR4-BASE-10 checkpoint; Controls 1.744; code PR14; docs PR5; `tests/tooling/Slice4beViewerEventDetail.ps1`; v36/v37 folders above.
