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
<!-- Stable research, design, code, tests, schemas, migration/rollback steps, reuse/donor comparison, or other scaffold prepared upstream. Use N/A only when DIRECT CODING EXECUTION is justified. -->

### Must resolve live
<!-- Repo/runtime-dependent imports, versions, generated artifacts, environment wiring, secrets, current conventions, existing local components, or other details that require live reconciliation. -->

### Continuous reuse re-check — D-0139
<!-- Reuse-first continues during implementation; it is not frozen at prebuild.

1. State the prebuild reuse basis or point to the Build Admission receipt: existing VLS code, native/framework capability, package/tool/platform reuse, and any bounded donor candidates checked.
2. After re-reading the live repo/runtime, explicitly evaluate whether implementation exposed any reopen trigger:
   - duplicated commodity logic;
   - hidden dependency or existing local component;
   - unexpectedly large custom surface;
   - repeated adapter/auth/pagination/retry plumbing;
   - a new machine-observable residual; or
   - a materially better maintained reusable implementation.
3. If a trigger fired, record the bounded re-comparison and whether the owning Acquisition Path changed. Reconcile Build Admission before relying on newly selected external code.
4. If no trigger fired or no donor/reuse candidate earned selection, say so. "No donor earned" is a valid result.

Do not pause every coding step for broad external research, and do not manufacture a donor merely to satisfy this section.
-->

**Build-time reuse disposition:** <!-- NO REOPEN TRIGGER | RECHECKED / PATH UNCHANGED | RECHECKED / PATH CHANGED — see owning Build Admission evidence -->

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
- [ ] Prebuild reuse comparison is recorded in the owning Build Admission evidence or controlling pointer.
- [ ] D-0139 build-time reuse triggers were evaluated after live reconciliation.
- [ ] If a reuse trigger fired, the bounded alternatives were re-compared and any material Acquisition Path change was reconciled before relying on new external code.
- [ ] No secrets were placed in scaffold or PR content.
- [ ] Relevant acceptance criteria and downstream consumers were checked.
- [ ] Rollback/disable/recovery path is understood.
