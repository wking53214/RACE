RACE — HERALD

PHASE 1: DEEP RESEARCH, ARCHITECTURAL CHALLENGE & SOLUTION IDENTIFICATION

1. MISSION

Conduct a comprehensive research and solution-design campaign based on the completed HERALD Phase 0 discovery package.

Phase 0 established what exists, what is known, what is broken, what HERALD connects to, and what needs further investigation.

Phase 1 must determine:

What is the best way to make HERALD fulfill its intended purpose, including the best ways to replace, redesign, integrate, simplify, or eliminate its existing components?

This is not another general code review.

It is a deep investigation of problems, opportunities, technical alternatives, system-wide implications, and possible solutions.

Phase 1 must produce a complete, dependency-aware implementation blueprint for Phase 2.

No code updates or production modifications are permitted in Phase 1.

---

2. MANDATORY PHASE 0 INPUT GATE

Phase 1 is INOPERABLE until the actual Phase 0 output is provided.

Do not start Phase 1 using:

- Memory of the previous audit.
- A summary of Phase 0.
- The Phase 0 prompt without its results.
- Assumptions about what Phase 0 probably found.
- A previous repository baseline.
- An incomplete or unverified collection of Phase 0 excerpts.

Required inputs

Require the Phase 0 kickoff package:

1. "PHASE0_EXECUTIVE_AND_KICKOFF.md"
2. "PHASE0_FINDINGS_REGISTER.csv"
3. "PHASE0_DEPENDENCY_REGISTER.csv"
4. "PHASE0_CONTRACT_INVENTORY.csv"
5. "PHASE0_QUESTIONS_AND_RESEARCH_AGENDA.md"
6. "PHASE0_SOURCE_INDEX.md"
7. "PHASE0_MANIFEST.json"

Equivalent formats are acceptable only when the information is complete and traceable.

Validate the package

Before conducting research:

- Verify that every required artifact is present.
- Read the entire available package.
- Validate finding IDs and cross-references.
- Validate dependency and contract references.
- Check the manifest's completeness status.
- Identify missing, conflicting, or malformed information.
- Establish the exact repository commits and versions used by Phase 0.
- Identify any gaps that could materially affect solution design.

The package must establish at least "READY FOR PHASE 1 WITH DOCUMENTED GAPS".

If Phase 0 declared "NOT READY FOR PHASE 1", Phase 1 must not proceed normally.

If required artifacts are missing, incomplete, or unusable, return:

"PHASE 1 BLOCKED — PHASE 0 INPUT INSUFFICIENT"

Then produce a precise list of missing items and explain what must be supplied or corrected.

Do not invent the missing research inputs.

Do not quietly downgrade this gate to a recommendation.

Revalidate material facts

The Phase 0 package is the starting point, not unquestionable truth.

Before relying on a material finding, inspect the relevant current source and verify that the repository has not materially changed.

Record baseline drift:

- Different HEAD commits.
- Changed interfaces.
- New dependencies.
- Changed branches or releases.
- Modified contracts.
- Changed downstream repositories.

If material drift is detected, assess its effect and update the research assumptions.

Do not silently replace Phase 0 facts with newer facts. Record the difference and its consequences.

---

3. PERMANENT RACE EXPERT PANEL

The same three seats used in Phase 0 remain permanent.

No additional expert seats may be added.

UCO — Universal Chief Officer

Challenge:

- Whether the solution supports HERALD's overarching mission.
- Whether the architecture is strategically sound.
- Whether responsibilities belong in HERALD or elsewhere.
- Whether downstream dependencies are being handled correctly.
- Whether the proposed target architecture will remain viable as STACK evolves.

Hacker — Adversarial Security Expert

Challenge:

- Whether proposed solutions can be bypassed.
- Whether they create new vulnerabilities.
- Whether trust guarantees are real and independently verifiable.
- Whether the migration introduces temporary security weaknesses.
- Whether downstream systems could accept invalid or forged information.

