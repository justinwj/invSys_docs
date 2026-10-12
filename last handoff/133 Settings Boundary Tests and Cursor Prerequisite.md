# Settings boundary tests; native cursor prerequisite unresolved

## 1. Goal and release outcome

Complete4be-A recording/Event Viewer/How-To authoring and approved early B0 under
v4.11/Plan022; stop before broader4be-B. **4be-A remains incomplete.** This checkpoint
adds Settings tab boundary tests, without a runtime or architectural change.

## 2. Current verified state

Last verified:2026-10-12,02:32 UTC. Both branches main. Code `e92b5693` is pushed;
docs base `8b26929`, with synchronized evidence/Controls1.523 and this handoff in
the following docs commit. Candidate remains `deploy/validation-admin-entry-02`,
catalog33/151, byte-identical to prior GREEN. No rebuild or promotion.
Excel, all test controllers and passive monitor are closed. Monitor02:18:01-02:31:54
recorded166 samples, zero cursor/desktop/capture failures and zero error5.

Preserve user-owned docs: modified handoff067, deleted old024 Delivery Overrun,
untracked023 Critique,024 REPORT and025 GUIDANCE. Raw runtime artifacts remain ignored.

## 3. Decisions and constraints

All prior approvals remain, including RUN-SCALE-01/02, RUN-UI-01 and D18-REPLAY-01.
Catalog33 specification/permissions remain unchanged. New tests cannot manufacture
behavioral RED from fixture or native-input failure. Never aggregate partial runs
into GREEN. Preserve prior launcher24/tab43, Close70, Settings202 and smoke86 evidence.
Actual Win32error5 requires timestamp, runtime stop, owned cleanup and exit. A
successful SetCursorPos with unexpected coordinates is a different diagnosis.
Run Excel jobs serially; qualify delayed events before another. No force-kill,
COM recovery reattachment or desktop rebinding. User mouse interference is unconfirmed.

## 4. Evidence and traceability

New switch: `Test-Slice4beAdminSettingsEntry.ps1 -Navigation -NavigationFailures`.
The expanded gate covers defaults/disabled/user/control policy, current policy on
an open form, repeated activation, target/sign-out, same-session permission loss,
older policy, storage notice and preservation. It is **not accepted**.

Exact controllers/workers and classifications are in code
`tests/integration/plan022_slice4be_admin_entry_results.md`:
- 170/5: disabled fixture incorrectly set Collect=True; corrected, not runtime RED.
- 95/1: cursor prerequisite; original message ambiguously combined read failure
  and unexpected coordinates.
- 58/1: improved helper confirms SetCursorPos success and successful coordinate
  read returning the original position at02:29:24.9347374Z (7:29:24 PM Pacific).

All attempts preserve settings/packages, close Excel normally and pass delayed
native audits. Standalone diagnostic plus12 bounded small/large moves pass with
matching input/thread desktops, exact target/restoration and unchanged display/clip
bounds. They do not prove the failed worker's thread state. No error5 observed.
Static `admin-navigation-boundary-static-01/ratchet-verification.json`: all28 caps,
326 components/6371 procedures/139227 lines, dynamic9/45 and192 duplicates unchanged;
three schemas and466 PowerShell scripts validate.

## 5. Do Not Repeat

Do not retry the full Excel gate solely because a separate cursor probe passes.
Capture evidence in the failing helper before changing input behavior. Do not weaken
the exact-position guard, treat successful API return as movement, or equate passive
desktop reads with working input. Posted nested-tab clicks were already disproven;
retain owned SendInput and native event/destination prerequisites.

## 6. Assumptions to Re-verify

Recheck Git/pins, Excel closure and desktop access. Restart the passive monitor for
UI work. Ignored diagnostic scripts need inspection before reuse. No response yet
to whether the user moved the mouse around7:27 PM; do not infer an answer.

## 7. Open questions and blockers

Cursor success/unexpected-position cause remains unresolved; same-helper desktop,
clip/display bounds and immediate-versus-delayed reads were not captured at failure.
Expanded tab GREEN, public-launcher negative cases, active capture, publication and
independent guide proof remain open. Wider4be-A controls/layout/human gates and
the prior intermittent Shipping Sent native chain failure remain unchanged.

## 8. Immediate next action

Instrument the native tab helper to capture its own desktop, bounds and immediate/
delayed cursor facts on mismatch, retaining fail-before-click behavior, before another Excel run.

## 9. Critical references

- v4.11 D18 Settings entry/navigation refinement; Plan022; Controls1.523.
- Code `plan022_slice4be_admin_entry_results.md`, `plan022_slice4be_remaining_acceptance.md`; handoff132 for prior qualified GREEN.
- `Slice4beAdminSettingsNavigation.ps1`, new `Slice4beAdminSettingsNavigationFailures.ps1`, `Slice4beAdminSettingsEntry.ps1` and its controller/Config worker.
- `tools/diagnose-cursor-handoff.ps1`; ignored `reports/runtime/diagnose-navigation-cursor.ps1`, `diagnose-navigation-cursor-sequence.ps1` and their receipt roots in the results record.
