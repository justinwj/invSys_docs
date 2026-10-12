# Local recording decision pending

## 1. Goal and release outcome

Complete4be-A recording/Viewer/How-To and approved early B0 under v4.11/Plan022,
then stop before broader4be-B. Goal remains active/incomplete. This checkpoint
proves the local recording gap and requests a specific architecture decision.

## 2. Current verified state

Last verified2026-10-12. Main pushed: code `b36f412e`, docs `40dd338` before this
handoff. Code clean; unrelated docs remain unchanged: old024 deletion,067 edit,
023/024REPORT/025 untracked. Four hashes were rechecked. Controls1.543;
catalog34/154. No product source/package changes. Unpromoted candidate remains
`deploy/validation-admin-reconcile-recording-06`, with five compiled pins in
`reports/runtime/admin-reconcile-recording-build-06/compiled-pins.json`.
Excel/controllers/static workers/owned monitor are closed. Monitor10:12:27–
10:20:23 UTC:95 samples, zero cursor/desktop/capture/error5 failures. This does
not prove mouse movement. Restart monitor and verify pins before runtime work.

## 3. Decisions and constraints

**D18-LOCAL-01 is proposed, not approved.** Async approval request sent this turn;
no answer received as of this handoff. v4.11 line2062 is the authoritative text,
synchronized to Plan022/Controls1.543. Proposal: optional recording and libraries
use any valid captured signed-in warehouse's own existing runtime, local or UNC,
including a valid local fallback context. Never redirect an unavailable NAS
library to a different local root. Business/replay eligibility and all rights,
policy, binding, integrity and immutable-evidence rules remain independent.
Do not implement before approval. All earlier approvals/invariants remain.
On desktop Win32error5: timestamp, stop runtime, owned cleanup, handoff/commit/push
and exit. VBA Err5 differs. Serial Excel jobs; no force-kill/recovery COM attach,
desktop rebinding or edits to pinned scripts during a controller run.

## 4. Evidence and traceability

Code receipt: `tests/integration/plan022_slice4be_admin_reconcile_results.md`, final
section. **199/199 diagnostic PASS**, exact172 prior checks; not behavioral RED
or acceptance of a recording exclusion. Controller:
`reports/runtime/admin-reconcile-controller/6e96e1190da74e1e92d6e42583b219c3`.
Worker: `reports/runtime/slice4be-admin-reconcile/f6fd0eb4df7a4cc2b076ddda01919019`.
UTC10:13:37.1084819–10:15:32.7776022; no native failures through10:15:44.7776022.
Five instrumented compiles, exact log/JSON, normal closure/preservation pass.
Ignored `local-recording-diagnostic.json` and controller
`local-diagnostic-verification.json` contain sanitized facts only.

NAS fixture: enabled policy, one queued correction, two activity files.
Explicit local: actual resolver yields WH_SOURCE_LOCAL; live sign-in/policy and
one exact queued correction pass, but context/activity/journal unavailable,
zero activity files and zero warning. Modeled fallback has the same result.
Inventory/custom values, prior training files and saved policy are preserved.
Three shared NAS-only guards explain the gap; D18 comprehensive coverage requires
an explicit decision, then packaged local-recording RED/GREEN. Diagnostic uses
actual callback/Inspect handler with deterministic presentation; no native claim.

Static `admin-reconcile-local-diagnostic-static-01`:332/6399/139542,28 unchanged
caps, dynamic9/45,duplicates194,three schemas,482 parsers pass. No new exception.
Reuse unchanged-package360 guide proof (handoff148), cold compiles,86 smoke,
202 Settings,32 chain/48 live-role/15 Create Warehouse receipts.

## 5. Do Not Repeat

WH_SOURCE_NAS=0, REMEMBERED=1, LOCAL=2, FALLBACK=3. The explicit local diagnostic
uses ClearWarehouseTarget + root override + ResolveWarehouseTarget, then live
sign-in; ordinary test SelectTarget substitutes a UNC HubRoot and cannot prove
local behavior. Fallback source-type injection is not full fallback discovery.
Do not patch only CaptureContext and leave activity/journal stores inconsistent.
Do not count199 as replacement for360. Prior native-crash caveats remain in the
receipt/handoff146; a clean rerun is not a repair.

## 6. Assumptions to Re-verify

Check for a new approval reply before proceeding. Candidate remains unpromoted.
Do not commit raw runtime reports/screenshots. The local diagnostic takes about
two minutes; full360 guide gate takes about28 minutes.

## 7. Open questions and blockers

D18-LOCAL-01 approval is pending; no desktop blocker. Other Admin coverage remains
open. Independent source audit of Verify Add-ins Published is appended to
`plan022_slice4be_admin_remaining_coverage.md`: its service checks only presence/
nonzero size of five files, while the callback first prepares/formats workbook
surfaces. Do not claim hash/deployment verification or an entirely read-only
callback. Existing service tests do not establish recording/authorization.

## 8. Immediate next action

After D18-LOCAL-01 approval, add and run a packaged local recording/journal RED before changing the three shared gates; while approval is pending, the next independent coverage target is the actual Verify Add-ins Published callback identified in the source audit.

## 9. Critical references

- v4.11 D18-LOCAL-01, D18 Reconcile/evaluation, D14-RECON-01/D8-RECON-01;
  Plan022 and Controls1.543.
- `Test-Slice4beAdminReconcileIdentity.ps1 -DeployRoot deploy/validation-admin-reconcile-recording-06 -Phase GREEN -LocalRecordingDiagnostic`.
- `Slice4beAdminReconcileLocalDiagnostic.ps1`, source gates
  `modActivity.CaptureContext`, `modActivityStore.StoreRoot`,
  `modRecordingJournal.JournalRoot`.
- Separate replay gate `modExecutionTarget.Read` remains NAS-restricted; this
  proposal does not change it or Operations business-target permissions.