MacGyver — Systems Engineering Expert

Challenge:

- Whether the proposed solution is unnecessarily complex.
- Whether an existing capability can be reused.
- Whether there is a better technical approach.
- Whether the solution can be implemented and maintained.
- Whether the same result can be achieved with fewer components and dependencies.

Each seat must investigate solutions rather than merely comment on the Phase 0 findings.

Record meaningful disagreement and resolve it through evidence and reasoning.

Do not claim independent AI agents were used unless they actually were.

---

4. ARCHITECTURAL REPLACEMENT AND ELIMINATION AUTHORITY

HERALD's existing architecture has no presumption of permanence.

Claude Code is authorized to investigate and recommend complete replacement or elimination of any aspect that does not directly support HERALD's overarching intent and required functionality.

Where a better solution exists, the existing implementation may be discarded entirely in the proposed design.

Investigate:

- Complete module replacement.
- Component consolidation.
- Architectural separation.
- Alternative data models.
- Alternative verification mechanisms.
- Alternative signing and key-management arrangements.
- Existing STACK capabilities that could replace duplicated HERALD functionality.
- Removal of unnecessary abstractions.
- Removal of obsolete or mission-inconsistent functionality.
- Fundamentally different approaches where the current approach is inadequate.

Do not bias toward incremental modification simply because it appears less disruptive.

Compare incremental repair against structural redesign and complete replacement.

For every elimination recommendation, identify:

- Existing functionality.
- Whether that functionality is required.
- Replacement functionality, if required.
- Actual consumers.
- Contract and compatibility consequences.
- Migration requirements.
- Risks of removal.
- Why the proposed new approach is better.

This authority covers research and design in Phase 1.

It does not authorize Phase 1 code changes.

Phase 2 may implement complete replacement or elimination when it is included in the Phase 1 blueprint and explicitly approved by the human owner.

---

5. RESEARCH METHOD

For every material Phase 0 finding or opportunity, use the following process.

A. Establish the real problem

Determine:

- What is actually wrong or missing?
- Is the issue a design flaw, implementation defect, incomplete integration, missing operational capability, or documentation problem?
- Is the issue isolated or a symptom of a larger architectural problem?
- What evidence demonstrates the problem?
- What happens if it is not addressed?

Do not solve symptoms without investigating root causes.

B. Investigate alternatives

For every P0 and P1 issue, investigate at least:

1. The smallest reasonable correction.
2. A structural improvement to the current architecture.
3. A replacement approach, where technically plausible.

For lower-priority issues, investigate alternatives proportionately.

Do not manufacture alternatives merely to satisfy a number. Explain when a meaningful alternative does not exist.

C. Research technical viability

Investigate:

- Existing STACK capabilities.
- Relevant standards and specifications.
- Established technical approaches.
- Library and dependency maturity.
- Security properties.
- Python compatibility.
- Operational requirements.
- Licensing and supply-chain considerations.
- Long-term maintenance.
- Performance and scaling.
- Integration complexity.

Prefer primary documentation, standards, implementation references, and authoritative technical sources.

When external research is used:

- Cite the source.
- Identify its publication or version date when available.
- Separate documented guarantees from assumptions.
- Do not treat a vendor claim as independent validation.
- Identify where current information could not be verified.

D. Compare alternatives

For each solution candidate, evaluate:

- Functional correctness.
- Security and trust properties.
- Complexity.
- Maintainability.
- Integration compatibility.
- Downstream dependency impact.
- Migration difficulty.
- Operational burden.
- Performance.
- Failure recovery.
- Extensibility.
- Dependency and supply-chain risk.

Identify meaningful trade-offs.

Do not assign arbitrary numerical scores or claim quantitative superiority without a defensible method.

E. Select a recommendation

Recommend:

- Preferred approach.
- Rejected alternatives.
- Why the preferred approach wins.
- What evidence supports the decision.
- Remaining risks.
- Unresolved assumptions.
- Conditions under which the decision should change.

---

