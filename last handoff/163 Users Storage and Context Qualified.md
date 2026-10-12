# Users storage and context qualified

## 1. Goal and release outcome

Complete4be-A recording/Viewer/How-To and required early B0 under v4.11/Plan022;
stop before broad4be-B. Goal active/incomplete. Users storage failures and
context changes at recording entry now have qualified packaged evidence.

## 2. Current verified state

Last verified2026-10-12 UTC. Both main: code `51fcb16c` pushed; docs `d14164b`
before this handoff. Final docs push includes it. Storage checkpoint was separately
pushed as code `a8563620` / docs `7fe4420`. Controls1.559; catalog38/160 unchanged.
Current unpromoted candidate: `deploy/validation-admin-users-context-01`.

Excel/build/test controllers are closed. Owned desktop monitor ended normally
20:17:06-21:10:55UTC:644 samples, zero cursor/desktop/capture/error5 failures.
Passive reads do not prove mouse movement. Restart monitoring before runtime work.
Code clean; unrelated docs024 deletion/067 edit/untracked023/024REPORT/025 remain
untouched. Four user-file hashes still match handoff161. No station deployment.

## 3. Decisions and constraints

D8-USERS-01 remains approved. D18 already requires one fixed tracking notice on
context/storage failure without blocking/repeating business work or inventing
records. No new contract: `modAdminUsersAction.BeginObservation` now reads live
context after its optional call. Only that statement order changed in production.
SAVED/APPLIED editor choices remain qualified; choosing an expectation is not proof.

D18-LOCAL-01 and D16-VBA-LOAD-01 remain unapproved. The existing async local-recording
question has no reply; check before asking again. Do not change local eligibility,
source-loading registry or disabled StationUpdate. On desktop error5: timestamp,
stop runtime, preserve restoration, handoff/push and exit. No force-kill, recovery
COM attachment, desktop rebinding, rebuild with Excel open or pinned test-tool edits.

## 4. Evidence and traceability

Canonical code receipts under `tests/integration/`:
`plan022_slice4be_admin_users_storage_results.md` and
`plan022_slice4be_admin_users_context_results.md`.

Storage GREEN420 retains353 prior checks. Six real attempt/outcome file-Open
failures leave one persisted business write, one fixed notice and honest partial
records; fresh read-only Auth results, privacy and preservation pass. No product fix.
Context RED254/3 isolates missing notices after sign-out for all three commands;
Core refusal/authority/attribution already pass. Corrected GREEN493 retains all420
prior and257 RED checks in order, including nine context changes and six failures.

GREEN controller `reports/runtime/auth-read-controller/87af6ea5187149d8a20cd3a9c12dc0f8`;
worker `slice4be-auth-read/59c39d36b2234456993871d51027953d`. Five instrumented compiles,
four reviewed captures, preservation/normal closure and audit through21:04:23UTC pass.
Captures retain readable healthy/invalid Auth, full context refusal and Settings
Save with blank credentials. Native warning/confirmation acceptance and existing
long-path/account-copy-button clipping remain open.

Build `admin-users-context-build-01`: five cold compiles/Operations cold start,
334 unchanged compiled components; only Admin/modAdminUsersAction changed.
Static `admin-users-context-static-01`:342/6428/140068;28 caps, dynamic9/45 and196
duplicates unchanged;506 parsers/three schemas pass. Fresh chain32/live-role48/
Create15 retains prior ordered checks and closes unassisted, with preservation and
clean audit through21:10:37UTC. Controller `admin-users-context-regression/chain-b8a65ba3c8a24f879238c10db58322fc`.

## 5. Do Not Repeat

Initial storage probe failed before tests because of statement matching; excluded
from RED. Use exact trimmed, case-insensitive compiled statement matching. Existing
explicit confirmation/notice seams remain; do not revive intrinsic MsgBox shadowing.
Keep controllers through normal closure: full493 took17m29; chain5m51 with three
normal cleanup waits. Do not hash packages while Excel holds them open.
Grant/verify ACTION_PATH_MAINT explicitly in guide fixtures; earlier Verify guide
work failed without it. Inspect offered outcomes before assigning dropdown values.

## 6. Assumptions to Re-verify

Desktop access, closed Excel, candidate pins, user changes and pending approval
replies. Handler/visible evidence is not ordinary native warning acceptance.

## 7. Open questions and blockers

Continuous Users recordings, exact publication and independent saved-guide
conclusions remain open, as do other context/reentrancy boundaries, other controls
and native/layout acceptance. Seed has remaining recording/guide work. Broader4be-A
requirements and early B0 must still withstand the final completion audit.

## 8. Immediate next action

Extend packaged Users tests to record a continuous Save/Deactivate/Delete sequence,
publish exact observations and prove a separately authored SAVED guide conclusion
against an independent recording before changing implementation.

## 9. Critical references

- Current v4.11/Plan022/Controls pointers and the two receipts above.
- `Slice4beAdminUsersRecording.ps1`, `...Storage.ps1`, `...Context.ps1`;
  full `Test-Slice4beAuthReadOnly.ps1 -AdminRefresh -AdminWriteDiagnostic
  -RequireWriteAuthority -CoreAuthority -UserRecording -CaptureEvidence -Phase GREEN`.
  `-UserRecordingOnly` is focused mode, not the retained full authority gate.
- `modAdminUsersAction.BeginObservation`; `frmCreateDeleteUser.RunUserWriteForm`;
  `modAuthUserCommands`; existing Verify/GeneralSettings guide helpers.
