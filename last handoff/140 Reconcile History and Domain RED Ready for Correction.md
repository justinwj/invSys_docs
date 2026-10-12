# Reconcile history/Domain RED ready for correction

## 1. Goal and release outcome

Finish 4be-A recording/Viewer/How-To and approved early B0 under v4.11/Plan022;
stop before broader4be-B. **Incomplete; goal remains active.** Qualified packaged
tests now protect the approved Reconcile rule through actual Domain application.

## 2. Current verified state

Last verified2026-10-12,04:35 UTC. Both branches main, pushed: code `de37ee1e`,
docs `59dfd34`; this handoff follows in a documentation commit. Code clean.
Only user docs changes remain: modified067, deleted old024 Delivery Overrun,
untracked023 Critique/024 REPORT/025 GUIDANCE. Preserve them. Excel is closed;
test/static/monitor handles are drained. No runtime implementation changed here.

Use frozen `deploy/validation-admin-auth-read-01`, catalog33/151. Reconcile,
Core and Domain are unchanged from candidate02. Auth prerequisite111/111 and
its visible evidence remain valid. Build/package receipts in handoff139/results.
Do not rebuild open packages, overwrite either candidate or promote deployment.

## 3. Decisions and constraints

**D14-RECON-01 is approved**, not pending. Exact event/key, entity-only current
quantity versus all its history through that event's AppliedSeq; negative delta
with preview/narrative, current attributes preserved, no automatic rollback or
SKU/ROW inference. Inspection is nonmutating; Domain enforces event/key association.
v4.11, Plan022 and Controls1.532 agree. No new tracking ID or exception approved.

Keep Core/Domain headless and calculations/validation in their owners. Use declared
primitive/serialized result envelopes at XLAM boundaries; do not copy legacy
workbook-returning bridges into a new interface. Preserve exact identity, unknown
columns, captured binding and all accepted GREEN checks. Current-source behavior
and legacy unit fixtures cannot override the normative contract.

Desktop Win32error5 requires timestamp, stop runtime, owned cleanup, handoff and
commit/push, exit. Serial Excel jobs; no force-kill, recovery COM reattachment or
desktop rebinding. Controller pins every tooling script; do not edit while running.

## 4. Evidence and traceability

Exact record: `tests/integration/plan022_slice4be_admin_reconcile_results.md`.
Final **31 PASS /24 expected FAIL**,55 checks, retains original18 outcomes/order.
Five compiles, exact receipt/log agreement, package/tooling/settings preservation,
normal unassisted shutdown and clean delayed native audit through04:32:59.7929839.
Controller `admin-reconcile-controller/19fc5155c0db4587837b7b3d34d7b6dd`, worker
`slice4be-admin-reconcile/b7f66bcb810f4fd686f12d65472f5dc6` under reports/runtime.

Real Admin-generated inventory and Domain fixture events establish:
- Older shipment: current A21 versus selected after-event15 => -6, excluding B39.
- Multi-entity/multiline event: A's two lines yield18; current A22/B55 => -4.
- Distinct canaries are bound to each System_Key, saved, and rows sorted before
  inspection. Callback preserves values/bytes but dirties inventory.
- Actual queued payload reports APPLIED without the correct entity quantity and
  loses custom values on rebuild. Current Location/Condition and idempotency pass.
- Wrong-entity, non-SHIP and positive corrections mutate quantities/history;
  missing narrative is correctly refused.

Failures: original3 +10 history identity/delta/prompt/attribute/read checks +2
queued-application checks +9 Domain guard checks. No native-dialog/full processor
acceptance claimed; only prompts are deterministic seams, not business behavior.

Static `admin-reconcile-history-red-static-01`: all28 caps hold; unchanged326
components/6371 procedures/139226 lines, dynamic9/45,192 duplicate candidates;
three schemas and473 PowerShell scripts validate.

## 5. Do Not Repeat

Fixture payload factory defaults IoType=CREATE: explicitly use SHIP/ADJUST.
VBA object-return functions with required arguments cannot be indexed by their own
function name; use a local object and then Set the return. One compile dialog
needed verified native OK control2 dispatch before original cleanup completed;
no kill/COM reattachment. That attempt is not RED or normal-shutdown acceptance.

Fixture event application clears prior projection canaries. Restage/prove them
immediately before the read test, then test actual queued application separately;
do not attribute fixture-time loss to the callback or remove the application check.
Use direct ConvertFrom-Json assignment, shared-read hashing and VBA fixture setup.

## 6. Assumptions to Re-verify

Fresh desktop checks/package pins/Excel closure before runtime. Monitor
04:20:44–04:35:17 UTC:174 samples, zero cursor/desktop/capture/error5 failures,
stopped normally. Read access alone is not input proof. No new native input gate.

## 7. Open questions and blockers

No contract approval is pending for this correction. Runtime fix is not started.
Core's existing resolver enters create/schema maintenance during inspection;
`RunInventoryQueryReadOnlyLocal` provides a lease pattern, but its default path
builder has fallback roots, so preserve explicit trusted/captured target binding.
Domain `ValidateAdminShipmentReconcileLine` only checks event existence/narrative.
`RewriteEntityProjectionTable` clears rows and rewrites managed fields without
restoring unknown values; preserve them by exact key, not row position.

Closed/missing/invalid authority, cancellation, roles, native/layout, full processor
and broader regressions remain to prove. Remaining Admin/Operations recording,
full layout/human/full-chain gates and Shipping native faults stay open. Prior
Settings125/123/177/98 and early B0 scoped121 do not close4be-A.

## 8. Immediate next action

Implement approved D14-RECON-01 through a Core read-only lease and headless Domain quantity/association rules, preserve custom values during projection rebuild, and drive the existing55-check RED to GREEN before claiming completion.

## 9. Critical references

- v4.11 D3/D14/D14-RECON-01/D18; Plan022; Controls1.532; coverage/result files.
- `Test-Slice4beAdminReconcileIdentity.ps1`, `Slice4beAdminReconcileIdentity.ps1`, `Slice4beAdminReconcileHistory.ps1`.
- `modAdminShipmentReconcile` (561 lines); Core `modInventoryDomainBridge` (956).
- Domain `modInventoryBridgeApi`, `modInventoryQueries`, `modInventoryApply`.
- `modInventoryApply` has a2882-line no-growth ratchet; extract cohesive owner logic if needed.
- Source searches find old Reconcile public helpers used only internally and by legacy `TestPhase6CoreSurfaces.bas`; review reachability before changing/removing them, and do not retain SKU/ROW authority for those old tests.