6. EXPANDED RESEARCH COVERAGE

Phase 1 must go beyond the issues already identified in Phase 0.

Use the following domains as a mandatory research checklist. Do not assume Phase 0 covered these deeply enough merely because it mentioned them.

A. Evidence and claim model

Investigate:

- What constitutes a source?
- What constitutes evidence?
- What constitutes a claim?
- How are source references retained?
- How is claim identity established?
- How are revisions represented?
- Can claims be merged, superseded, or withdrawn?
- How is conflicting evidence represented?
- How are derived claims distinguished from directly extracted claims?
- Can the system reconstruct the origin and transformation history of a claim?
- Are provenance and confidence being conflated?
- Are claims independently verifiable after export?

Identify the most suitable evidence and claim lifecycle.

B. Source authenticity and extraction

Investigate:

- Source authenticity.
- Source integrity.
- Document identity.
- File and content digests.
- Extraction reproducibility.
- OCR and document parsing.
- Tables, images, and structured data.
- Multilingual extraction.
- Malformed and adversarial documents.
- Prompt injection in source material.
- Hidden or misleading content.
- Extraction failure and partial extraction.
- Extractor versioning.
- Extractor provenance.
- Reproducibility across versions.

Determine whether extraction should remain a HERALD responsibility or use a replaceable adapter architecture.

C. Confidence and calibration

Investigate:

- Meaning of a confidence value.
- Whether confidence is calibrated against actual outcomes.
- Difference between model confidence and evidence quality.
- Confidence aggregation.
- Threshold design.
- Per-kind thresholds.
- Missing data.
- Conflicting evidence.
- Uncertainty representation.
- Human confirmation effects.
- Calibration corpus size and composition.
- Multilingual and domain-specific evaluation.
- False acceptance and false rejection.

Determine which confidence statements HERALD can actually defend.

Do not imply probabilistic calibration unless supported by suitable validation data.

D. Human confirmation and identity

Investigate:

- What qualifies as human confirmation?
- How confirmation is bound to a claim.
- How a claim revision affects prior confirmation.
- Confirmation expiration.
- Replay resistance.
- Revocation.
- Authenticated identity.
- Attribution.
- Delegation.
- Multi-person confirmation.
- Conflicting human confirmations.
- Audit records.
- External identity-provider integration.

Determine what HERALD can safely implement itself and what must be delegated to an identity or trust service.

E. Cryptographic architecture

Investigate:

- HMAC versus asymmetric signing.
- Portable verification.
- Key generation.
- Key ownership.
- Key storage.
- Key distribution.
- Key rotation.
- Key revocation.
- Compromise recovery.
- Algorithm agility.
- Signature envelope formats.
- Canonical serialization.
- Domain separation.
- Digest versioning.
- Verification after software upgrades.
- Historical signature validation.
- External trust roots.

Evaluate the Ed25519 approach and other viable alternatives.

Do not recommend cryptography merely because it is stronger in isolation. Establish who owns and verifies the keys, how consumers obtain trust, and what happens when trust is withdrawn.

F. Distributed operation and lifecycle

Investigate:

- Independent processes.
- Multiple machines.
- Service boundaries.
- Restart behavior.
- Concurrency.
- Idempotency.
- Duplicate delivery.
- Ordering.
- Eventual consistency.
- Retries.
- Replay protection.
- Partial failure.
- Network interruption.
- Version disagreement.
- Recovery.
- Time and clock assumptions.

Establish what is required for HERALD to work reliably outside a single process.

G. Persistence and evidence lifecycle

Investigate:

- What must be persisted.
- What can be reconstructed.
- What constitutes the system of record.
- Immutability requirements.
- Version history.
- Retention.
- Deletion.
- Archival.
- Export and import.
- Backup and recovery.
- Integrity verification.
- Evidence lineage across systems.

Examine whether TIE or another existing STACK component should own any persistence responsibility.

Do not duplicate an established capability without a demonstrated need.

H. Privacy and data protection

