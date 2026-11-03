# RACE PHASE 1 MANIFEST SCHEMA

## 1. Purpose

Define the required manifest accompanying controlled implementation under an approved Phase 0 baseline.

The manifest records what was authorized, what was changed, how changes were performed, and what must be independently verified in Phase 2.

## 2. Required Identity Fields

- RACE campaign identifier.
- Mission identifier.
- Target system, repository, or subject.
- Manifest version.
- Creation date and time.
- Responsible operator or AI system.
- Phase designation: PHASE_1.
- Manifest status.
- Reference to the accepted Phase 0 manifest.

## 3. Approved Baseline

Record:

- Approved objective.
- Approved scope.
- Explicit exclusions.
- Accepted Phase 0 findings.
- Implementation requirements.
- Acceptance criteria.
- Dependencies.
- Known limitations.
- Required approvals.

Any change to the approved baseline must be documented.

## 4. Expert Panel

Record all three mandatory permanent seats. No seat may be
omitted, replaced, or silently substituted.

For EACH permanent seat, record:

- Expert ID.
- Canonical expert name.
- Identity formalization status.
- Identity version, if established.
- Identity approval status.
- Capability-library formalization status.
- Capability-library version, if established.
- Capability approval status.
- Capability performance-validation status.
- Operating-doctrine version and status, if established.
- Functional mission assignment.
- Selected capability IDs and names, where applicable.
- Participation evidence and actual contribution.
- Known limitations and specialist dependencies.

Current UCO baseline, subject to verification against the current
registry and version manifest:

- UCO-001 — Universal Chief Officer.
- Identity v1.0: APPROVED.
- Capability library v1.0: APPROVED.
- Operating doctrine v1.0.
- Performance validation: NOT PERFORMED.

The Hacker and MacG currently have permanent panel seats, but their
canonical identities and capability libraries are NOT YET FORMALIZED.
Record those gaps explicitly. Do not invent versions, capabilities,
approval, or validation status.

For every selected capability, regardless of which permanent or mission-specific expert owns it, identify the owning expert by ID and name, then record all seven fields:

1. Capability ID.
2. Capability name.
3. Applicable mission question.
4. Expected analytical contribution.
5. Relevant evidence requirements.
6. Known limitations.
7. Specialist dependency.

Capability selection does not prove exercise, demonstration, or success.
Record actual exercise and supporting evidence separately.

Also record:

- Mission snapshot ID/reference.
- Exact assembled expert content or immutable references.
- Prompt version/hash, if available.
- Additional mission-specific experts and justification.
- Material disagreements and unresolved objections.
- Known identity, capability, validation, and specialist gaps.
- Whether expert perspectives were simulated in one execution or
  separately executed. Do not claim independent execution without evidence.

The permanent seats cannot be removed or replaced.

## 5. Authorization Register

For each authorized action, record:

- Authorization identifier.
- Action description.
- Authorized scope.
- Approving human.
- Approval reference.
- Approval date and time.
- Applicable restrictions.

Permitted action categories:

- INSPECT
- ANALYZE
- RECOMMEND
- PREPARE
- MODIFY
- COMMIT
- PUSH
- DEPLOY
- EXTERNAL ACTION

Authorization for one category does not imply authorization for another.

## 6. Implementation Plan

Record:

- Planned changes.
- Target files, components, or systems.
- Dependencies.
- Expected behavior.
- Implementation sequence.
- Rollback or recovery considerations.
- Verification requirements.

## 7. Implementation Record

For each material change, record:

- Change identifier.
- Description.
- Target.
- Before state.
- After state.
- Execution evidence.
- Related authorization.
- Deviations from plan.
- Result.

Distinguish proposed, prepared, and actually executed changes.

## 8. Testing and Adversarial Controls

Record:

- Tests planned.
- Tests executed.
- Commands and environments.
- Results.
- Failures.
- Skipped tests.
- Untested areas.
- Adversarial checks performed.
- Remaining vulnerabilities or weaknesses.

Use the evidence classifications:

- EXECUTED
- INSPECTED
- INFERRED
- UNKNOWN

## 9. Deviations and Outstanding Issues

Record:

- Baseline deviations.
- Unapproved or blocked changes.
- Unexpected behavior.
- Unresolved defects.
- Deferred work.
- Additional authorization required.

Unauthorized changes must not be represented as approved work.

## 10. Phase 1 Completion Status

Permitted values:

- DRAFT
- IN_PROGRESS
- COMPLETE
- BLOCKED
- REJECTED

COMPLETE requires implementation records, authorization references, test results, documented deviations, and a Phase 2 handoff.

Completion does not mean the implementation has passed independent verification.

## 11. Phase 2 Handoff

Record:

- Implemented baseline.
- Changed components.
- Change evidence.
- Authorization references.
- Test results.
- Known defects.
- Untested areas.
- Adversarial verification targets.
- Acceptance criteria.
- Outstanding risks.

## 12. Governing Rule

Phase 1 executes only authorized work. Its own implementation claims are not substitutes for independent Phase 2 verification.
