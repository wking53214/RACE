# RACE DEPENDENCY PROTOCOL
Version: 1.0

## 1. Purpose

Establish how RACE identifies, evaluates, records, and validates dependencies between systems, repositories, components, people, processes, and external services.

## 2. Dependency Identification

A dependency is a relationship in which one component relies upon another for functionality, data, authorization, execution, or operational continuity.

Investigators must distinguish:

- Direct dependencies.
- Indirect dependencies.
- Optional dependencies.
- Runtime dependencies.
- Development dependencies.
- External dependencies.
- Human or organizational dependencies.
- Proposed dependencies.
- Unverified dependencies.

## 3. Dependency Evidence

Every material dependency claim should identify:

- Source component.
- Target component.
- Relationship type.
- Nature of reliance.
- Evidence supporting the relationship.
- Direction of dependency.
- Version or interface constraints where applicable.
- Failure consequences.
- Verification status.

## 4. Dependency Verification

A dependency must not be considered verified solely because:

- Two repositories mention each other.
- A README describes an integration.
- A proposed architecture includes a connection.
- A package is listed but never exercised.
- A developer states that integration exists.

Where possible, inspect imports, interfaces, configuration, call paths, execution records, and integration tests.

## 5. Dependency Mapping

RACE should identify:

- Critical dependencies.
- Single points of failure.
- Circular dependencies.
- Version incompatibilities.
- Unowned dependencies.
- Missing dependencies.
- Hidden assumptions.
- External service risks.

## 6. Dependency Classification

Use the following dispositions:

- VERIFIED: Supported by direct evidence.
- PARTIALLY VERIFIED: Some aspects established; others remain uncertain.
- PROPOSED: Intended but not established as implemented.
- UNVERIFIED: Evidence is insufficient.
- BROKEN: Evidence demonstrates a failed dependency.
- NOT APPLICABLE: No relevant dependency exists within the examined scope.

## 7. Change Impact

Before proposing a change, identify affected components and downstream relationships.

Consider compatibility, data contracts, security boundaries, operational continuity, and rollback implications.

## 8. Uncertainty

Unknown dependency relationships must remain explicitly identified.

Do not invent integration paths to complete a diagram.

## 10. Governing Rule

A documented relationship is not automatically an operational dependency. Dependency claims require evidence appropriate to the claimed relationship.
