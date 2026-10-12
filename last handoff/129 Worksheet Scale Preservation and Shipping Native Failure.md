# Worksheet Scale preservation and Shipping native failure

## 1. Goal and release outcome

Finish 4be-A recording/Event Viewer/How-To authoring and approved early B0 Receiving
replay under Architecture v4.11/Plan022; stop before broader4be-B. **4be-A is incomplete.**
This checkpoint enforces existing D14 on successful worksheet reload/Scale; full-chain
acceptance remains blocked by an intermittent native Excel failure.

## 2. Current verified state

Last verified:2026-10-12,00:51 UTC. Both branches main. Code `f69cc396` is pushed;
docs base `0e87acb`, with this evidence/Controls1.519 update to follow. Current
unpromoted candidate: `deploy/validation-run-scale-success-02`, catalog32/145.
Excel is closed. Owned passive monitor stopped at00:51:18.796 UTC after425 samples,
zero cursor/desktop/capture failures and zero error5. It does not prove RDP/input reliability.

Preserve user-owned docs: modified handoff067; untracked guidance023,024 REPORT,
025 GUIDANCE; deleted old024 Delivery Overrun file. Four retained hashes were
verified unchanged. Raw runtime reports/captures remain ignored.

## 3. Decisions and constraints

RUN-SCALE-01/02, RUN-UI-01 and D18-REPLAY-01 are approved; do not ask again.
This correction changes no contract: preserve custom columns under D14, exact
System_Key and captured-workbook authority. A per-load cProductionStagingReload
retains named chooser/palette tables with custom fields, writes managed fields
by normalized name and clears only managed output formulas. Output preparation
does not allocate a premature key. No global captured-workbook state was added.
Actual Win32 error5 requires timestamp, cleanup, handoff, commit/push and exit.
VBA Err.Raise5 is not desktop error5. No COM reattachment to recovery or forced kills.

## 4. Evidence and traceability

Actual packaged Scale RED66/3 -> GREEN69 -> expanded86 preserves custom positions,
values/formulas, exact input identity and repeated non-compounding quantities.
Five cold/instrumented compiles pass. Build02 changes only mProduction, adds the
class and retains314 packaged components. Static323 components/6355 procedures/
138982 lines; dynamic9/45, duplicates192 unchanged; mProduction shrinks20 lines,
other27 caps unchanged; three schemas and461 parsed PowerShell scripts pass.
Two successful Scale captures are reviewed; long recipe descriptions still clip.

Enabled218, missing-definition64 and refusal/caught-failure162 retain exact prior
check order with preservation, normal closure and zero delayed native faults.
Smoke86 also qualifies both unassisted exits. Layout passes18 requested size/page
pairs, six maximized pages and five native transitions. Five original PNGs were
directly reviewed; settings-default's black preview is byte-identical to the
reviewed settings-minimum file. No Excel rerun was needed. Layout is not populated
long-value or human acceptance. Exact controllers/receipts are in Run results below.

Ordinary chain fails5/1, live-role40/1, warehouse15/15 at Shipping
`modTS_Shipments.RunShipmentsSentFormActionForTest`, HRESULT0x800706BE. Windows logs
ntdll.dll/c0000028 at00:45:36.699 UTC; both Production batches and Boxing passed
before it. Controller `reports/runtime/run-scale-success-regression/chain-0518429fa5d44e81b2063b699d3c5c5e`
contains candidate pins and sanitized failed-verification. A verified crash-reporter
child closed after a normal native close request; no recovery prompt was observed,
COM was not reattached and no force was used. Settings/packages/tracked reports
were restored; audit through00:48:40.190 UTC. Closure was assisted, so no chain GREEN.
The signature matches earlier failures at other calls; root cause remains unknown.

## 5. Do Not Repeat

Do not repeat unchanged chains to chase a pass or infer a native repair from clean
focused/smoke runs. Reuse the existing calibrated module/offset observer. Two40/1
fixture failures and a64/5 diagnostic with two wrong test predicates preceded the
qualified RED; they are not RED. Preserve actual names proc_*_rchooser
for chooser tables and proc_*_palette for palettes. Test normalized amount headers,
never rename System_Key. Minimum/default layout requests can have identical bytes.
CIM creation timestamps lose sub-microsecond precision; exact Get-Process timestamp
comparison against CIM falsely rejected cleanup before any close request.

## 6. Assumptions to Re-verify

Check desktop access, Excel absence and candidate hashes before interaction;
restart an owned passive monitor. Qualify delayed native events before another
Excel task. Prior loaded-run503/reusable171 and other guide evidence retain their
original candidate scope, not fresh execution claims.

## 7. Open questions and blockers

Native Shipping-call failure blocks the current ordinary chain; cause is unresolved.
Independent worksheet Scale guides, broader D14 rebuild coverage, Settings Open/page
navigation, remaining Operations/Admin recording and human/multiline/long-value
acceptance remain in the acceptance index. No new architectural approval is pending.

## 8. Immediate next action

Localize the Shipping Sent native failure using the existing calibrated metadata-only
observer and bounded call-boundary tracing before retrying the ordinary chain.

## 9. Critical references

- Architecture v4.11 D14/D18/RUN-SCALE-02; Plan022; Controls1.519.
- Code `tests/integration/plan022_slice4be_remaining_acceptance.md`.
- `plan022_slice4be_production_run_local_results.md`, `plan022_slice4be_native_localization_results.md`.
- `cProductionStagingReload`, `mProduction.LoadRecipeChooser`, `frmProduction.ApplyWorksheetRunScale`.
- `Test-Slice4beProductionRunLocal.ps1 -WorksheetScaleOnly -ScaleDesignsDisabledForTest -ScaleSuccessForTest`.
- `Slice4beProductionRunScaleSuccess.ps1`, `Test-NativeExceptionObserver.ps1`, `NativeExceptionObserver.cs`.
- Runtime roots `run-scale-success-build-02`, `run-scale-success-static-02`, `run-scale-success-regression`.
