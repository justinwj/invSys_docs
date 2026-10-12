# Admin Close and approved Scale failure guard

## 1. Goal and release outcome

Finish 4be-A recording/Event Viewer/How-To authoring, including approved early B0
Receiving replay, under Architecture v4.11/Plan022; stop before broader 4be-B.
**4be-A remains incomplete.** This checkpoint advances D18 observations and the
approved RUN-SCALE-02 failure contract without claiming comprehensive acceptance.

## 2. Current verified state

Last verified:2026-10-12,00:02 UTC. Both branches are main. Code `8762b4e2` is
pushed, following Admin Close `348c62fc`; code tree is clean. Docs base is pushed
`72225bb`, which recorded RUN-SCALE-02 approval before implementation. This update
synchronizes Architecture, Plan022, Controls1.517 and this handoff.

Current unpromoted package is `deploy/validation-run-scale-stop-01`, catalog32/145
controls. Only `frmProduction` and `modProductionRunScaleActions` differ from
`validation-admin-close-02`;313 compiled components match. Excel is closed.
The owned passive desktop monitor is stopped:674 samples, zero error5, last sample
00:02:16.403 UTC. This is not proof that RDP/locking is fixed. No rebuild with Excel open.

Preserve user-owned docs: modified handoff067; untracked guidance023,024 REPORT,
025 GUIDANCE; deleted old024 Delivery Overrun file. Four retained document hashes
match their prior values. No generated runtime evidence is staged or committed.

## 3. Decisions and constraints

RUN-SCALE-01, RUN-UI-01 and RUN-SCALE-02 are approved; do not ask again. Scale02
stops after a False worksheet-load result and the captured-context check, before
scaling/output preparation/subsequent refresh. Exact message: "Recipe could not
be loaded. Scale was not applied." FAILED/Error/Unknown makes no rollback claim.
The reusable Execute branch is unchanged. The form shrinks two lines by putting
the typed result check in the existing Scale workflow module.

D18 catalog32 registers deliberate Admin Settings button/native Close. It observes
dismissal/discard only, never saved settings or Domain application. Lost permission
cannot trap Close; stale context cannot retarget records. Internal Unload/shutdown
is excluded. Shared Core dismissal vocabulary retains Production's existing words.
This refines the approved comprehensive-recording contract; it does not complete
coverage of Settings Open/pages or every Operations/Admin control.

Actual desktop Win32 error5 still requires timestamp, owned cleanup, handoff,
commit/push and exit. Do not force-kill Excel or reattach to recovery. User confirmed
they dismissed the earlier15:18 PDT Document Recovery prompt; retention choice is unknown.

## 4. Evidence and traceability

Scale02: missing-definition RED61/3 -> GREEN64; caught-owner-failure RED159/3 ->
GREEN162. Both fail only preservation/post-load-work/message predicates before
implementation. GREEN proves exact key/custom fields/formulas, FAILED facts and
the fully readable approved message. Enabled-Designs218 retains exact prior order.
Five cold/instrumented compiles, preservation and normal delayed-clean shutdown pass.
Current chain32/live48/warehouse15, smoke86 and layout18 requested page/size pairs,
six maximized pages/five native transitions pass. Six layout captures are reviewed.
Static:322 components,6346 procedures,138837 lines, dynamic9/45, duplicates192;
form minus2 lines, other27 oversized caps unchanged, three valid schemas and459
parsed scripts under tools/tests-tooling. No human acceptance or deployment promotion.

AdminClose02: RED34/19 -> GREEN53, extended GREEN70 covering user-off, old policy,
permission/context loss and unavailable storage notices. Production Close232,
chain32/live48/warehouse15, smoke86 and static gates pass on that predecessor.
Initial AdminClose01 Settings202 retains its scope. Older loaded-run503 and full
reusable171 Boolean/two-aggregate evidence retain their original candidate scopes.

Exact controllers, workers, dates, builds and qualified receipts are in code
`tests/integration/plan022_slice4be_production_run_local_results.md` and
`plan022_slice4be_admin_close_results.md`. Raw JSON/images remain ignored under
`reports/runtime/`. New runtime builds/static roots are `run-scale-stop-build-01`
and `run-scale-stop-static-01`. Current ordinary chain is
`run-scale-stop-regression/chain-78f29462f4a84ddfa7841dc256eca4c3`.

## 5. Do Not Repeat

Do not infer native-crash repair from these passing chains. Earlier ordinary chains
failed with ntdll C0000028; first-chance C0000005 was also observed. Root cause is
unresolved. Use a new diagnostic question if it recurs, not repeated unchanged runs.
Do not copy separate Close vocabulary builders: they added duplicate groups; the
shared module restores192. Black combined previews are not source-image evidence:
individual original review and equal minimum/default hashes resolved this artifact.
Do not count loader/compile/harness failure as RED, or registration as acceptance.

## 6. Assumptions to Re-verify

Check actual desktop access before interaction and restart an owned passive monitor
if needed; the previous monitor is intentionally stopped. Verify Excel and package
hashes before building/testing. Qualify delayed native failures before another Excel run.

## 7. Open questions and blockers

No Scale02 approval remains pending. Admin Close still needs independent recording,
guide authoring and How-To/Diagnostic/Compare conclusion proof. Successful worksheet
recipe reload/general D14 rebuild preservation and independent worksheet guides
remain open. Broader control coverage, human/multiline/long-value acceptance and
the intermittent native diagnosis remain tracked in the remaining-acceptance index.

## 8. Immediate next action

Extend the existing packaged recording/guide harness to prove Admin Settings Close
with distinct source and observed button/native sequences, then evaluate and view
the authored dismissal-only conclusion in How-To, Diagnostic and Compare modes.

## 9. Critical references

- Architecture v4.11 D18 catalog32 and approved RUN-SCALE-02; Plan022; Controls1.517.
- Code `tests/integration/plan022_slice4be_remaining_acceptance.md`.
- `modAdminSettingsClose`, `modFormCloseCodes`, `ADMIN_SETTINGS_CLOSE`.
- `Slice4beAdminCloseActivity.ps1`, `Test-Slice4beAdminClose.ps1`.
- Existing `Slice4beGeneralSettingsRecorded.ps1`, `Slice4beGeneralSettingsGuidePaths.ps1`
  and shared recording/guide helpers; reuse them where appropriate.
- `frmProduction.ApplyWorksheetRunScale`, `modProductionRunScaleActions.TryLoadWorksheetRecipe`.
- `Slice4beProductionRunWorksheetScale.ps1`; unchanged frozen predecessors remain available.
