# Pull Request

## Summary
<!-- What changed and why? -->

## Governing authority
<!-- Link or pointer to the controlling backlog item, decision, implementation plan, issue, or other current authority. -->

## Build admission
**Acquisition Path:** <!-- REUSE | DONOR-DERIVED | NEW COMPONENT | NOT YET NEEDED. Copy/pointer to the owning Build Admission value; this PR is evidence, not a second authority. -->
**Chat Prebuild Disposition:** <!-- CHAT FULL PREBUILD | CHAT PARTIAL PREBUILD | DIRECT CODING EXECUTION -->

**Base SHA:** <!-- Commit SHA Chat/executor prepared against -->

### Prepared in Chat
<!-- Stable research, design, code, tests, schemas, migration/rollback steps, applicable D-0140 fitness baseline, reuse comparison, or other scaffold prepared upstream. Use N/A only when DIRECT CODING EXECUTION is justified. -->

### Must resolve live
<!-- Repo/runtime-dependent imports, versions, generated artifacts, environment wiring, secrets, current conventions, existing local components, or other details that require live reconciliation. -->

### Continuous fitness re-check — D-0140
<!-- For material implementation changes, after live reconciliation evaluate only the D-0140 dimensions affected by this change. Small low-risk changes should remain proportionate; do not rerun settled dimensions without a new trigger.

Initial trigger IDs:
- FIT-REUSE-01 — new material custom surface, duplication, hidden dependency, newly visible residual, or materially better reusable implementation. Reopen D-0139/D-0109 reuse comparison for the affected slice; "no donor earned" remains valid, and unrelated accepted work remains unaffected unless its owning dependency/gate requires otherwise.
- FIT-SEC-01 — dependency/lockfile, credentials, auth, permissions, network exposure, endpoint, privilege, or security-sensitive configuration change. Route the affected slice to existing security authority.
- FIT-CPLX-01 / FIT-CPLX-02 — new persistent operational component, or material abstraction/generalization beyond the current consumer. Require earned-existence/simplification review.
- FIT-AUTH-01 — source identity, ownership, canonical pointer, or duplicate-authority change/conflict. Reconcile live authority before reliance.
- FIT-REL-01 — background/async execution, persistent state, remote/irreversible mutation, retry behavior, or external dependency change. Verify bounded failure/recovery and consumer outcome.
- FIT-COST-01 — material increase in paid/premium use, recurring cadence, persistent compute/storage/network/API use, or repeated toil. Re-evaluate cheapest adequate lifecycle path.
- FIT-OBS-01 — material async/background/remote action lacks sufficient receipt/log/status/readback/consumer proof. Add the smallest sufficient evidence path or leave INCONCLUSIVE.

Record only triggered dimensions and the smallest evidence/action needed. A trigger invokes its existing authority; this PR section does not approve architecture, security posture, Build Admission, exceptions, or deployment. Use BLOCKED only when an existing governing authority makes the condition blocking.
-->

**Fitness result:** <!-- NO_TRIGGER | RECHECK | INCONCLUSIVE | BLOCKED BY EXISTING AUTHORITY -->
**Triggered IDs:** <!-- NONE | FIT-... -->
**Recheck evidence / owning authority:** <!-- N/A when NO_TRIGGER; otherwise concise pointer/result. For FIT-REUSE-01, reconcile any material Acquisition Path change before relying on new external code. -->

### Direct-execution reason
<!-- Required only for DIRECT CODING EXECUTION. Explain why live repo/runtime state materially dominates or Chat scaffolding would add rework. -->

## Verification
<!-- Tests, CI, runtime checks, consumer checks, or evidence completed. -->

## Rollback / disable / recovery
<!-- How this change can be backed out, disabled, or recovered if needed. -->

## Acceptance status
<!-- NOT READY | READY FOR REVIEW | ACCEPTED. Acceptance evidence must come from the applicable governing process, not from this template itself. -->

## Checklist
- [ ] Live repository/runtime state was re-read immediately before mutation.
- [ ] Chat scaffold was reconciled against current code/configuration/dependencies/conventions and existing local components where applicable.
- [ ] When an implementation/acquisition decision is in scope, the prebuild reuse comparison is recorded in the owning Build Admission evidence or controlling pointer.
- [ ] Applicable D-0140 trigger checks were evaluated from the current change/runtime evidence; only affected dimensions were reopened.
- [ ] Triggered rechecks were routed to their existing owning authority; no fitness result self-approved a material decision.
- [ ] Any material Acquisition Path/current-state change was reconciled in its owning evidence before reliance.
- [ ] No new policy/scanner/workflow/control plane was introduced merely to satisfy this template.
- [ ] No secrets were placed in scaffold or PR content.
- [ ] Relevant acceptance criteria and downstream consumers were checked.
- [ ] Rollback/disable/recovery path is understood.
