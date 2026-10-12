# Directory preservation and native projection blocker

## 1. Goal and release outcome

Complete 4be-A recording/Viewer/How-To and approved early B0 under v4.11/Plan 022,
then stop before broader 4be-B. Goal remains active/incomplete. View Warehouses
needs a D14 preservation prerequisite before its recording coverage.

## 2. Current verified state

Last verified 2026-10-12, 14:54 UTC. Both branches are main: code `4e80a39e`
(pushed); docs `13ece3a` before this handoff. Controls1.546; catalog36/156 unchanged.
Code is clean. Preserve unrelated docs: old024 deletion,067 edit and untracked
023/024REPORT/025. Their four existing file hashes were checked unchanged.

Unpromoted candidate `deploy/validation-admin-directory-01`; pins and compiled
comparison in `reports/runtime/admin-directory-build-01`. Only modAdminConsole's
two directory procedures change; one small row helper is added. The other106
procedures and328 compiled components are unchanged. Prior console-03 is frozen.

Excel and all owned test controllers are closed; settings/reports restored.
The desktop monitor stopped normally:14:14:32–14:53:32 UTC,467 samples, zero
cursor/desktop/capture/error5 failures. These passive reads do not prove mouse
movement. Restart monitoring before further UI work.

## 3. Decisions and constraints

D14 directory enforcement: clear managed fields and reuse rows; preserve unknown
cells/formulas/headers/positions, including local cells beyond current results.
Keep discovery order, deduplication and no-results wording. No new warehouse
identity, annotation association, recording ID or authority contract was added.

D18-LOCAL-01 remains proposed/unapproved. Do not change NAS-only context/activity/
journal gates or separate replay eligibility. View Warehouses recording is pending.

On desktop Win32 error5: timestamp, stop runtime, retain cleanup/restoration,
handoff/commit/push and exit. VBA/native crashes differ. Excel serial; no build
while open, force-kill, recovery COM attachment or desktop rebinding. Never edit
pinned tooling during a live controller. Preserve exact System_Key, unknown
columns, captured binding, all accepted GREENs and unrelated changes.

## 4. Evidence and traceability

Canonical receipt: code `tests/integration/plan022_slice4be_admin_directory_columns_results.md`.

- Actual View Warehouses Ribbon: initial19/2 RED, expanded26/4 -> GREEN31,
  exact30-check prefix. Normal/empty/restored discovery, saved authority and
  unknown cells pass. One generated local-cell capture reviewed.
- Five cold/instrumented compiles, Operations cold start, Console118 and smoke86
  pass with pins/restoration/clean delayed audits; smoke has two unassisted exits.
- Static01:337 components/6412 procedures/139745 lines, all28 caps without growth,
  dynamic9/45, duplicates194, three schemas and492 parsed scripts. No exception.
- Settings202 and Console188/Verify202/Reconcile360 guide baselines are explicitly
  reused through compiled/procedure comparison; they are not fresh full reruns.
- Ordinary chain1:5/1, live32/1, Create15; ntdll/c0000028 during projection recovery.
  Chain2:32/32, live48/48, Create15, but combase/c0000005 in its native audit.
  Neither is accepted. First recovery used normal WM_CLOSE, no force-kill/COM attach.
- Existing trace protection74/74. Traced chain again5/1, live32/1, Create15.
  Owner/start-time matching identifies LiveRole.excel at14:48:26.6774796Z;
  last boundary is Projection.31 / modProcessor.RunBatchReportForAutomation,
  immediately after projection deletion. Native cause inside VBA remains unknown.
  Owned recovery closed normally; settings/reports/packages preserved.
- Narrow AfterProjection/Setup Chain/TraceBoundaries diagnostic fails installation
  at modInventorySchema.EnsureTableWithHeaders.7, before business checks/compiles.
  It is not product RED. Clean normal closure and zero native events through
  14:51:40.9293918UTC. Source contains `lo.Name = tableName`; matcher uses ordinal
  case-sensitive comparison. Compiled casing is a hypothesis, not verified cause.

## 5. Do Not Repeat

Do not credit all-GREEN assertions when the same interval has a native crash.
Do not rerun broad chains without a diagnostic purpose. Earlier native localization
already tried deleted-table/local-reference release; the current validator includes
the deleted-table cleanup. Read that receipt before repeating it. Copied-fixture
replay previously needed an expired lock lease; never reset/bypass the lease.

The first expanded directory test had an off-by-one message comparison; the
corrected26/4 supersedes it. Formula survival was always GREEN, not a defect claim.
Recovery process start times from CIM and Get-Process differed by one tick;
validate each API's actual timestamp rather than weakening ownership guards.

## 6. Assumptions to Re-verify

Desktop access, closed Excel, package pins, Git states and any D18-LOCAL-01 reply.
Check the actual compiled anchor spelling/count before changing trace matching.
No native crash is claimed fixed and no clean chain exists on directory-01.

## 7. Open questions and blockers

Native full-chain qualification blocks this prerequisite's acceptance. The narrow
trace's installation mismatch currently blocks deeper localization. Remaining
Admin recording/local eligibility still block 4be-A; no goal completion claimed.

## 8. Immediate next action

Protect and diagnose the compiled projection-trace anchor matcher with a focused
test before correcting tooling and repeating the existing AfterProjection control.

## 9. Critical references

- v4.11 D14 directory clarification; Plan022; Controls1.546.
- `ProjectionBoundaryTrace.ps1`, `Test-Slice4beProjectionLiveControl.ps1`.
- Focused root `reports/runtime/projection-live-control/b4fd39bcecd84d099ee747f8e33bc862`.
- Trace `reports/runtime/admin-directory-native-trace-01`; controller
  `admin-directory-native-regression/chain-157975d59bcc4da8acd9a03cc87014f6`.
- `tests/integration/plan022_slice4be_native_localization_results.md`, especially
  deleted-table cleanup/ordinary-chain limits; directory receipt has exact run IDs.
- After qualification: D18 View Warehouses scope must preserve original open-Config/
  scan-root inputs before optional observation and the existing optional root prompt.
  Its presentation is not target selection, creation or exhaustive discovery.
