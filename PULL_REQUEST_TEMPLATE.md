# Pull Request

## Summary
<!-- What changed and why? -->

## Governing authority
<!-- Link or pointer to the controlling backlog item, decision, implementation plan, issue, or other current authority. -->

## Build admission
**Target Fit:** <!-- REUSE | DONOR-DERIVED | NEW COMPONENT | NOT YET NEEDED -->
**Chat Prebuild Disposition:** <!-- CHAT FULL PREBUILD | CHAT PARTIAL PREBUILD | DIRECT CODING EXECUTION -->

**Base SHA:** <!-- Commit SHA Chat/executor prepared against -->

### Prepared in Chat
<!-- Stable research, design, code, tests, schemas, migration/rollback steps, or other scaffold prepared upstream. Use N/A only when DIRECT CODING EXECUTION is justified. -->

### Must resolve live
<!-- Repo/runtime-dependent imports, versions, generated artifacts, environment wiring, secrets, current conventions, or other details that require live reconciliation. -->

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
- [ ] Chat scaffold was reconciled against current code/configuration/dependencies/conventions where applicable.
- [ ] No secrets were placed in scaffold or PR content.
- [ ] Relevant acceptance criteria and downstream consumers were checked.
- [ ] Rollback/disable/recovery path is understood.
