# Create contract review tightened

## 1. Goal and release outcome

Complete4be-A and early Receiving B0 under v4.11/Plan022; Create New Warehouse
owner authorization precedes recording. **4be-A remains incomplete.**

## 2. Current verified state

Last verified2026-10-13: both branches `main`; code54e069f2 pushed, docs base0721419
before this proposal/handoff commit. This turn changes documentation only; no
Excel, desktop automation, test run or build was started. Qualified unpromoted
root-recording-04/catalog40/162 remains unchanged. Recheck Excel before a build.
Preserve unrelated docs: modified067, deleted old024, untracked023/024REPORT/025.

## 3. Decisions and constraints

D8-CREATE-01 remains **PROPOSED, approval pending**, now incorporating user review:
explicit reopened **Publish Existing Warehouse** validates/binds the existing
runtime and uses the new session without bootstrap or local Config/Auth/inventory
rewrites; ordinary Create still refuses duplicates. ADMIN_MAINT belongs to the
captured source warehouse; check after confirmations immediately before writes.
No Windows/Office identity substitute. Use typed calls/primitive envelopes and
redact recording/activity/all logs, including downstream diagnostics.
Plan022 and Controls1.572 are synchronized. No implementation approval inferred.
Continue in ordinary turns; stop for approval, desktop error5 or mouse lock.
All earlier architectural, preservation and native-lifecycle constraints remain.

## 4. Evidence and traceability

Prior owner RED45/2, five compiles, preservation and native audit are detailed in
`tests/integration/plan022_slice4be_admin_create_owner_results.md` and handoff172.
They are unchanged historical evidence, not proof of the expanded contract.
This documentation revision passed diff/whitespace and reference review only.

## 5. Do Not Repeat

The current owner probe already invokes Core SignOut before Create (line182) and
checks IsSignedIn=False. It lacks a wider state matrix and confirmation-time hook.
Reuse the existing Users diagnostic `SignedOut` state and Close activity `SignedOut`
mode for expansion; do not describe sign-out-before-Create as missing coverage.

## 6. Assumptions to Re-verify

Desktop input, Excel absence, Git/package pins and user approval before automation.
Do not infer reopened publication from the same-instance retry test.

## 7. Open questions and blockers

Await approval of revised D8-CREATE-01. Expanded RED, implementation, recording,
guide conclusions and remaining4be-A acceptance are still pending.

## 8. Immediate next action

After approval, expand packaged RED for reopened publication, source/destination
authority, post-confirmation context loss and redaction before changing product code.

## 9. Critical references

- v4.11 D8-CREATE-01; Plan022; Controls1.572; owner receipt above; handoff172.
- `Test-Slice4beAdminCreateWarehouseOwner.ps1`, `Slice4beAdminCreateWarehouseOwner.ps1`.
- `Slice4beAdminAuthWriteDiagnostic.ps1`, `Slice4beAdminCloseActivity.ps1`.
