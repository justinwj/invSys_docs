# Reconcile recording and binding GREEN

## 1. Goal and release outcome

Complete4be-A recording/Viewer/How-To plus approved early B0 under v4.11/Plan022,
then stop before broader4be-B. Goal remains active and incomplete. This checkpoint
adds the first Reconcile recording gate; it does not finish that family's coverage.

## 2. Current verified state

Last verified2026-10-12. Both main pushed: code `543a7305`, docs `fecbd0d` before
this handoff. Code clean. Candidate `deploy/validation-admin-reconcile-recording-06`
is unpromoted; five pins: `reports/runtime/admin-reconcile-recording-build-06/compiled-pins.json`.
Controls1.540, catalog34/154. Excel, controllers and desktop monitor are closed.
Monitor06:58:30--08:03:41 UTC:780 samples, zero cursor/desktop/capture/error5 failures.
Reads/captures do not establish mouse movement; native keyboard tests are separate.
Restart the monitor and verify closed Excel/pins before runtime work.

Preserved unrelated docs: modified067; deleted old024 Delivery Overrun; untracked
023 Critique,024 REPORT and025 GUIDANCE. Their four hashes/deletion remain unchanged.

## 3. Decisions and constraints

All prior approvals/invariants remain; none pending in this checkpoint. D18 now
maps ADMIN_RECONCILE_OPEN/INSPECT/CANCEL to actual handlers. Native narrative
responses belong to Inspect. Only actual Open/OPENED and Inspect/CONFIRMED establish
CommandCompleted. CONFIRMED references exactly the new Inventory/Submitted event;
FAILED permits at most one Unknown reference. Neither proves Domain application.
Capture business target/user/context before optional logging. Changed sessions
must refuse under D8-RECON-01; tracking never grants authority or repeats commands.

On desktop Win32error5: timestamp, stop runtime, owned cleanup, handoff/commit/push
and exit. VBA Err5 is distinct. Serial Excel jobs; no force-kill/recovery COM
attachment/desktop rebinding. Keep controllers alive through restoration and never
edit their pinned tests. Preserve exact System_Key, unknown columns and prior GREEN.

## 4. Evidence and traceability

Code receipt: `tests/integration/plan022_slice4be_admin_reconcile_results.md`, final
section. Absent-record207/11 RED and warning/reference REDs precede implementation.
Corrected entry-binding246/2 RED on recording-05 becomes **248/248 GREEN** on06,
retaining203 prior native/identity/authority checks and151 catalog definitions.
Actual native callbacks generate20 correctly correlated records. Global/action/user
suppression preserves one business execution. Session changes cannot rebind actions.

Final controller under runtime: `admin-reconcile-controller/7ddc1113764344a99d3dc0510a692a71`;
worker `slice4be-admin-reconcile/46d64de022df47908b3fffa27fac4ef9`.
Five cold/instrumented compiles, Operations startup,86 smoke,202 Settings and
32 chain/48 live-role/15 Create Warehouse pass with exact prior check order,
preservation, normal closure and clean delayed audits. Final chain:
`admin-reconcile-recording-regression/chain-ce50c7639c4046caaeb6c85697667bdd`.
Minimum-size history and typed confirmation captures directly reviewed.

Static `admin-reconcile-recording-static-04`:332 components/6399 procedures/139542
lines;28 caps, dynamic9/45, three schemas,479 parsers pass. Duplicates194: reviewed
+1 exception for distinct fixed three-ID registries, not duplicate business logic.
The prior one-line layout-adapter exception remains.

## 5. Do Not Repeat

- Hidden builds twice crashed in VBE7.DLL/c0000005. Canonical builder now offers
  opt-in `-VisibleHost` with a disposable unsaved host; default remains unchanged.
  This is a diagnostic accommodation, not a native-crash repair.
- First chain crashed in ntdll.dll/c0000028 at Shipping Shipments Sent; its
  0x800706BE/assisted-cleanup run is not GREEN. Generated recovery was verified
  and closed via normal WM_CLOSE, without COM attachment or force-kill. Separate
  fresh chain passes; root cause remains unresolved. Exact failed-run reference
  and safe diagnosis are in the code receipt.
- InvokeCallback returns successful-queue observation, not invocation success.
  A no-queue assertion must require False and unchanged queue count. The corrected
  test was rerun RED/GREEN; the earlier247/1 observer failure is not GREEN.
- Older scoped tests assert historical catalog versions. When rerunning on34,
  explicitly reconcile the version assertion with the spec; retain all checks.

## 6. Assumptions to Re-verify

Candidate pins, closed Excel and interactive desktop must be current. Raw runtime
reports/screenshots/fixtures stay ignored. Do not promote the candidate implicitly.

## 7. Open questions and blockers

Reconcile storage-failure, active recording/publication/guide proof and remaining
Admin coverage are open. Local eligibility is unresolved: shared Core training
context/store require an allowed NAS target, while D18 names the selected runtime
store and D8 preserves Admin local business access. WH_SOURCE_LOCAL differs from
WH_SOURCE_FALLBACK; the existing local business test uses fallback. No local
recording exclusion, storage-policy change or Operations-style business restriction
is approved here. The native Excel crash above remains unexplained.

## 8. Immediate next action

Extend the packaged Reconcile gate with a controlled activity-store failure and prove the actual callback queues once, reports one fixed tracking warning and preserves inventory before changing implementation or adding publication/guide proof.

## 9. Critical references

- v4.11 D8-RECON-01/D14-RECON-01/D18 Reconcile map; Plan022; Controls1.540.
- Code Reconcile receipt and `plan022_slice4be_admin_remaining_coverage.md`.
- `modAdminShipmentReconcile`, `frmShipmentReconcileSelection`,
  `cAdminReconcileActivity`, `modAdminReconcileCodes`, `modActivityStore`.
- `Test-Slice4beAdminReconcileIdentity.ps1 -DeployRoot deploy/validation-admin-reconcile-recording-06 -Phase GREEN -NativePresentation -CheckRecording`.
- `Slice4beAdminReconcileRecording.ps1`; use existing publication/guide test
  patterns in `Slice4beAdminNavigationRecorded.ps1` without fabricating records.