Investigate:

- Personally identifiable information.
- Sensitive document contents.
- Data minimization.
- Redaction.
- Retention and deletion.
- Confidentiality of exports.
- Access boundaries.
- Tenant or organizational separation.
- Logging exposure.
- Secret handling.
- Regulatory implications where applicable.

Distinguish technical requirements from legal conclusions. Do not invent compliance claims.

I. API and contract evolution

Investigate:

- Public interfaces.
- Schema evolution.
- Version compatibility.
- Deprecation.
- Optional versus required fields.
- Unknown fields.
- Error semantics.
- Status semantics.
- Contract tests.
- Backward and forward compatibility.
- Consumer version negotiation.
- Migration adapters.

Determine how HERALD should evolve without silently breaking downstream consumers.

J. Operational reliability

Investigate:

- Performance requirements.
- Throughput.
- Latency.
- Memory usage.
- Large documents.
- Resource exhaustion.
- Timeouts.
- Retry behavior.
- Observability.
- Logging.
- Metrics.
- Diagnostics.
- Failure classification.
- Operational recovery.

Do not invent service-level requirements. Identify what needs an explicit owner decision.

K. Software supply chain and release engineering

Investigate:

- Dependency pinning.
- Reproducible builds.
- Dependency vulnerability management.
- GitHub Actions hardening.
- Secret handling in CI.
- Build provenance.
- Package integrity.
- Release tagging.
- Changelog strategy.
- Versioning.
- SBOM requirements where appropriate.
- Third-party licensing.
- Installation and upgrade safety.

Identify which improvements are necessary for reliable downstream adoption.

L. Test and validation architecture

Investigate:

- Unit tests.
- Contract tests.
- Integration tests.
- Cross-process tests.
- Security tests.
- Property-based testing.
- Fuzz testing.
- Regression suites.
- Golden datasets.
- Adversarial document corpus.
- Calibration evaluation.
- Fault injection.
- Migration tests.
- Compatibility tests.
- Reproducibility of tests.

Identify where the current test suite proves behavior and where it merely checks internal implementation details.

M. Human and operational workflow

Investigate:

- Who uses HERALD?
- Who provides source documents?
- Who confirms claims?
- Who consumes outputs?
- How are exceptions handled?
- How are uncertain results presented?
- How are corrections made?
- How are decisions audited?
- How are failed or disputed claims handled?

Do not invent users or business requirements. Mark those requiring owner decisions.

---

7. STACK-WIDE DOWNSTREAM SOLUTION DESIGN

For every proposed change, follow its effects beyond HERALD.

Revisit all verified relationships in the Phase 0 dependency register.

Investigate actual repository contracts and implementation where available, including relevant relationships with:

- CNS.
- TIE.
- CCC.
- Conservation_Kernel.
- Governance_Gateway.
- CCCb.
- Any additional verified consumers or producers.

For each proposed solution, determine:

A. Contract effects

- Which interfaces change?
- Which data structures change?
- Which fields become required, optional, or obsolete?
- Do status values change?
- Do error semantics change?
- Do digests or signatures change?
- Does version negotiation become necessary?

B. Downstream implementation requirements

- Which repository must change?
- What exact behavior must change?
- Which consumer assumptions must be updated?
- Are adapters needed?
- Are coordinated releases required?
- Is a temporary compatibility layer necessary?

C. Failure and migration scenarios

- HERALD upgraded before consumer.
- Consumer upgraded before HERALD.
- Older historical records.
- Mixed contract versions.
- Failed verification.
- Missing keys.
- Removed or replaced components.
- Partial rollout.
- Rollback after migration.

D. Ownership and authority

Establish which system owns:

- Claim creation.
- Source extraction.
- Evidence persistence.
- Signature verification.
- Identity authentication.
- Policy evaluation.
- Consequence governance.
- Authorization.

Do not let a convenience integration silently transfer authority to the wrong component.

E. Change classification

Classify each proposed change as:

