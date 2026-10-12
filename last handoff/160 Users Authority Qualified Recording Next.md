# Users authority qualified; recording next

## 1. Goal and release outcome

Complete4be-A recording/Viewer/How-To and required early B0 under v4.11/Plan022;
stop before broad4be-B. Goal active/incomplete. Approved D8-USERS-01 now has a
qualified command correction, removing the prerequisite authorization defect.

## 2. Current verified state

Last verified2026-10-12 UTC. Both main branches: code `92bc9f53`, docs `470649a`
before this handoff. Code is pushed; final docs push includes this handoff.
Controls1.555; catalog version37 with157 definitions, unchanged by this correction.
Unpromoted candidate: `deploy/validation-admin-users-authority-01`.
Excel, test/build controllers and the owned desktop monitor are closed. No station
deployment or permanent settings change. Code clean after commit; unrelated docs
024 deletion/067 edit/untracked023/024REPORT/025 remain untouched. Four prior user-file
hashes match. Review status again before new work.

Desktop monitor ended normally18:13:10-19:02:12UTC:587 samples, zero cursor,
desktop/capture/error5 failures. Passive reads alone do not prove mouse movement.

## 3. Decisions and constraints

D8-USERS-01 was explicitly approved2026-10-12. Core `modAuthUserCommands` owns
SaveUser, DeactivateUser and DeleteUser. The form captures context on opening;
Core rechecks live session generation, exact trusted warehouse/station/Auth and
fresh ADMIN_MAINT before mutation. Typed primitive APIs; no normal-write schema
repair, unrelated dirty save, borrowed close or false persistence/rollback claim.
Reads, explicit provisioning and headless processor authority are preserved.

D16-VBA-LOAD-01 and D18-LOCAL-01 remain proposed/unapproved. Do not change the
source-loading registry setting, local recording gate or disabled StationUpdate.
No Users recording ID has been added. D18 mapping/recording remains next.

On desktop error5: timestamp, stop runtime, retain owned restoration, handoff/push
and exit. No force-kill, recovery COM attachment, desktop rebinding, rebuild with
Excel open, or edits to test tooling while a controller pins it.

## 4. Evidence and traceability

Canonical receipt: code
`tests/integration/plan022_slice4be_admin_auth_write_diagnostic.md`.
Real-handler RED139/9 -> GREEN148 -> Core250 -> final visible/data259 retains each
earlier ordered check set. Nine unauthorized form writes stop; authorized writes
persist. Direct Core protects stale sessions/grants, wrong paths, missing/invalid/
read-only/dirty authority, ownership and no repair. Delete confirmation-time sign-out
is denied. Real BeforeSave cancellation reports failure and preserves disk bytes;
borrowed memory remains dirty. Custom columns, dates, existing credentials and
fresh saved new-user capability scope pass.

Final controller `auth-read-controller/d83395dd10694cb294d92b31c2ad08c9`, worker
`slice4be-auth-read/010a2b2a9b7b43a8bd9271943d792240`, under `reports/runtime/`.
Four reviewed captures show the complete refusal and retained read/Settings flows.
Modeless presentation is a test seam; ordinary modal launch and existing long-path/
account-copy-button clipping remain open. Delayed audit through18:54:35.3119085UTC
is clean; compiles, settings/package/tooling/fixture restoration and closure pass.

Build `admin-users-authority-build-01`: five cold compiles/Operations cold start;
331 unchanged components. Only new Core owner and changed Admin form affect behavior.
Seed observer differs solely by two previously documented trailing newlines.
Static02:341 components/6427 procedures/139981 lines,28 non-growing caps, dynamic9/45,
three schemas/503 parsers. Reviewed duplicate exception195 versus194 is solely the
two distinct one-line Deactivate/Delete adapters; Execute is the shared owner.

Smoke86 and chain32/live-role48/Create15 retain prior ordered checks. Chain controller
`admin-users-authority-regression/chain-1b9bb6b512f54beab17ffd847af178d1` confirms
restoration and delayed audit through19:01:29.4473393UTC. Inter-stage waits complete
unassisted; no intervention in the qualifying chain. Exact smoke/build/static paths
and checks are in the canonical receipt. No4be-A acceptance or promotion is claimed.

## 5. Do Not Repeat

Expanded test instrumentation initially failed before behavior: a late-added form
member was not recognized, a case-sensitive status anchor failed after VBE recasing,
and a generated Sub had the wrong terminator. Existing ShowStatusForm observation,
a case-insensitive anchor and corrected probe compile cleanly. These were harness
failures, not product RED. The compile helper now records only module/line metadata.
Owned compile dialogs were dismissed only in those failed runs; final gates were
unassisted. Do not rerun old verifiers expecting later tooling to retain old hashes.

## 6. Assumptions to Re-verify

Desktop access, closed Excel, candidate pins, absent source-loading option and user
changes. This passing chain does not settle the earlier intermittent native loading
diagnostic or approve its proposed registry change.

## 7. Open questions and blockers

Users recording/guide coverage and form clipping; remaining Admin controls and
broader4be-A acceptance. Seed observation114 remains the prior qualified checkpoint;
context/storage/continuous recording, exact Viewer publication and independent saved
guide conclusions remain open. D16-VBA-LOAD-01/D18-LOCAL-01 remain unresolved.
No active runtime blocker or acceptance waiver is declared.

## 8. Immediate next action

Map the existing Users & Roles controls under D18 and add/run actual-handler
recording RED against the qualified Core commands before implementing observations.

## 9. Critical references

- Current specification/Plan022/Controls pointers and remaining-acceptance index.
- Auth-write receipt above; Seed recording receipt referenced by handoff159.
- `src/Core/Modules/modAuthUserCommands.bas`; `frmCreateDeleteUser` Initialize,
  SaveUserAndRolesForm, SetUserStatusForm, DeleteUserForm.
- `Test-Slice4beAuthReadOnly.ps1 -Phase GREEN -AdminRefresh -AdminWriteDiagnostic
  -RequireWriteAuthority -CoreAuthority -CaptureEvidence` with the candidate above.
- `Slice4beAdminAuthWriteDiagnostic.ps1`, `Slice4beAdminUsersAuthority.ps1`,
  `Slice4beAdminAuthRefresh.ps1`, `Slice4beEvaluationNativeTrace.ps1`.
