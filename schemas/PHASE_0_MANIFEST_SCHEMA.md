# RACE PHASE 0 MANIFEST SCHEMA

## 1. Purpose

Define the required manifest accompanying every Phase 0 discovery, investigation, adversarial analysis, and architectural blueprint.

The manifest establishes what was examined, what was found, what remains unknown, and what is proposed for Phase 1.

## 2. Required Identity Fields

- RACE campaign identifier.
- Mission identifier.
- Target system, repository, or subject.
- Manifest version.
- Creation date and time.
- Responsible operator or AI system.
- Phase designation: PHASE_0.
- Manifest status.

## 3. Mission Definition

- Human-stated objective.
- Intended outcome.
- Scope.
- Explicit exclusions.
- Known constraints.
- Available resources.
- Success criteria.

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

## 5. Discovery and Evidence

Record:

- Sources examined.
- Files, systems, and interfaces inspected.
- Tests or commands executed.
- Execution results.
- Evidence references.
- Unavailable sources.
- Inspection limitations.

Every material claim must use one classification:

- EXECUTED
- INSPECTED
- INFERRED
- UNKNOWN

## 6. Findings

Each finding must include:

- Finding identifier.
- Description.
- Supporting evidence references.
- Confidence or verification status.
- Impact.
- Relevant risks.
- Contradictions or limitations.

## 7. Adversarial Analysis

Record:

- Threats and attack surfaces examined.
- Assumptions challenged.
- Failure scenarios.
- Identified weaknesses.
- Unresolved attack paths.
- Recommended mitigations.

## 8. Architecture and Recommendations

Record:

- Existing architecture.
- Proposed architecture.
- Alternatives considered.
- Dependencies.
- Integration boundaries.
- Trade-offs.
- Implementation considerations.

Every material recommendation must use one disposition:

- KEEP
- INTEGRATE
- ADAPT
- PARTIAL
- SEPARATE
- DEFER
- REJECT
- NO ACTION

## 9. Authorization Boundary

Record:

- Actions authorized.
- Actions explicitly prohibited.
- Approval references.
- Proposed actions requiring future approval.

Phase 0 does not authorize Phase 1 modifications.

## 10. Phase 0 Completion Status

Permitted values:

- DRAFT
- IN_PROGRESS
- COMPLETE
- BLOCKED
- REJECTED

COMPLETE requires all mandatory sections, evidence references for material findings, identified limitations, and a documented recommendation.

## 11. Phase 1 Handoff

Record:

- Approved objective and scope proposed for Phase 1.
- Proposed implementation requirements.
- Dependencies.
- Acceptance criteria.
- Unresolved issues.
- Required approvals.
- Deferred and rejected proposals.
- Explicit statement that Phase 1 requires separate authorization.

## 12. Governing Rule

A Phase 0 manifest records investigation and recommendations. It does not establish implementation authority or convert proposed capabilities into verified capabilities.
