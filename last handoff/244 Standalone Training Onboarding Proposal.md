# Handoff 244: standalone Training onboarding proposal

Date: 2026-11-15 Pacific. Predecessor: handoff 243.

## Goal and release outcome

Enable the new Training warehouse hands-on 4be-A review through a supported first-use path under Architecture v4.11 D8/D18; no warehouse or human acceptance is complete.

## Current verified state

Last verified 2026-11-15: docs branch `work/perplexity-handoff218` contains proposed D8-TRAINING-ONBOARD-01 in Architecture v4.11 and pending checkpoints in Plan 022 and Controls 1.759. It is **PROPOSED, not approved or implemented**. Code PR16 branch `work/d14-packaged-chain-coverage` at `6e866f16210ac864a891a3b425e2d99001b19d1a` contains the operator review sheet and is tracked-clean. Main code checkout has Justin's unrelated `AGENTS.md` edit; docs checkout also has unrelated pre-existing edits/untracked files. Excel is closed. The ignored review candidate's five XLAM hashes matched PR4-BASE-18, and `TrainingHub` remains empty.

## Decisions and constraints

Justin chose a new disposable Training warehouse, approved a **test-only** post-create PIN and `ACTION_PATH_MAINT` grant for preview, and directed a user-side path that creates a warehouse without existing invSys credentials and secures it afterward. He selected **standalone local first**; shared/NAS credential-free creation is out of scope. Existing D8-CREATE-01 still requires captured signed-in source Admin and remains binding until the proposed exception is approved. Do not infer test-only grant as product acceptance.

## Evidence and traceability

Source: `modAdminCreateEntry.OpenFromRibbon` captures the current source context; `modWarehouseCreateCommands.CreateWarehouse` rechecks source ADMIN_MAINT. `modWarehouseBootstrap` creates the initial user with ADMIN_MAINT/RECEIVE_POST but no PIN hash; normal sign-in rejects blank hash. Users & Roles exposes six rights and cannot grant `ACTION_PATH_MAINT`. Symptom: a new user cannot create a warehouse through the approved interactive path or author a guide after current bootstrap. Governing rules: D8-CREATE-01, D8-USERS-01, D18-REPLAY-01. No behavioral RED/GREEN has run for the proposed correction.

## Do Not Repeat

Do not remove the D8 source check from the existing Create command, treat Windows/NAS identity as an invSys session, use an unsecured warehouse for operations, or count a fixture-only preview as onboarding GREEN. Do not edit or publish operational workbooks to simulate the path.

## Assumptions to Re-verify

Recheck current PR heads, Excel closure, candidate hashes and empty Training hub before any runtime setup. The first-use setup claim and pending-state design have not been approved or implemented.

## Open questions and blockers

Justin's decision on the exact proposed D8-TRAINING-ONBOARD-01 text is pending. The proposal uses a separate signed-out local Core setup command, a protected profile-bound pending claim, a later masked Secure action, ready-state gates and a Training guide right; signed-in Create/Publish retains accepted authority/results. Approval is required before D13 product work. No first-use user-side path currently exists.

## Immediate next action

After approval, mark D8-TRAINING-ONBOARD-01 approved in Architecture v4.11, synchronize Plan/Controls, then write and run a focused behavioral RED through the packaged signed-out Create and Secure handlers before implementation.

## Critical references

`0 plan docs/xlam_invSys/invSys-Design-v4.11.md` D8-TRAINING-ONBOARD-01 and D8-CREATE-01; Plan 022; Controls 1.759; code PR16; docs PR5; `tests/integration/plan022_slice4be_operator_review.md`; ignored `reports/runtime/4be-a-human-review-20261115/` candidate and local proposal.
