# RACE ARCHITECTURE
## System Structure and Phase Relationships

Version: 1.0
Status: Initial Foundation

## 1. Architectural Objective

RACE provides a repeatable framework for converting human objectives into structured AI execution assignments.

Its architecture separates mission definition, investigation, planning, implementation, and verification.

## 2. Principal Components

### Core
RACE_CORE.md defines governing principles and mandatory operating requirements.

### Templates
Templates standardize the structure of Phase 0, Phase 1, Phase 2, repository profiles, and evaluations.

### Protocols
Protocols establish common rules for evidence, dependencies, authorization, and handoffs.

### Schemas
Schemas define required manifest information and phase-specific output structures.

### Campaigns
Campaign profiles preserve mission-specific context, scope, constraints, and requirements.

### Evaluations
Evaluation standards provide repeatable criteria for assessing RACE quality.

## 3. Three-Phase Architecture

### Phase 0 — Discovery and Blueprint

Purpose:
Establish an independently investigated understanding of the mission and produce an evidence-supported architectural blueprint.

Required activities:
- Establish mission scope.
- Inspect available evidence.
- Identify dependencies.
- Identify architectural constraints.
- Conduct adversarial examination.
- Evaluate alternatives.
- Identify unresolved questions.
- Produce recommendations.

Primary output:
Phase 0 Manifest and Architectural Blueprint.

Phase 0 does not authorize implementation.

### Phase 1 — Construction

Purpose:
Translate the approved blueprint into a controlled implementation plan and authorized work.

Required activities:
- Confirm Phase 0 acceptance.
- Define implementation boundaries.
- Identify affected components.
- Establish change sequence.
- Define acceptance criteria.
- Establish rollback considerations.
- Execute only authorized changes.

Primary output:
Phase 1 Manifest and implementation record.

### Phase 2 — Verification and Closure

Purpose:
Determine whether the implementation satisfies the approved requirements.

Required activities:
- Inspect resulting artifacts.
- Execute authorized tests.
- Conduct adversarial retesting.
- Compare outcomes against acceptance criteria.
- Identify remaining defects.
- Record unresolved risks.
- Produce a closure recommendation.

Primary output:
Phase 2 Manifest and final evaluation.

## 4. Permanent Expert Panel

Every phase retains three permanent expert seats:

- UCO
- The Hacker
- MacG

Mission-specific experts may supplement these seats.

## 5. Evidence and Traceability

Each phase must preserve traceability between:

- Human objectives.
- Source evidence.
- Findings.
- Recommendations.
- Authorizations.
- Actions.
- Verification results.
- Final disposition.

## 6. Authorization Boundaries

Phase completion does not automatically authorize the next phase.

Human approval is required at defined decision boundaries.

No implementation, external modification, commit, push, or deployment may be inferred from approval of an investigation alone.

## 7. Handoffs

Each phase must provide a structured handoff containing:

- Completed deliverables.
- Supporting evidence.
- Decisions.
- Outstanding questions.
- Risks.
- Dependencies.
- Required approvals.
- Next-phase entry conditions.

## 8. Architectural Integrity

The core defines authority.

Protocols define operating rules.

Templates define document structure.

Schemas define required information.

Campaigns define mission-specific context.

Evaluations measure quality.

No individual campaign may silently override RACE's governing requirements.