- HERALD ONLY.
- HERALD + CNS.
- HERALD + TIE.
- HERALD + MULTIPLE STACK REPOSITORIES.
- DOWNSTREAM ONLY.
- EXTERNAL DEPENDENCY.
- NO CODE CHANGE REQUIRED.
- DEFERRED PENDING OWNER DECISION.

Use exact repository names and evidence.

Do not assume an entire repository must be modified when a smaller adapter or contract change would suffice.

---

8. TARGET ARCHITECTURE DESIGN

Produce a complete proposed HERALD target architecture.

Include:

- Component responsibilities.
- Public interfaces.
- Internal boundaries.
- Data structures.
- Evidence and claim lifecycle.
- Validation sequence.
- Human confirmation lifecycle.
- Provenance model.
- Cryptographic and verification model.
- Error and failure behavior.
- Export and downstream consumption.
- CNS integration.
- External service boundaries.
- Ownership of each responsibility.

Show how a source becomes an evidence-backed claim and how that claim is verified and consumed by downstream systems.

Identify all trust transitions.

The architecture must be explicit enough that Phase 2 can implement it without inventing missing design decisions.

Provide architecture diagrams where useful, including:

- Component diagram.
- Data-flow diagram.
- Trust-boundary diagram.
- Sequence diagram for the primary governed path.
- Downstream dependency diagram.
- Migration and deployment sequence.

Every diagram must match the written design.

Do not depict planned functionality as existing functionality.

---

9. SOLUTION AND DECISION REGISTER

For every Phase 0 finding, determine what should happen.

For every newly discovered issue, add a new entry.

Every entry must include:

Field| Required content
ID| Unique stable identifier
Source finding| Phase 0 finding ID or NEW
Root cause| Established underlying problem
Evidence| Source and external research
Options| Meaningful alternatives examined
Recommendation| Preferred solution
Disposition| KEEP / INTEGRATE / ADAPT / PARTIAL / SEPARATE / DEFER / REJECT / NO ACTION
Priority| P0 / P1 / P2 / P3
Scope| Exact affected component or repository
Dependencies| Upstream and downstream requirements
Contract impact| Interface, schema, version, or semantic changes
Security impact| Trust and attack-surface implications
Migration| Transition requirements
Validation| Required tests and acceptance criteria
Risk| Remaining weaknesses
Decision status| Recommended / unresolved / awaiting owner
Phase 2 authorization| Pending human approval

Required disposition discipline

Do not preserve a component automatically.

Use:

- KEEP when it is fit for purpose.
- INTEGRATE when a proven existing capability should be reused.
- ADAPT when the capability is sound but needs changes.
- PARTIAL when only some functionality should survive.
- SEPARATE when responsibilities are improperly coupled.
- DEFER when a prerequisite or owner decision is missing.
- REJECT when the proposal is unsuitable.
- NO ACTION when no change is justified.

For components recommended for complete removal, explicitly record the removal scope and all replacement or downstream consequences.

---

10. IMPLEMENTATION AND MIGRATION BLUEPRINT

Design Phase 2 around dependency order, not the order in which findings appeared.

Establish:

- Prerequisite changes.
- Independent changes.
- Changes that must be coordinated.
- Changes requiring versioned contracts.
- Changes requiring migration.
- Changes requiring external services.
- Changes that can be implemented entirely within HERALD.
- Changes that cannot safely proceed without another repository or owner decision.

Implementation sequencing

Group work into coherent implementation units.

For each unit specify:

- Objective.
- Exact repositories.
- Exact architectural surfaces.
- Required modifications.
- Dependencies.
- Expected outputs.
- Acceptance criteria.
- Regression tests.
- Adversarial tests.
- Downstream integration tests.
- Rollback conditions.
- Completion evidence.

Use one logical intervention per retest wherever practical.

Do not combine unrelated fixes simply because they are in the same file.

Compatibility strategy

Specify:

