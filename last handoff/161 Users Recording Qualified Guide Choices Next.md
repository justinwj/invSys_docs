# Users recording qualified; guide choices next

## 1. Goal and release outcome

Complete4be-A recording/Viewer/How-To and required early B0 under v4.11/Plan022;
stop before broad4be-B. Goal active/incomplete. Users write recording now has a
qualified automated checkpoint; comprehensive Users/guide acceptance remains open.

## 2. Current verified state

Last verified2026-10-12 UTC. Both main branches: code `32a855c5`, docs `c0e73ce`
before this handoff; both pushed. Final docs push includes this handoff.
Controls1.556; catalog version38 with160 definitions. This is a definition count,
not a comprehensive-coverage percentage. Candidate:
`deploy/validation-admin-users-recording-01`, unpromoted.

Excel and runtime/build/test controllers are closed. The owned desktop monitor
ended normally19:05:41-20:01:02UTC:662 samples, zero cursor/desktop/capture/error5
failures. Passive reads alone do not prove mouse movement. Revalidate and restart
monitoring before runtime work. No station deployment or permanent settings change.
Code clean after commit; unrelated docs024 deletion/067 edit/untracked023/024REPORT/
025 remain untouched. Four previously captured user-file hashes match.

## 3. Decisions and constraints

D8-USERS-01 remains approved and governs all Auth writes. D18 semantic inheritance
adds ADMIN_USER_SAVE/DEACTIVATE/DELETE, Admin > Users & Roles, Command class,
ADMIN_USERS_ROLES owner and ADMIN_MAINT capability. Core supplies SAVED only after
confirmed persistence, REJECTED before writing, DENIED for authority refusal and
FAILED for errors. Declined Delete supplies CANCELLED. Only SAVED concludes the
command; no Domain source references/application claim. Required actor ID stays;
target-account/credential payloads do not enter activity. All157 prior definitions
remain unchanged. Inputs and both contexts are captured before optional logging.

D18-LOCAL-01 remains unapproved. A new async approval question was sent this turn
for the existing proposal at v4.11:2096; no reply received before this handoff.
Check for a reply before asking again or changing eligibility. D16-VBA-LOAD-01
also remains unapproved. Do not change the source-loading registry option, local
recording gate, or disabled StationUpdate.

On desktop error5: timestamp, stop runtime, retain owned restoration, handoff/push
and exit. No force-kill, recovery COM attachment, desktop rebinding, rebuild with
Excel open, or edits to test tooling while a controller pins it.

## 4. Evidence and traceability

Canonical receipt: code
`tests/integration/plan022_slice4be_admin_users_recording_results.md`.
Qualified missing-record RED33/37 -> GREEN353/353 retains all70 RED check names
and all259 prior authority checks in order. Actual handlers cover all three saved,
dirty-authority and cancelled-save cases, Reader denial, declined Delete, privacy,
correlated records, honest conclusions and quiet global/action/user suppression.
Core authority, ownership, unknown columns, dates and credentials remain protected.

GREEN controller `auth-read-controller/cc8e0251e2404c11ae92254db2ebc9a9`, worker
`slice4be-auth-read/5a563ca70d0e4724a8a1e0ac35bd4274`, under `reports/runtime/`.
Four reviewed captures retain healthy/invalid Auth, full context refusal and
Settings Save; credential fields are blank. Modeless display/confirmation responses
are test seams. Ordinary modal launch, actual native confirmation/tracking notice,
and existing long-path/account-copy-button clipping remain open.

Build01:five cold compiles/Operations cold start;329 unchanged compiled components,
five intended changed components and new Admin `modAdminUsersAction`. Static02:
342components/6428procedures/140068lines,28 non-growing caps,dynamic9/45,three schemas/
504 parsers. Explicit bounded duplicate exception196 vs195 is the three one-line
native event delegates; prior Core adapter exception remains. See receipt for IDs.

Smoke86,Settings202,Seed114,Console118 and chain32/live-role48/Create15 retain their
prior ordered checks. Normal closures/restoration and delayed audits pass; last
chain audit through20:00:09.5420332UTC is clean. Exact paths/pins are in the receipt
and `admin-users-recording-qualification-01/shared-verification.json`.

## 5. Do Not Repeat

Two preliminary attempts are excluded: BeforeSave fixture initially omitted
EnableEvents=True; subsequent private MsgBox interception failed after probe
insertion. Seven exact generated Delete prompts were declined solely to restore
that controller. The qualified probe explicitly redirects the known confirmation
call to a fixed test response, retaining real handler/Core execution. Do not revive
the ambiguous intrinsic shadow. No intervention occurred in qualified RED/GREEN.
Do not hash candidate files while another stage has them open, or restart controllers
because normal cleanup waits appear. Full chain took5m49 and closed unassisted.

## 6. Assumptions to Re-verify

Desktop access, closed Excel, package pins, absent source-loading option and user
changes. Check pending D18-LOCAL-01 reply. Passing this chain does not resolve or
approve the historical native-loading registry proposal.

## 7. Open questions and blockers

The shared expected-conclusion editor's fixed list omits Users SAVED and Seed
APPLIED. Both outcomes are registered; neither new option has been implemented.
Users context/reentrancy/storage/continuous-recording boundaries, exact publication,
independent saved-guide conclusions, other controls and native/layout acceptance
remain open. Seed still needs its previously documented remaining recording/guide
coverage. No4be-A acceptance, replay expansion or local-recording waiver is claimed.

## 8. Immediate next action

Extend the existing packaged expected-conclusion editor test to require Users
SAVED and Seed APPLIED via the real control-selection handler, and run RED against
the qualified candidate before changing the shared outcome list.

## 9. Critical references

- Current specification/Plan022/Controls pointers and the Users recording receipt.
- `modAuthUserCommands`; `modAdminUsersAction`; `frmCreateDeleteUser.RunUserWriteForm`.
- `Test-Slice4beAuthReadOnly.ps1 -UserRecording` with the full flags in the receipt;
  `-UserRecordingOnly` is the focused diagnostic path, not retained authority proof.
- `Slice4beAdminVerifyGuide.ps1:Test-AdminVerifyExpectationChoices` already opens a
  real saved guide and drives `cboExpectedControl`/`cboExpectedOutcome` in
  `frmActionPathExpectation`. Candidate harness for the next test; not yet extended.
- `Test-Slice4beAdminVerifyAddins.ps1 -ExpectationChoicesOnly` and Core
  `modExpectationDraft.Choices`; existing VERIFIED choice checks must remain.
