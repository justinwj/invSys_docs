# Shipment Reconcile RED; quantity decision pending

## 1. Goal and release outcome

Finish4be-A recording/Viewer/How-To and approved early B0 under v4.11/Plan022;
stop before broader4be-B. **Incomplete.** This turn establishes D13 behavioral
RED for a reachable Admin prerequisite, without changing runtime implementation.

## 2. Current verified state

Last verified2026-10-12,04:00 UTC. Both branches main. Code `ec4dc3ee` is pushed
and clean; docs base `edb04aa`, synchronized proposal/Controls1.529 and this
handoff follow in the next commit. Candidate `deploy/validation-admin-entry-02`
remains unchanged, catalog33/151. Excel is closed; monitor/helper jobs are drained.
Preserve user docs: modified067, deleted old024 Delivery Overrun, untracked023
Critique/024 REPORT/025 GUIDANCE. Raw reports/packages remain ignored.

## 3. Decisions and constraints

**D14-RECON-01 is PROPOSED, not approved.** An async approval question is pending:
exact selected entity's current quantity versus balance immediately after the
selected shipment event; preview negative difference, require narrative, preserve
current attributes, no automatic rollback. See v4.11 near4998. Do not infer approval
from the existing exact-identity rule or invent repeated/multiline semantics.
No new tracking ControlId, exclusion or outcome is approved. Prior approvals stand.

Actual desktop Win32error5 requires timestamp, runtime stop, owned cleanup,
handoff/commit/push and exit. Serial Excel jobs; no rebuild while open, force-kill,
recovery COM reattachment or desktop rebinding. The user says Firefox/Outlook
setup may explain earlier unexpected input; causation remains unconfirmed.

## 4. Evidence and traceability

`tests/integration/plan022_slice4be_admin_reconcile_results.md` is the exact receipt.
Final actual packaged callback RED: **15 pass/3 fail**, five compiles. Generated
Admin training/CSV entities share SKU; Domain applies fixture shipment/adjustment.
Failures: missing selected System_Key, legacy Row payload, inventory becomes dirty.
Both quantities, file bytes, saved unknown column and other Config remain intact.
Presentation prompts alone are deterministic seams; callback/lookup/queue are real.
No native-dialog or Domain-application acceptance is claimed.

Controller `admin-reconcile-controller/98f7f7b2ba024611b27f0004edf6fd4a`, worker
`slice4be-admin-reconcile/3a6a8caff1b24490abeef3a809f092cb` under reports/runtime:
exact checks, package/settings preservation and normal closure; no native failures
through03:57:02.8767575 UTC. Static `admin-reconcile-red-static-01` holds all28 caps,
326/6371/139227 components/procedures/lines, dynamic9/45,192 duplicate candidates;
three schemas/471 PowerShell scripts pass. Prior Settings125/123/177/98 still scoped.

Read-only cause to isolate: Core resolver enters its local create/schema path for
borrowed inventory, contrary to D3 query-lifetime requirements. Existing
`RunInventoryQueryReadOnlyLocal` provides the established lease pattern. Do not
assume the source trace alone establishes every dirty-state cause.

## 5. Do Not Repeat

Earlier fixture/hash/JSON/canary attempts are not RED. On PowerShell5 assign
ConvertFrom-Json directly; wrapping the pipeline in @() nests its array and gives
false property checks. Use shared-read file hashing and VBA canary staging with a
passing pre-callback baseline. Do not infer column loss from failed COM setup.
One earlier hash-failure run required owned WM_CLOSE; final run closed normally.
No kill or COM reattachment occurred. Preserve the final qualified receipt.

## 6. Assumptions to Re-verify

Fresh desktop validation before runtime. Monitor03:48:14–03:59:51 UTC recorded139
samples, zero cursor/desktop/capture failures, then stopped. Read success is not
input proof. Recheck Git, package pins and Excel closure. Legacy unit tests use
Row/SKU/migration fixtures; they cannot redefine D14 or replace packaged proof.

## 7. Open questions and blockers

D14-RECON-01 approval is pending; no implementation started. Auth Refresh's D8-A
read/schema issue remains an independent test-first task if approval is still
pending. Remaining Admin/Operations capture, broader layout/human/full-chain gates,
replay observation accounting and ordinary Shipping native faults stay open.
General long values still clip. Early B0 scoped121 is not whole4be-A acceptance.

## 8. Immediate next action

After explicit D14-RECON-01 approval, add focused repeated/multi-entity and Domain event/key guard tests, then correct the packaged exact-key/read path while preserving the qualified RED.

## 9. Critical references

- v4.11 D3/D14/D14-RECON-01/D18; Plan022; Controls1.529.
- Code `Slice4beAdminReconcileIdentity.ps1`, `Test-Slice4beAdminReconcileIdentity.ps1`, `Test-Slice4beConfigCommands.ps1`.
- `modAdminShipmentReconcile.OpenShipmentReconcileTool`, `QueueAdminShipmentReconcileEvent`.
- `modInventoryDomainBridge.RunInventoryQueryReadOnlyLocal` and `OpenOrCreateCanonicalInventoryWorkbookLocal`; Domain `modInventoryApply.ValidateAdminShipmentReconcileLine`.
- Handoff137/Admin coverage map for Auth and remaining entries;136/Settings results for retained gates.