- Existing contract versions.
- Proposed contract versions.
- Backward compatibility.
- Forward compatibility.
- Adapters.
- Deprecation.
- Migration.
- Data conversion.
- Historical record verification.
- Rollback.

If compatibility cannot be preserved, explain the breaking change and the coordinated deployment requirement.

Implementation boundaries

Phase 2 may modify HERALD and other repositories only when their changes are included in the approved scope.

If a downstream dependency cannot be changed, do not silently pretend the integration is complete. Identify the blocked dependency and propose a safe interim boundary.

---

11. TEST AND ACCEPTANCE BLUEPRINT

Phase 1 does not modify or implement code. It designs the validation campaign.

Produce explicit acceptance criteria for each proposed implementation unit.

Include, where relevant:

- Regression tests.
- Trust-boundary tests.
- Claim substitution tests.
- Claim mutation tests.
- Confirmation binding tests.
- Forged provenance tests.
- Unknown extractor tests.
- Threshold validation tests.
- Non-finite numeric tests.
- Concurrency and replay tests.
- Cross-process signature verification.
- Key rotation and revocation tests.
- Export/import tests.
- CNS contract tests.
- TIE consumer verification.
- Schema compatibility tests.
- Failure propagation tests.
- Historical data migration tests.
- Adversarial extraction corpus.
- Performance and resource tests.

For each test specify:

- What is being tested.
- Which component or repository owns it.
- Expected behavior.
- Attack or failure scenario.
- Acceptance criterion.
- Required evidence.

Do not invent test counts or promise test results.

---

12. PHASE 1 REQUIRED DELIVERABLES

Create a self-contained Phase 2 implementation blueprint.

Deliverable 1 — Research executive assessment

Explain the best overall direction and why.

Deliverable 2 — Phase 0 finding disposition

Every Phase 0 finding must be addressed, with no unexplained omissions.

Deliverable 3 — Deep research report

Show root causes, alternatives, evidence, and solution decisions.

Deliverable 4 — Target architecture

Complete proposed design with responsibilities, flows, interfaces, and trust boundaries.

Deliverable 5 — Replacement and elimination plan

Identify what should be kept, adapted, integrated, separated, partially retained, or completely removed.

Deliverable 6 — Downstream impact matrix

Map every proposed change to affected repositories, contracts, consumers, dependencies, migration, and testing.

Deliverable 7 — Contract evolution plan

Define proposed schemas, interfaces, versioning, status semantics, and compatibility requirements.

Deliverable 8 — Security and trust design

Define the trust model, identities, confirmation, signing, keys, verification, and failure handling.

Deliverable 9 — Migration and compatibility plan

Define rollout order, adapters, historical-data treatment, rollback, and coordinated releases.

Deliverable 10 — Phase 2 implementation sequence

Specific ordered implementation units and dependencies.

Deliverable 11 — Phase 2 acceptance and test plan

All required tests and measurable acceptance criteria.

Deliverable 12 — Deferred and owner-decision register

Explicitly record anything that cannot be safely decided or implemented without human input.

Deliverable 13 — Final authorization register

For every proposed change record:

- Recommended action.
- Exact scope.
- Affected repositories.
- Destructive or replacement actions.
- Expected downstream effects.
- Outstanding conditions.
- Human approval status.

Deliverable 14 — Phase 2 handoff package

Create these files, or clearly equivalent artifacts:

1. "PHASE1_EXECUTIVE_AND_SOLUTION_BLUEPRINT.md"
2. "PHASE1_DECISION_REGISTER.csv"
3. "PHASE1_DOWNSTREAM_IMPACT_REGISTER.csv"
4. "PHASE1_TARGET_ARCHITECTURE.md"
5. "PHASE1_CONTRACT_AND_MIGRATION_PLAN.md"
6. "PHASE1_IMPLEMENTATION_SEQUENCE.md"
7. "PHASE1_ACCEPTANCE_AND_TEST_PLAN.md"
8. "PHASE1_DEFERRED_DECISIONS.md"
9. "PHASE1_AUTHORIZATION_REGISTER.csv"
10. "PHASE1_MANIFEST.json"

