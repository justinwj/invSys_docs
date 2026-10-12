# Users & Roles write-authority proposal

## 1. Goal and release outcome

Complete4be-A recording/Viewer/How-To and approved early B0 under v4.11/Plan022;
stop before broad4be-B. Goal active/incomplete. This turn made progress by proving
an independent Admin write-boundary gap that must be resolved before its recording.

## 2. Current verified state

Last verified2026-10-12,16:34UTC. Main branches: code `2f4af16b`, docs `e8185f3`
(before handoff), pushed. Controls1.550; catalog36/156 unchanged. Code clean.
Unrelated docs remain untouched: old024 deletion,067 edit, untracked023/024REPORT/025;
their four file hashes still match the preceding session baseline.

No product source/package change this turn. Current unpromoted candidate remains
`deploy/validation-detail-glyph-01`. Its prior Detail90/Viewer98/smoke86/compiles/
static/visible checkpoint remains scoped as recorded in handoff155 and the glyph
receipt. Directory/native qualification remains open; no new full chain claimed.
Excel/controllers are closed; settings and generated Auth fixtures restored.

Owned desktop monitor stopped normally16:24:49-16:33:41UTC:106 samples, zero cursor,
desktop/capture/error5 failures. Passive checks are not mouse-movement proof.
No actual station registration or periodic task changed.

## 3. Decisions and constraints

**D8-USERS-01 is proposed, not approved**, v4.11 line4991. An explicit approval
question was sent this turn; no reply yet. The proposal moves Create/Update,
Deactivate and Delete into headless Core commands checking captured live session,
exact trusted target and ADMIN_MAINT. It also protects unrelated dirty authority
and separates schema provisioning. This deliberately replaces form-owned writes/
schema ensure; do not implement before approval. Ordinary reads, processor rules
and explicit provisioning stay separate. Plan022/Controls1.550 synchronized.

**D16-VBA-LOAD-01 and D18-LOCAL-01 also remain proposed/unapproved.** Do not adopt
source loading or change local recording gates without approval. View Warehouses
recording is explicitly sequenced after its unresolved qualification.

Desktop Win32 error5: timestamp, stop runtime, preserve cleanup/restoration,
handoff/commit/push and exit. No force-kill, recovery COM attachment, desktop
rebinding, build with Excel open or tooling edits during live pinned controllers.
Preserve all existing identity/binding/authority/custom-column/GREEN invariants.

## 4. Evidence and traceability

Code receipt: `tests/integration/plan022_slice4be_admin_auth_write_diagnostic.md`.
Diagnostic139/139 retains original111 checks in order and adds28 precondition,
baseline/preservation checks. It is **not authorization GREEN**. All12 actual
Save/Deactivate/Delete invocations persist, including nine after sign-out,
Reader switch or switch to another warehouse's Admin. Core denies original-target
ADMIN_MAINT in those nine cases; the form still saves its originally selected Auth.
The three authorized baseline commands also persist, ruling out a dead fixture.

Source: form handlers -> SaveUserAndRolesForm/SetUserStatusForm/DeleteUserForm ->
OpenSelectedAuthWorkbookForm(forWrite=True) -> table edits/wb.Save, without a live
Core gate. D8-A explicitly left write review unresolved, so a new decision is needed.

Five instrumented compiles, normal closure, package/tooling/settings preservation,
original generated Auth restoration and other-warehouse Auth preservation pass.
Delayed Application audit through16:31:46.5417308UTC has zero failures.496 PS files
parse. Observation output contains fixed cases/actions and Boolean facts only.
No credential/account payload, path or raw authorization data is committed.

## 5. Do Not Repeat

Do not count diagnostic fixture/measurement checks as successful authorization.
Do not infer denied writes from Ribbon gating or from Core returning False when
the form never consults it. The form is loaded under verified Admin authority;
actual write handlers are invoked after the context changes. Delete confirmation
is a test prompt seam, not native confirmation proof. No ordinary modal/Ribbon
launch or complete Auth write contract is claimed by this diagnostic.

## 6. Assumptions to Re-verify

Approval replies, desktop, closed Excel, pins, Git state and source-option absence.
No new live-role/full-chain/human acceptance this turn. Existing glyph source/static
evidence remains scoped because runtime source/packages did not change.

## 7. Open questions and blockers

Three architectural proposals await approval: D8-USERS-01, D16-VBA-LOAD-01,
D18-LOCAL-01. Native full-chain qualification, View Warehouses recording and
comprehensive remaining Admin/control coverage keep4be-A incomplete.

## 8. Immediate next action

If D8-USERS-01 is approved, record that approval and first run actual-handler
denial RED for the nine diagnostic cases on unchanged glyph-01 before implementation.

## 9. Critical references

- `Test-Slice4beAuthReadOnly.ps1 -AdminRefresh -AdminWriteDiagnostic`,
  `Slice4beAdminAuthWriteDiagnostic.ps1`, `Slice4beAdminAuthRefresh.ps1`.
- Controller `reports/runtime/auth-read-controller/ed969a94324644e095de4da7072147c7`,
  including `qualified-verification.json`; worker
  `reports/runtime/slice4be-auth-read/1cf426d8c184480a91e6028236bc6264`.
- `frmCreateDeleteUser`, Core `modAuth`, `modAuthSession`, `modNasConnection`.
- Code remaining-acceptance/Admin-coverage indexes; handoff155/glyph receipt for
  rendering and handoff154/directory-columns receipt for native controls, station
  baseline and recovery pitfalls. No earlier failed evidence is relabelled GREEN.
