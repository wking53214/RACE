# RACE PROMPT RECORD SCHEMA

## 1. Identity

- Prompt identifier.
- Campaign identifier.
- Phase.
- Sequence number.
- Version.
- Generation date and time.
- Record status.

## 2. Generation Context

- Human objective.
- Input brief reference.
- Sanitized input snapshot.
- Scope and constraints.
- Target repository or system.
- Target branch and commit, if known.
- Intended deliverables.

## 3. RACE Framework Baseline

- RACE version or baseline identifier.
- Source document versions.
- Source template versions.
- Source schema versions.
- Git commit, if available.
- Applicable protocols.

Unknown values must be marked UNKNOWN, not guessed.

## 4. Expert Panel and Configuration

Record all three permanent seats in every prompt:

- UCO — Universal Chief Officer (UCO-001).
- The Hacker (HACKER-001).
- MacG (MACG-001).

### 4.1 Identity and Capability Status

For every permanent and additional expert, record:

- Expert ID and name.
- Identity formalization status.
- Identity version and approval status, if established.
- Capability-library formalization status.
- Capability-library version and approval status, if established.
- Performance-validation status.
- Operating-doctrine version and status, if established.
- Mission assignment.
- Participation evidence.
- Known limitations and specialist dependencies.

Current documented baseline; verify against the current identity registry,
capability registry, and version manifest when assembling a prompt:

- UCO-001: identity v1.0 APPROVED; capability library v1.0 APPROVED;
  operating doctrine v1.0 APPROVED; performance validation NOT PERFORMED.
- HACKER-001: identity and capability library NOT YET FORMALIZED.
- MACG-001: identity and capability library NOT YET FORMALIZED.

Do not invent missing identities, versions, capabilities, approvals, or
validation results. A mission assignment does not create or modify an
expert's permanent identity.

### 4.2 Selected Capability Records

For every capability selected from any expert, record all seven fields:

1. Capability ID.
2. Capability name.
3. Applicable mission question.
4. Expected analytical contribution.
5. Relevant evidence requirements.
6. Known limitations.
7. Specialist dependency.

Also record the owning expert ID and name for each capability.

Do not invent formal capability IDs or capability-library entries for an
expert whose capability library has not been formalized. If an analytical
assignment is needed before formalization, identify it as a mission
assignment, not as an approved library capability.

Capability selection does not establish that the capability was exercised,
demonstrated, or successful. Record actual participation and evidence
separately.

### 4.3 Panel Configuration and Traceability

Record:

- The mission snapshot identifier and location.
- The exact expert identities, versions, approval statuses, and capability
  selections used for this prompt.
- The mission assignment and participation evidence for each seat.
- Any additional experts, their formal status, versions, assignments, and
  limitations.
- Missing formal definitions, unresolved dependencies, and material
  disagreements.
- The exact generated prompt artifact location, version, and available hash.

The UCO, The Hacker, and MacG remain mandatory permanent seats. Additional
experts supplement the permanent panel; they do not replace its members.

A simulated expert perspective within one AI execution is not an
independently executed agent. Do not claim independent participation unless
separate execution and supporting evidence establish it.

## 5. Prompt Generation

- Prompt-generation method.
- Generating AI or system.
- Model and version, if known.
- Generation instructions or source references.
- Human modifications after generation.
- Approval status.

## 6. Execution Context

Complete when execution occurs:

- Executing AI or system.
- Model and version, if known.
- Execution date and time.
- Operator.
- Execution environment.
- Execution identifier, if available.
- Deviations from intended execution.

Do not confuse the generating AI with the executing AI.

## 7. Authorization

- Authorized actions.
- Prohibited actions.
- Approval references.
- Execution restrictions.

## 8. Output References

- PROMPT.md location.
- EVALUATION.md location.
- Result artifacts.
- Evidence references.
- Handoff references.

## 9. Lifecycle Status

Permitted values:

- DRAFT
- GENERATED
- ARCHIVED
- APPROVED
- EXECUTED
- EVALUATED
- SUPERSEDED
- WITHDRAWN

Status changes must reflect actual events.

## 10. Integrity

Record available hashes or other integrity references for archived prompt artifacts.

## 11. Governing Rule

A prompt record must preserve the distinction between what was generated, what was executed, and what was demonstrated by evidence.