The manifest must identify:

- The exact Phase 0 package used.
- The HERALD baseline revalidated.
- Repository commits/versions used.
- Every recommendation ID.
- Every implementation unit.
- All affected repositories.
- Required approvals.
- Deferred decisions.
- Completeness status.

Create research artifacts outside repository Git worktrees. Do not modify repositories to store the reports.

---

13. SECONDARY WORKSTREAM — INDEPENDENT RACE PERFORMANCE EVALUATION

Produce a separate evaluation of RACE's performance during Phase 1.

This is independent research. It does not have to build on or inherit the Phase 0 RACE evaluation.

Do not let the RACE evaluation alter the primary HERALD research or solution recommendations.

Evaluate:

Permanent-seat effectiveness

- Did UCO identify strategic or system-level solutions?
- Did Hacker materially improve the proposed trust and security architecture?
- Did MacGyver find simpler or better implementations?
- Did the seats challenge each other effectively?
- Did their contributions remain distinct?

Deep-research effectiveness

- Did RACE identify meaningful alternatives?
- Did it investigate root causes rather than symptoms?
- Did it discover downstream implications that might otherwise have been overlooked?
- Did structured challenge improve the preferred solution?
- Did the structure reduce unsupported assumptions?

New capabilities
Identify capabilities demonstrated during Phase 1 that were not evident in a conventional review workflow.

Operational burden

- Repetition.
- Analysis overhead.
- Excessive deliberation.
- Token or context consumption, only if measurable.
- Slower or less focused decisions.
- False disagreements.
- Unnecessary process.

Net value verdict

Use:

- HELP.
- PARTIAL HELP.
- NEUTRAL.
- HINDRANCE.
- INCONCLUSIVE.

Support the verdict with actual examples from this Phase 1 execution.

Independent output

Produce:

"RACE_PHASE1_INDEPENDENT_EVALUATION.md"

This must stand alone. Do not rely on the Phase 0 RACE evaluation to reach its conclusions.

Include:

- What worked.
- What failed.
- What was new.
- Which seat provided distinct value.
- Where the panel duplicated work.
- Whether disagreement produced better solutions.
- Whether RACE improved research quality.
- Whether it created unnecessary overhead.
- Net value verdict.
- Recommendations for future RACE use.

---

14. PHASE 1 QUALITY GATE

Phase 1 is complete only when:

- The complete Phase 0 package has been validated.
- Material baseline drift has been addressed.
- Every Phase 0 finding has a disposition.
- New issues are documented.
- Significant alternatives have been investigated.
- The target architecture is explicit.
- Replacement and elimination decisions are justified.
- Actual downstream requirements have been mapped.
- Contract and migration implications are explicit.
- Test and acceptance criteria are defined.
- Implementation order is dependency-aware.
- All unresolved owner decisions are recorded.
- The Phase 2 package is complete.
- The independent RACE evaluation is separately produced.

Phase 1 exit status

Return exactly one:

- "READY FOR PHASE 2 APPROVAL"
- "READY FOR PHASE 2 APPROVAL WITH DOCUMENTED CONDITIONS"
- "NOT READY FOR PHASE 2"

A complete blueprint is not implementation authorization.

---

15. FINAL AUTHORIZATION BOUNDARY

PHASE 1 ONLY.

No production source-code changes.

No test changes.

No repository documentation changes.

No dependency modifications.

No commits, pushes, merges, branch deletions, tags, or releases.

All proposed changes, including complete replacement or elimination, must be recorded in the blueprint.

Do not begin Phase 2 automatically.

Stop after delivering:

1. The complete Phase 2 implementation blueprint.
2. The human authorization register.
3. The separate RACE Phase 1 evaluation.

Phase 2 requires the actual Phase 1 output and explicit human approval of the implementation scope.

Phase 1 identifies the best solution. Phase 2 is responsible for implementing the approved solution.
