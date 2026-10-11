# Native chain localization and fixture isolation

## 1. Goal and release outcome

Finish 4be-A under Architecture v4.11/Plan022; retain General recording/guide proof
while resolving native validation failures before claiming clean release gates.

## 2. Current verified state

Last verified:2026-10-11 UTC. Code main `fe0ff848` is pushed; docs main before this
update is `c1f9835`. Runtime remains `6f583238`, catalog31, frozen unpromoted
`deploy/validation-general-settings-02`. Only diagnostic tools/evidence changed.
General871, smoke86 and UOM228 remain scoped GREENs; 4be-A remains incomplete.
Plan022 and Controls1.502 agree. Excel, controllers and desktop monitor are closed.
No rebuild/deployment occurred. Four user-owned docs hashes were verified unchanged:
handoff067 and guidance023/024 REPORT/025 GUIDANCE; the old024 deletion is preserved.

## 3. Decisions and constraints

No architecture or product contract changed. The original combase fault is not
repaired by clean partial runs or collection controls. Native fault and desktop
Win32 error5 are different. On actual error5, timestamp, stop, safely clean only
owned tests, commit/push the ending handoff and exit as directed. No secondary COM
attachment to live/recovering Excel, desktop rebinding, keep-awake or Windows changes.
Preserve captured binding, exact System_Key, unknown columns, headless authority
and all approved D18 A/B boundaries. Current clone tests use explicit fixture and
package-pin receipts; do not infer candidates or reuse historical defaults.

## 4. Evidence and traceability

Exact receipts and scope: code
`tests/integration/plan022_slice4be_native_localization_results.md`.

- Original chain32/live48/warehouse15 has combase.dll/c0000005 after live completion;
  exact owner/call unknown. Its evidence remains failed at the native gate.
- Passive isolated restart12: Quit returned, Excel lingered210 seconds and exited
  after its worker ended. Collection control12 exited while the worker stayed alive.
  Neither reproduced the crash or established its cause.
- Traced full chain instead failed earlier: ntdll.dll/c0000028 at08:48:52.5688535Z,
  live child created08:47:49.1973544Z. Last passed
  `InventoryDomain.ProjectionRecovery.Delete`; failing step **Delete and rebuild
  canonical inventory projections**. Chain5/1, live32/1, warehouse15/15. Later
  stages unreached. Assisted native recovery closure retained files for later viewing.
- First late-stage clone15 was native-clean but wrote three source test inboxes:
  configured DataRoot still referenced the source; missing station InboxRoot falls
  back to it. Core override alone is insufficient. This is diagnostic fixture RED,
  not product RED; earlier isolated controls did not verify source hashes.
- Corrected late15 and final collected restart12 retain exact prior check order,
  all13 source files/hashes, settings/packages, normal exit and delayed zero faults.
  Only cloned config paths are rebound. Earlier17 full-chain checks are absent.
- Pure tooling56; static319/6340/138712, dynamic9/45, duplicates192 and28 caps
  unchanged; three schemas and455 scripts pass. No runtime compile was required.
- KVM preflight moved/restored the cursor;375 monitor samples over31 minutes had
  zero cursor/desktop/capture failures or error5. Monitor stopped09:10:02Z.

## 5. Do Not Repeat

Do not treat the two native fault classes as one proven cause, DLL names as root
causes, Quit returning as process exit, or passing business counts as native
acceptance. Do not silently restore source fixture writes or erase failed runs.
Historical partial reports inherited full-chain headings; their qualification
receipts reject that scope. The final generator now writes explicit partial scope.
Do not retry an unchanged broad chain or promote collection as a runtime repair.

## 6. Assumptions to re-verify

Desktop input and frozen package hashes before more Excel automation. Native
failures are not reproducible in the focused late controls. Instrumentation may
alter timing; no native stack or failing API has been established. Original
generated source fixture inboxes changed before clone isolation was corrected.

## 7. Open questions and blockers

Both native failures remain unresolved. Remaining Settings regressions, broad
Operations/Admin observation coverage, final live-role/chain/binding/visible
acceptance remain open. RUN-SCALE-01/RUN-UI-01 remain pending decisions; approved
D18-REPLAY-01 and the A finish line remain unchanged.

## 8. Immediate next action

Add owned-process and before/after call tracing to the live child's projection
deletion/rebuild boundary, verify tracing preserves its assertions, then run one
qualified full-chain diagnostic with the existing later-stage trace retained.

## 9. Critical references

- Architecture v4.11 D13/D18; Plan022; Controls1.502; remaining-acceptance index.
- `tests/tooling/New-Slice4beChainTrace.ps1`, `Slice4beShutdownTrace.ps1`,
  `Test-Slice4beShutdownTrace.ps1`, `Test-Slice4beShutdownControl.ps1`.
- `tools/validate_release1_full_chain.ps1`: `New-OrderedLiveValidator`,
  `Invoke-RestartReconciliation`, `Invoke-RuntimeFivePackageEvidence`.
- `tools/validate_phase6_live_role_workflows.ps1`: projection recovery step.
- Native localization results give exact ignored receipts; General Settings
  results retain871/86/228 scope and original native-failed chain evidence.
