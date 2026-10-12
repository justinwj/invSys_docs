# Admin coverage audit; identity prerequisite next

## 1. Goal and release outcome

Complete4be-A recording/Event Viewer/How-To authoring and approved early B0 under
v4.11/Plan022, then stop before broader4be-B. **4be-A remains incomplete.** The
remaining Admin entry map now identifies concrete prerequisites to comprehensive capture.

## 2. Current verified state

Last verified:2026-10-12,03:43 UTC. Both branches main. Code `b0405364` is pushed
and clean, following `a0491583`. Docs base `07dcf62`; Controls1.528, synchronized
audit notes and this handoff follow in the next docs commit. All five candidate
hashes remain unchanged: `deploy/validation-admin-entry-02`, catalog33/151.
No Excel automation, builds, runtime edits or desktop input occurred this turn.
Excel is closed; no new monitor/helper is running. This is not a fresh desktop test.

Preserve user docs: modified handoff067; deleted old024 Delivery Overrun; untracked
023 Critique,024 REPORT and025 GUIDANCE. Raw reports/packages/captures remain ignored.

## 3. Decisions and constraints

No new ControlId, outcome, exclusion, replay adapter, permission or business rule
was approved. Source findings do not supply behavioral RED. Follow D14 exact keys;
do not invent a ROW/SKU compatibility contract. If correction semantics need to
change, resolve and approve v4.11 first. Preserve all prior approvals.

Actual desktop Win32error5 still requires timestamp, runtime stop, owned cleanup,
handoff and exit. Revalidate desktop before runtime work. Serial Excel jobs,
delayed native audits, no force-kill/recovery COM reattachment/desktop rebinding.

## 4. Evidence and traceability

Code `tests/integration/plan022_slice4be_admin_remaining_coverage.md` maps all14
packaged Actions buttons and separately identifies three Session/target controls.
All14 IDs, enable/dispatch callbacks and source macro mappings agree. Ignored
`reports/runtime/admin-remaining-source-audit-01/{ribbon,map}-verification.json`
records the pinned package/source evidence; RuntimeAcceptance is false.

The source audit changes the next priority:
- **Confirmed D14 source conflict:** reachable `OpenShipmentReconcileTool` selects
  EventID/SKU without System_Key, uses SKU history/balance, reads `tblSkuCatalog.ROW`
  in `ResolveRowForSku`, then queues `CreatePayloadItem`'s Row/SKU payload.
  Required test: actual packaged callback in generated training inventory, selected
  exact entity plus another entity sharing SKU, exact queued key and preservation.
- **Auth read finding, effects unverified:** `frmCreateDeleteUser` Refresh calls
  `OpenSelectedAuthWorkbookForm`; its closed-workbook branch opens writable and calls
  `modAuth.EnsureAuthSchema`. Borrowed and write callers differ. Required test: actual
  Refresh on generated complete/incomplete Auth, no create/repair/format/dirty/save,
  caller-owned book preservation and current rights/context. Reconcile D8-A before edits.
- The generated Ribbon checks ADMIN_MAINT before macros; several macros do not
  repeat it. Do not replace actual dispatch/handler authorization proof with a service call.

Prior Settings recording125, Close guide123, native177 and launcher98 remain valid
at their documented scopes (handoff136/results); no new runtime pass is claimed.

## 5. Do Not Repeat

Do not treat public functions or unit-test callers as operator reachability.
The current Ribbon omits direct processor/lock/reissue/snapshot/publication buttons;
the console removes old `btnAdmin` shapes. Complete reachability review before an
exclusion. Do not delete legacy/shared code automatically or globally replace
CreatePayloadItem without reviewing its other callers. Do not infer whether Domain
accepts/rejects the current correction from this source audit; it has not been run.
Use `src/InventoryDomain`, not guessed `src/Domain` or `src/Inventory.Domain` paths.

## 6. Assumptions to Re-verify

Recheck Git, package pins and Excel closure; start the passive monitor before UI
work. Keep generated fixtures isolated. Prior ordinary full-chain native faults
remain unresolved. Ignored verification/helper scripts require inspection before use.

## 7. Open questions and blockers

No behavioral RED exists yet for the newly found identity/read paths. Exact
correction semantics across repeated/multiline shipment events need owner-level
review before changes; never derive an entity from SKU or position. Remaining
Operations/Admin lifecycle/selection coverage, replay-control observation accounting,
broader layout/human/full-chain gates remain open. Prior early B0 scoped121 is valid
evidence, not whole4be-A acceptance. General long values still clip.

## 8. Immediate next action

Create and run a focused packaged Shipment Reconcile callback test on Admin-generated training fixtures that proves the selected entity's exact System_Key and isolation from another entity with the same SKU before changing that owner or adding its recording contract.

## 9. Critical references

- v4.11 D14 source-audit checkpoint, D18 comprehensive coverage, D8-A Auth separation; Plan022; Controls1.528.
- Code `plan022_slice4be_admin_remaining_coverage.md`, `plan022_slice4be_remaining_acceptance.md`; handoff136 for prior gates.
- `tools/build-xlam.ps1`: `Add-RibbonCallbacksModule`, Admin Ribbon groups.
- `src/Admin/Modules/modAdminShipmentReconcile.bas`: `OpenShipmentReconcileTool`, `BuildRecentShipmentSentRows`, `DetectNasIncreaseAfterShipEvent`, `ResolveRowForSku`, `QueueAdminShipmentReconcileEvent`.
- `src/Core/Modules/modRoleEventWriter.bas`: `CreatePayloadItem`, `CreateInventoryEntityPayloadItem`, `QueuePayloadEvent`.
- `src/InventoryDomain/Modules/modInventoryApply.bas`: `BuildPayloadLines`, `ValidateAdminShipmentReconcileLine`; preserve current Domain authority.
- `src/Admin/Forms/frmCreateDeleteUser.frm`: `mBtnRefreshUsers_Click`, `RefreshUsersForm`, `OpenSelectedAuthWorkbookForm`; the helper also serves writes.
