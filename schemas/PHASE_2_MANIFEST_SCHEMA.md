# RACE PHASE 2 MANIFEST SCHEMA

## 1. Purpose

Define the required manifest accompanying independent verification, adversarial retesting, acceptance assessment, and campaign closure.

The manifest establishes what was verified, what failed, what remains unresolved, and whether the mission meets its acceptance criteria.

## 2. Required Identity Fields

- RACE campaign identifier.
- Mission identifier.
- Target system, repository, or subject.
- Manifest version.
- Creation date and time.
- Responsible operator or AI system.
- Phase designation: PHASE_2.
- Manifest status.
- References to accepted Phase 0 and Phase 1 manifests.

## 3. Verification Baseline

### 3.1 Independent Verification Record

Record:

- Implementer identity and role.
- Verifier identity and role.
- Whether the verifier participated in implementation.
- Whether the verifier belongs to the same team or reporting structure.
- Whether the verifier used the same AI execution or merely a separate perspective within it.
- Any personal, organizational, financial, or other conflicts.
- Separation measures applied to protect verification independence.
- Evidence independently obtained or reproduced by the verifier.
- For each verification activity, classify it as:
  - Independently designed and executed by the verifier.
  - Independently executed by the verifier against the relevant system or evidence.
  - Independently reproduced by the verifier.
  - Reviewed only from Phase 1 test results, claims, or artifacts.
  - Not performed.
- Identify the evidence, artifacts, test results, or records supporting each classification.
- Identify the AI system/model and execution or session context used by the implementer and verifier, where applicable.
- Limitations affecting independence.
- Independence determination and supporting rationale.

Permitted independence determinations:

- INDEPENDENT
- LIMITED
- NOT INDEPENDENT
- UNKNOWN

A separate expert perspective, separate prompt section, or claimed agent
persona does not by itself establish independent verification. Disclose
when verification relies on the implementer's own claims or evidence.

Independence rules:

- The same person or the same AI execution reviewing its own implementation
  is self-review, not independent verification.
- A separate invocation, prompt, model, or expert persona does not by itself
  establish independence.
- INDEPENDENT requires evidence that the verifier was sufficiently separated
  from implementation and independently obtained, executed, or reproduced
  the relevant verification evidence.
- LIMITED applies when some meaningful separation exists but material
  dependencies or restrictions remain.
- NOT INDEPENDENT applies to self-review or verification without sufficient
  separation.
- UNKNOWN applies when the available evidence cannot establish the degree
  of independence.


Record:

- Approved Phase 0 requirements.
- Phase 1 implementation baseline.
- Authorized scope.
- Expected behavior.
- Acceptance criteria.
- Known limitations.
- Required adversarial tests.
- Authorization references for verification activities.
- Explicit approval for destructive, intrusive, or external testing.
- Restrictions on test scope and permitted environments.

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

## 5. Verification Evidence

For every verification activity, record:

- Verification identifier.
- Requirement or claim being tested.
- Test method.
- Environment.
- Source or artifact examined.
- Execution evidence.
- Result.
- Limitations.
- Evidence references.

Use the classifications:

- EXECUTED
- INSPECTED
- INFERRED
- UNKNOWN

## 6. Requirement Status

Every applicable requirement must receive exactly one status:

- PASS
- FAIL
- PARTIAL
- NOT TESTED
- NOT APPLICABLE

Each status must include an explanation and supporting evidence or a documented reason why evidence is unavailable.

## 7. Adversarial Retesting

Record:

- Attack or failure scenario.
- Targeted weakness or assumption.
- Test method.
- Execution result.
- Evidence.
- Exploitability or impact.
- Remaining exposure.
- Recommended disposition.

A previously identified weakness is not considered resolved solely because a change was made.

## 8. Defects and Residual Risk

Record:

- Defect identifier.
- Description.
- Severity or impact.
- Evidence.
- Affected requirements.
- Resolution status.
- Residual risk.
- Required follow-up.

## 9. Acceptance Assessment

Record:

- Acceptance criterion.
- Applicable requirement.
- Evidence references.
- Result.
- Outstanding conditions.
- Rationale.

Permitted overall assessment values:

- ACCEPTED
- ACCEPTED WITH CONDITIONS
- REJECTED
- INCONCLUSIVE

Acceptance must not conceal failed, partial, or untested requirements.

## 10. Campaign Closure Status

Permitted values:

- DRAFT
- IN_PROGRESS
- COMPLETE
- BLOCKED
- REJECTED

COMPLETE requires a documented acceptance assessment, disposition of outstanding findings, and an explicit closure decision.

Campaign closure does not authorize deployment, publication, or other external actions.

## 11. Final Handoff

Record:

- Verified capabilities.
- Failed requirements.
- Partially verified capabilities.
- Untested areas.
- Residual risks.
- Accepted limitations.
- Deferred recommendations.
- Required future actions.
- Explicit closure decision.

## 12. Governing Rule

Phase 2 evaluates evidence against requirements. It must not treat implementation claims, documentation, or prior phase completion as proof of successful operation.
