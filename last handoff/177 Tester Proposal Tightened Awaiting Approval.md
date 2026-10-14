# Tester proposal tightened, awaiting approval

## 1. Goal and release outcome

Complete4be-A including early Receiving B0 under v4.11/Plan022; broader4be-B and
full Release1 acceptance remain separate. Goal remains paused for proposal approval.

## 2. Current verified state

Last verified2026-10-13 Pacific: both branches `main`; code `23de4e59`, docs base
`c2510347` before this documentation-only revision. No runtime or test edits.
Qualified candidate remains create-recording-02, catalog41/172. User-modified
`AGENTS.md` adds the explicit error5/mouse-lock/approval exit rule; preserve it
uncommitted. Preserve unrelated docs: modified067, deleted old024, untracked023/
024REPORT/025. No desktop/Excel automation ran this turn; recheck before any build.

## 3. Decisions and constraints

The user requested six tightenings **before approving** D8-TESTER-01. They are now
in the normative proposal, Plan022 and Controls1.576; approval is still pending:

- Receipt binds immutable provisioning Core user/session-generation provenance;
  reopened/different-Admin access requires fresh authority at the recorded source.
- Confirmation, folder/container-resolution dialogs, prompts/popups, event pumping
  and asynchronous/external waits are explicit yield points; no new UI is authorized.
- Container-combination/nested/stale-path results use fixed redacted outcomes.
- Setup refuses already-open external/borrowed Config/containers, clean or dirty;
  current-command-owned workbook lifecycle remains valid.
- Setup refuses unmarked conflicting, nonempty or already-published destinations.
- Checks include reservation/provisioning/rename/seed/publication, cleanup deletion,
  read-only post-cleanup verification and receipt finalization. Lost scope prevents
  success and receipt removal; empty-destination eligibility precedes first reservation.

Approval authorizes D13 implementation only. D18-REPLAY-01 B0 boundaries remain
intact; no new recording control ID, runtime implementation or acceptance is claimed.
Exit Goal mode/prompt for error5, actual mouse lock or required proposal approval.

## 4. Evidence and traceability

Unchanged packaged cleanup diagnostic:25 PASS/4 expected FAIL, controller
`admin-tester-owner-controller/077e6f9d746c458ab37b5eeb0c904de6`. Real deletion
survives sign-out, Reader sign-in, warehouse switch and confirmation-time sign-out.
Five instrumented compiles and preserved pins/settings/normal shutdown passed;
prior delayed audit reported zero Excel events. These are earlier results, not reruns.
This turn checks document consistency, diff whitespace and pointer/reference validity.

## 5. Do Not Repeat

Do not treat immutable creator generation as a reusable grant or prohibit legitimate
reopening solely because the old session ended. A form/name/receipt alone grants no
authority. Map reachable yields to tests; absent dialogs are inapplicable, not covered.

## 6. Assumptions to Re-verify

Explicit approval, desktop input, Excel absence, Git state and frozen package pins.
The prior canary diagnostic proves deletion behavior, not Setup or new receipt semantics.

## 7. Open questions and blockers

D8-TESTER-01 remains proposed, approval required. Setup/ownership RED expansion,
implementation and qualification precede Tester recording. Remaining Admin coverage,
visible acceptance and early B0 remain open;4be-A is incomplete.

## 8. Immediate next action

After explicit approval, synchronize its status in the three authorities and expand
packaged RED for the six tightened requirements before changing implementation.

## 9. Critical references

- v4.11 D8-TESTER-01, D8-A, D8-CREATE-01, D18-REPLAY-01; Plan022; Controls1.576.
- `Test-Slice4beAdminTesterSetupOwner.ps1`, `Slice4beAdminTesterSetupOwner.ps1`.
- `frmSetupTesterStation`, `modTesterSetup`; code diagnostic receipt
  `tests/integration/plan022_slice4be_admin_tester_owner_results.md` and coverage map.
