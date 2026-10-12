# Source-loading chain and station proposal

## 1. Goal and release outcome

Complete 4be-A recording/Viewer/How-To and approved early B0 under v4.11/Plan022,
then stop before broader4be-B. Goal active/incomplete. This turn made progress:
broader controls support an explicit station-prerequisite proposal; no acceptance
gate has been waived and no native root cause is claimed repaired.

## 2. Current verified state

Last verified2026-10-12,15:52UTC. Main branches: code `e98e3ca8` and docs `24ba752`
(before this handoff), pushed. Controls1.548; catalog36/156 unchanged. Code clean.
Preserve unrelated docs: old024 deletion,067 edit and untracked023/024REPORT/025.

Unpromoted directory-01 and frozen console-03 package pins remain unchanged.
No product code or station implementation changed. Excel and owned controllers
are closed; settings/reports restored. `ForceVBALoadFromSource` is absent again.
No actual station registration or periodic task was changed.

Desktop monitor stopped normally15:22:32-15:51:11UTC:343 samples, zero cursor,
desktop, capture or error5 failures. Passive reads are not mouse-movement proof.
Restart monitoring before runtime work.

## 3. Decisions and constraints

**D16-VBA-LOAD-01 is PROPOSED, not approved.** Approval question was sent this turn;
no reply received. v4.11 line168, Plan022 and Controls1.548 are synchronized.
It proposes consented account-wide VBA source loading before Excel starts,
StationSetup establishment/restoration and updater verification. All existing
qualification gates remain. Do not implement or enable a permanent setting before
approval; do not silently treat diagnostic success as release acceptance.

**D18-LOCAL-01 also remains proposed/unapproved.** Preserve NAS-only recording/
library gates and separate replay eligibility. View Warehouses recording is pending.

On desktop Win32 error5: timestamp, stop runtime, retain owned cleanup/restoration,
handoff/commit/push and exit. No force-kill, recovery COM attachment, desktop
rebinding, or build with Excel open. Preserve unrelated changes, exact System_Key,
unknown columns, captured binding, headless authority and all accepted GREENs.

## 4. Evidence and traceability

Canonical receipt: code `tests/integration/plan022_slice4be_admin_directory_columns_results.md`.
It retains directory RED26/4 -> GREEN31, Console118/smoke86, compiles/capture,
guide reuse, trace RED7/4 -> GREEN11/existing74 and static02/493 parsers.

- Temporary source-loading full live control:48/48, exact original order, normal
  closure and zero native events through15:25:25.5513872UTC. Option restored.
- Ordinary frozen console-03 control:32/1 at processor after projection deletion;
  owner/start-matched ntdll/c0000028 at15:27:26.9820905UTC. Thus the failure is not
  unique to the directory edit. Its historical clean runs remain historical facts.
- Recovery opened current and earlier test copies. Read-only registry metadata
  identified all19 entries as exactly two generated test folders. Reviewed UIA
  actions discarded only those recovered copies. All25 saved original fixture
  files retain identical hashes. No COM attachment/force termination. Controller
  restoration completed; delayed audit through15:34:55.5737854UTC has two events.
- Temporary source-loading full chain:32/32, live48/48, Create15/15, exact prior
  order. Restart reconciliation, runtime-five-package and static gates execute.
  Normal unassisted closure; zero native events through15:43:20.8613671UTC;
  option absence restored15:43:20.9518291UTC. Packages/settings/reports preserved.
  Only chain derivation change is ephemeral fixture-credential generation before
  writing the ordered validator; synthetic payload assertions remain intact.
- Existing StationSetup9/9 baseline exercises actual published NAS bootstrap,
  installer and updater with disposable feed/cache/test-registry. The diagnostic
  copy adds a resolved scratch-cleanup guard only. No periodic task requested.

These are diagnostics/baselines, not new product RED/GREEN or adopted configuration.

## 5. Do Not Repeat

The old close helper recognizes bosa/#32770 but misses NUIDialog. Do not send
repeated WM_CLOSE while any modal dialog exists. Fifteen initial requests caused
stacked notices; subsequent actions inspected exact prompts/origins individually.
Never discard a recovery copy based merely on a generic inbox filename.

Source loading affects all VBA workbooks in the account. It is an explicit new
prerequisite proposal, not a hidden harness fix. Earlier save/recompile-before-save,
relocation, timing and Domain-substitution experiments did not prove a durable fix.
Two hidden Excel processes during later full-chain gates exited naturally; a quiet
log or observation timeout is not terminal/hang evidence.

## 6. Assumptions to Re-verify

Approval replies, desktop, closed Excel, package pins, registry option absence and
Git state. Excel version verified16.0.20430.20146. Do not infer a current Microsoft
bug diagnosis from the historical Excel2016 source-loading article.

## 7. Open questions and blockers

D16-VBA-LOAD-01 approval and implementation are pending. Ordinary native qualification
remains open. D18-LOCAL-01 and remaining Admin recording/visible gates still block
4be-A. No requested deliverable is dropped because source-loaded diagnostics pass.

## 8. Immediate next action

Resolve D16-VBA-LOAD-01 approval; if approved, synchronize the approval record and
run a focused actual StationSetup/updater RED for unconsented activation and the
missing source-loading prerequisite before implementation.

## 9. Critical references

- `tools/install_invsys_station_from_nas.ps1`, `start_invsys_nas_station_setup.ps1`,
  `update_invsys_station.ps1`, `invsys_release_common.ps1`, publisher/registration;
  `tests/tooling/Test-Plan022Slice4bjNasStationSetup.ps1` is the existing9 baseline.
- Updater currently restores a whole Excel-options snapshot on failure. Protect
  concurrent source-option changes through that real handler; an installer-only
  finally block cannot guarantee preservation. Never re-enable the disabled updater
  task during these tests. Use isolated registry/cache/feed parameters.
- Ignored source full-chain proof:
  `admin-directory-source-chain/chain-bb2392bf91194743a82782404d5c9c1d/qualified-verification.json`;
  option controller `chain-source-load/a5b665ae6360484c86a3db28b8a1714b`.
- `reports/runtime/PrepareSourceLoadChain01.ps1`, `TestChainSourceLoad01.ps1`,
  `TestStationSetupBaseline01.ps1`; full comparison IDs are in the canonical receipt.
- After qualification, View Warehouses recording must preserve original open-Config/
  scan-root scope and optional root prompt; presentation is not target selection.
