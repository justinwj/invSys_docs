# Scale preservation and pending failure contract

## 1. Goal and release outcome

Finish 4be-A recording/Event Viewer/How-To authoring, including approved early B0
Receiving replay, under Architecture v4.11/Plan022; stop before broader 4be-B.
4be-A remains incomplete. This checkpoint advances D14/D18 Production evidence.

## 2. Current verified state

Last verified:2026-10-11,23:00 UTC. Code main `0d89557e` is pushed; docs main
before this update is `292e0a6`. Current unpromoted candidate is
`deploy/validation-run-scale-empty-recipe-01`, catalog31. Only `mProduction`
differs from frozen `validation-run-scale-disabled-01`;312 compiled components
are unchanged. Focused61, disabled160, smoke86 and static gates pass. Excel and
the passive desktop monitor are closed; no rebuild is permitted with Excel open.
Code is clean. User-owned docs changes remain: handoff067; guidance023,024 REPORT,
025 GUIDANCE; deletion of old024. Four retained document hashes were unchanged.
Architecture, Plan022 and Controls1.514 are synchronized in this docs update.

## 3. Decisions and constraints

RUN-SCALE-01 and RUN-UI-01 are approved, implemented and scoped-tested. Earlier
handoff125's pending status is superseded. RUN-SCALE-02 is **proposed, unapproved**:
after a worksheet load returns False, stop subsequent scaling/output preparation/
refresh and display "Recipe could not be loaded. Scale was not applied." Keep
FAILED/Error/Unknown without claiming rollback inside the owner. An asynchronous
approval question is pending; do not infer approval from silence or prior01 approval.

Current D14 guard returns False before rebuilding staging if the definition is
still missing after refresh. It preserves custom fields but deliberately retains
current subsequent scaling/wording pending02. No hybrid contract. Actual error5
requires timestamp, stop, owned cleanup, handoff/commit/push and exit. No desktop
rebinding, keep-awake, forced Excel kill or COM reattachment to recovery.
User confirmed personally dismissing recovery around15:18PDT; retention choice
is unknown. Do not attribute that dismissal to test automation.

## 4. Evidence and traceability

Exact receipts: code `tests/integration/plan022_slice4be_production_run_local_results.md`
and `plan022_slice4be_native_localization_results.md`; raw data stays ignored.

- Current guard: actual-handler RED54/7 to GREEN61, exact order and48 retained
  checks; no injected owner result/fault. RED destroyed custom fields and recorded
  the wrong terminal; GREEN stops before rebuild, preserves fields and records
  FAILED. Five cold/instrumented compiles, disabled160, smoke86, preservation,
  unassisted closure and delayed native audits pass. Static320/6342/138754,
  dynamic9/45, duplicates192,28 caps unchanged; three schemas and458 scripts pass.
- Current visible evidence still says the recipe loaded and scales prior values;
  descriptions clip. This motivates pending02, not visible acceptance.
- Prior disabled01: enabled218, loaded503, smoke86 and layout qualify. Layout's
  apparent black combined previews were not blank files: original PNGs are readable
  and duplicate requests have identical hashes. Review amendments preserve history.
- Prior Scale01: guide104 (RED53/1), fault245, yield236, policy218, chain32/live48/
  warehouse15 and full reusable171 Boolean observations/two aggregates qualify.
  General871, SettingsActivity548, UOM228, Settings202, user-policy104 and B0 native121
  retain their original candidate/scope; do not silently claim current-candidate runs.
- Native failure remains: ordinary disabled01 chains crash at two-batch action or
  projection rebuild (chain5/1; live35/1 or32/1; warehouse15). Observer captures
  first-chance C0000005, then first/second-chance ntdll C0000028. Cause unknown.
  Calibrated observer now captures the first AV stack (RED46/3 to GREEN49).
  Two subsequent observed business passes did not reproduce it; one deliberately
  skips final static. Neither establishes ordinary native acceptance or a repair.
- Dismissal helper now confines input to the original process identity: RED1/1 to
  GREEN2/2. This is a separate tooling correction, not a native crash fix.

## 5. Do Not Repeat

Do not blindly retry chains until one passes, equate DLL names with root causes,
or classify recovery as user activity without evidence. Retain the calibrated
observer for the next justified reproduction. No Python/pwsh installation for
convenience. The maintenance generator validates all three schemas; do not repeat
expensive schema checks after success. Rehash package files only after Excel closes.
Use rg to discover paths. Reopen an individual original image before rejecting a
black combined preview. Do not rerun the24-minute reusable test without a reason.

## 6. Assumptions to re-verify

Fresh desktop/input check and monitor before Excel work; package hashes and current
Git state. No error5 occurred in this session. Clean cursor reads alone do not prove
input. Native observers may change timing. Current candidate has no fresh full-chain
or geometry run; previous results remain explicitly scoped.

## 7. Open questions and blockers

RUN-SCALE-02 awaits approval. Successful worksheet reload, general D14 rebuild
preservation, independent worksheet guidance, comprehensive Operations/Admin
coverage, long/multiline visible acceptance and clean ordinary native-chain gates
remain open. No percentage or full acceptance is asserted.

## 8. Immediate next action

Resolve RUN-SCALE-02 approval, then record it in the three contract artifacts and
run actual-handler RED for missing-definition/caught-owner failure quantities and
exact wording before changing `frmProduction.ApplyWorksheetRunScale`.

## 9. Critical references

- Architecture v4.11 D13/D14/D18, RUN-SCALE-01/02 and RUN-UI-01; Plan022; Controls1.514.
- `mProduction.LoadRecipeChooser`, `frmProduction.ApplyWorksheetRunScale`.
- `tests/tooling/Slice4beProductionRunWorksheetScale.ps1`,
  `Test-Slice4beProductionRunLocal.ps1`, `NativeExceptionObserver.cs`.
- Ignored GREEN controller `production-run-local-controller/3cec570be61d4c5faae5f490dbdb974e`;
  worker `slice4be-production-run-scale-reload/415e075c97ee48f9ae47da73fa4f17e4`.
- Ignored `run-scale-empty-recipe-build-01`, `run-scale-empty-recipe-static-01`;
  detailed integration results name the RED/regression/native receipts.
