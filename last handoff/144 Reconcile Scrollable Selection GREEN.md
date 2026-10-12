# Reconcile scrollable selection GREEN

## 1. Goal and release outcome

Finish4be-A recording/Viewer/How-To and approved early B0 under v4.11/Plan022;
stop before broader4be-B. **Incomplete; goal active.** This checkpoint advances
D14-RECON-01 by making all20 shipment choices readable and reachable.

## 2. Current verified state

Last verified2026-10-12,06:34 UTC. Both main: code `3bf60c1a`, docs `d59e609`
before this handoff. Code clean; push both repositories before exit.
Excel closed; all runtime/static/monitor handles drained. No promotion.
Candidate: `deploy/validation-admin-reconcile-selection-02`; pins:
`reports/runtime/admin-reconcile-selection-build-02/compiled-pins.json`.
Controls1.538; tracking catalog33/151 unchanged. Preserve user docs: modified067,
deleted old024 Delivery Overrun, untracked023 Critique/024 REPORT/025 GUIDANCE.
Their four starting hashes and deletion were verified unchanged.

## 3. Decisions and constraints

D14-RECON-01 and D8-RECON-01 are approved; no approval remains pending here.
Admin owns `frmShipmentReconcileSelection`: locked/wrapped/scrollable full history,
numbered choice, Inspect/Cancel, minimum540x360 and default720x480. It returns to
the existing callback validation. Quantity, exact identity, captured live authority,
permitted local targets and headless processing remain unchanged. Do not replace
Core's live `modAuth.CanPerform` check with the NAS-only role wrapper.

Keep all prior invariants/approvals. On desktop Win32error5: timestamp, stop
runtime, owned cleanup, handoff/commit/push and exit. VBA Err5 is different.
Serial Excel jobs; no force-kill, COM recovery attachment or desktop rebinding.
Keep controllers alive through cleanup; do not edit their pinned tooling live.

## 4. Evidence and traceability

Exact receipt: code `tests/integration/plan022_slice4be_admin_reconcile_results.md`.
Pre-implementation native179/2 RED -> **191/191 GREEN**, retaining all181 prior
checks in order and the original172 prefix. Native Home/End reaches entry20;
Escape cancels. Native Tab/20/Enter reaches the actual Inspect handler and exact
Domain event/key lookup, concluding without queue when current quantity is lower.
Inventory bytes, quantities, custom values and saved state hold. Six reviewed
foreground captures cover default/minimum/grow/maximize/restore and Inspect entry.
The notice seam supplies the conclusion assertion, not a native confirmation image.

Qualified controller `admin-reconcile-controller/825b1a529c504fc6bd54f0b8f3734765`;
worker `slice4be-admin-reconcile/4397cbda0d054a6f8920d6d8d0f5368d`, under runtime.
UTC06:24:13--06:26:09; clean delayed audit through06:26:21.6691404.
Five cold/instrumented compiles, Operations startup, preservation and normal closure
pass. Only Admin Reconcile changes/new form;321 packaged components unchanged.

Same candidate:86 smoke;32 full-chain/48 live-role/15 Create Warehouse, exact prior
order, normal preserved closure and clean delayed audits. Chain controller:
`admin-reconcile-selection-regression/chain-98c7d4114a4048b6997d451769713736`,
audit through06:32:31.1695957 UTC. Static `admin-reconcile-selection-static-03`:
330 components/6390 procedures/139369 lines, all28 caps, dynamic9/45, three schemas,
476 PowerShell parsers. **Reviewed duplicate exception:**193 (+1) for the one-line
UserForm_Layout adapter forwarding to the existing shared anchor manager; no
duplicate layout implementation or scanner relaxation.

## 5. Do Not Repeat

- Keep a disposable visible operator workbook for native testing. Hiding all
  fixture windows also hides Excel; startup Visible=True alone did not survive.
  Hidden-host EXCEL.EXE access violations occurred before native input. The
  underlying Excel fault is not repaired or accepted; both qualified visible-host
  runs closed normally. Assisted recovery runs are diagnostic only.
- Set this FRX-less form's caption in Initialize; the designer initially kept
  UserForm1. Do not broaden this into an untested global builder change.
- MSForms caret end3210 differs from value length3229 with19 CRLF separators.
  Calibrate the control's end after capture; native Home then End after resizing
  proves viewport reachability. Caret position alone was insufficient.
- Parenthesize Boolean Start-Job arguments; an unparenthesized cast became a
  truthy string and wrongly sent Inspect during Cancel. Keep Check output outside
  returned receipt objects, and require all four resize cases explicitly.

## 6. Assumptions to Re-verify

Check package pins, Excel closure and desktop before runtime. The stopped monitor
observed516 samples,05:50--06:33 UTC, zero desktop error5. Read/capture probes do
not prove mouse movement; native keyboard input is separately proved above.

## 7. Open questions and blockers

Native confirmation/narrative and window-close coverage remain open, followed by
comprehensive Admin/Operations recording and guide proof. No new ControlId was
added. Earlier Settings/Auth/B0 evidence does not close4be-A. Hidden-host native
failure remains a diagnostic limitation; use the verified visible operator setup.

## 8. Immediate next action

Extend the same packaged callback gate to native confirmation/narrative and window-close cancellation, preserving all191 checks, before integrating Reconcile recording under the existing D18 contract.

## 9. Critical references

- v4.11 D8/D8-A/D13/D14/D14-RECON-01/D8-RECON-01/D18; Plan022; Controls1.538.
- Code Reconcile results and `plan022_slice4be_admin_remaining_coverage.md`.
- Admin `modAdminShipmentReconcile`, `frmShipmentReconcileSelection`.
- Core `modAdminReconcileAccess`; Domain Reconcile read/apply owners unchanged.
- `Test-Slice4beAdminReconcileIdentity.ps1 -DeployRoot deploy/validation-admin-reconcile-selection-02 -Phase GREEN -NativePresentation`.
- `Slice4beAdminReconcileSelection.ps1`, `Slice4beAdminReconcileNative.ps1`;
  ignored `qualify-admin-reconcile-selection-green.ps1` currently expects191.
