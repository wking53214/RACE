
RACE — HERALD

PHASE 0: INDEPENDENT DISCOVERY, ARCHITECTURAL REASSESSMENT & PHASE 1 KICKOFF

1. MISSION

Conduct a complete, independent reassessment of "wking53214/HERALD".

Establish the actual state of the repository, independently inspect its implementation, challenge its architecture, identify every material defect and opportunity, map its upstream and downstream dependencies, and establish what HERALD must become to fulfill its intended purpose.

This assignment repeats the depth and breadth of the previous HERALD FACP and code-hygiene review, but has a more demanding deliverable:

Phase 0 must produce the complete, evidence-backed kickoff package required to begin Phase 1 without rediscovering the repository, its problems, its interfaces, or its dependencies.

Do not stop at a code review. Establish the facts and provide the research agenda.

HERALD must be evaluated in two contexts:

1. As an independent software system.
2. As a component of STACK and its actual connected systems.

Do not presume that every STACK repository is connected to HERALD. Discover and prove actual relationships.

This is a discovery, inspection, and planning assignment. No production code changes are authorized in Phase 0.

---

2. PERMANENT RACE EXPERT PANEL

The following three seats are permanent. They participate throughout every phase and every major architectural decision.

No additional expert seats, randomly selected professions, or expanding panels are permitted. The three seats must cover the required perspectives without turning RACE into an unnecessarily complicated committee.

Seat 1 — UCO: Universal Chief Officer

Responsible for:

- Strategic architecture and mission alignment.
- Whole-system design and long-term viability.
- Component boundaries and responsibility allocation.
- STACK-wide implications.
- Identifying unnecessary complexity and architectural drift.
- Ensuring that proposed improvements serve HERALD's overarching purpose.

UCO must challenge whether the system is solving the right problem.

Seat 2 — Hacker: Adversarial Security Expert

Responsible for:

- Attack surfaces and trust boundaries.
- Exploitation, spoofing, bypasses, and replay.
- Forged or misleading provenance.
- Authentication, signatures, and verification.
- Hostile inputs and malformed data.
- Failure propagation across connected systems.
- Challenging optimistic assumptions and unsupported guarantees.

Hacker must assume that inputs, integrations, and users may be hostile or mistaken.

Seat 3 — MacG: Systems Engineering Expert

Responsible for:

- Practical implementation architecture.
- Simplicity and maintainability.
- Alternative technical approaches.
- Integration efficiency.
- Avoiding duplicated capabilities.
- Identifying unnecessary dependencies.
- Finding the smallest effective solution without sacrificing required behavior.

MacG must challenge overengineering and identify better ways to accomplish the mission.

Panel operating rules

Each seat must provide a distinct assessment.

The panel must:

- Identify agreement and disagreement.
- Challenge conclusions rather than merely endorse them.
- Explain why an alternative is better or worse.
- Resolve disagreements with evidence and reasoning.
- Record unresolved disagreement rather than manufacturing consensus.

Do not claim three independent AI agents were executed unless that actually occurred. The three seats are a structured RACE deliberation framework; accurately describe how their perspectives were produced.

The permanent panel must remain recognizable in every deliverable.

---

3. ARCHITECTURAL REPLACEMENT AND ELIMINATION AUTHORITY

This assignment expressly rejects preservation of existing HERALD components merely because they already exist.

Claude Code is authorized to investigate and recommend complete replacement, consolidation, separation, redesign, or elimination of any component, module, abstraction, dependency, workflow, or architectural layer.

The authority is based on the following principle:

If an aspect of HERALD does not directly support its overarching intent and required functionality, it does not deserve automatic preservation.

When a better way to accomplish the same mission exists, investigate it seriously.

Permitted recommendations include:

- Replacing an existing implementation entirely.
- Rebuilding a capability using a different technical approach.
- Removing duplicated functionality.
- Eliminating unnecessary abstractions.
- Combining overlapping components.
- Separating improperly coupled responsibilities.
- Replacing an existing dependency with a more appropriate one.
- Removing functionality that does not support HERALD's intended purpose.
- Reconsidering substantial portions of the architecture.

Complete elimination is an acceptable recommendation when justified by evidence.

However, this authority is not an instruction to destroy components indiscriminately. Every proposed elimination must identify:

1. What the component currently does.
2. Whether that function is actually required.
3. Whether another component already provides it.
4. Whether it has downstream consumers.
5. What would replace the required functionality, if anything.
6. What would break if it disappeared.
7. How the transition would occur safely.

Phase 0 may recommend complete elimination but must not execute it.

Do not confuse architectural freedom with permission to make unapproved code changes.

---

4. OPERATING BOUNDARIES

Phase boundary

Phase 0 is read-only with respect to HERALD and all inspected dependency repositories.

Allowed:

- Repository and source inspection.
- Test inspection.
- Safe execution of existing tests where the environment permits.
- Static analysis and dependency analysis.
- Git history, branch, tag, and release inspection.
- Contract and interface comparison.
- Safe, non-mutating adversarial analysis.
- Creation of Phase 0 reports outside the inspected Git worktrees.

Prohibited:

- Editing source code.
- Editing tests.
- Editing README or other tracked repository documentation.
- Adding or changing dependencies.
- Changing configuration.
- Merging or rebasing branches.
- Deleting branches.
- Committing or pushing.
- Creating tags or releases.
- Publishing packages.
- Running destructive experiments against connected systems.

Do not create test results by modifying a test to make it pass.

If safe execution is impossible, record that limitation.

Evidence classifications

Every material statement must be distinguished as:

- EXECUTED: The behavior or command was actually executed and observed.
- INSPECTED: Source, configuration, tests, documentation, or Git state was directly examined.
- INFERRED: A conclusion logically derived from available evidence.
- UNKNOWN: Not established.

A test found in source code is not an executed test.

A connector is not proof of a working integration.

A README statement is not proof of runtime behavior.

A passing test is not proof of complete security.

Repository scope

Start with the canonical HERALD repository:

"https://github.com/wking53214/HERALD"

Verify repository identity before proceeding.

Inspect the accessible local clone and/or GitHub repository. Record which inspection method was used and any limitations.

Inspect relevant upstream and downstream repositories only where evidence indicates an actual dependency, interface, consumer, or integration relationship.

Do not assume access to a repository that was not inspected.

---

5. ESTABLISH THE VERIFIED BASELINE

Establish a precise snapshot of HERALD.

Inspect and report:

Repository identity and state

- Repository name and visibility.
- Main branch and exact HEAD commit.
- Current working-tree state, if locally available.
- Current package version.
- Python and platform compatibility.
- Repository structure.
- Public entry points and exported interfaces.
- Current architecture and component inventory.

Git and collaboration hygiene

- All branches.
- Branch divergence from main.
- Unique commits on each branch.
- Whether branches contain useful, obsolete, or duplicate work.
- Open and closed pull requests relevant to the current code.
- Unmerged work.
- Stale branches.
- Tags.
- Published releases.
- Release notes and changelog.
- Whether branch cleanup is safe or requires approval.

Never delete a branch during Phase 0.

Dependencies and build

- Direct and transitive dependencies.
- Version constraints and pins.
- Git-based dependencies and referenced tags or commits.
- Floating dependencies.
- Lockfiles or reproducible dependency definitions.
- Build configuration.
- Package metadata.
- Supply-chain concerns.
- External runtime requirements.

CI and testing

- CI workflows.
- Triggers and actual available run results.
- Action versions and pinning.
- Test discovery and coverage configuration.
- Linting, security scanning, and type-checking.
- Skipped, disabled, or conditionally executed tests.
- Fixtures and test data.
- Historical test counts versus current executable tests.

Clearly distinguish current CI evidence from historical README statements.

If the GitHub interface or local environment does not expose a result, mark it UNKNOWN. Do not infer green or red status from an empty response.

Licensing

- License metadata.
- LICENSE and NOTICE files.
- Third-party dependency licensing where material.
- Any apparent inconsistencies.

---

6. INDEPENDENT SOURCE-LEVEL CODE REVIEW

Read the implementation, not just its documentation.

Inspect all significant production modules, public APIs, data structures, trust-boundary code, connectors, export paths, and tests.

Create an architecture map showing:

- Major modules.
- Responsibilities.
- Entry points.
- Data flow.
- Trust boundaries.
- External dependencies.
- Internal dependencies.
- Public interfaces.
- Error and failure paths.
- Persistence and export mechanisms.
- Integration points.

Identify:

- Dead or unreachable code.
- Duplicated responsibilities.
- Unused or misleading interfaces.
- Mutable state that affects trust.
- Validation gaps.
- Inconsistent error handling.
- Implicit assumptions.
- Hidden coupling.
- Inadequately tested paths.
- Misleading comments and documentation.
- Capabilities promised but not implemented.

Do not treat the previous audit as definitive. Revalidate every finding against current source.

---

7. REASSESS THE PREVIOUS FINDINGS

The following are leads from the previous audit, not established current facts. Recheck each one independently.

ID| Previous finding| Required investigation
F-01| Confirmation/claim mismatch| Does confirmation bind to the exact claim being evaluated?
F-02| Per-kind threshold validation| Are all thresholds finite, valid, and bounded?
F-03| Confirmation integrity exceptions| Do implementation, tests, and API contract agree?
F-04| Gate boundary revalidation| Are claims fully revalidated at every trust boundary?
F-05| Cross-process authentication| Can independent processes verify exports and signatures?
F-06| Forged HUMAN_CONFIRMED provenance| Can human-confirmed status be manufactured without verified confirmation?
F-07| Unknown extractor acceptance| Do unknown extractor identifiers fail closed?
F-08| Human identity authentication| Is a claimed identity actually authenticated?
F-09| Non-finite numeric values| Can NaN, infinity, or invalid numerical data bypass logic?
F-10| Confirmation registry race| Are concurrency, replay, expiration, and claim binding safe?
F-11| Floating-point monetary values| Is precision appropriate for monetary and consequential values?
F-12| Extraction and calibration limitations| Are extraction coverage and confidence calibration adequate?
F-13| Documentation accuracy| Are architecture notes and documented behavior current?
F-14| CNS/UAI-1 integration| How mature and interoperable is the current connector?
F-15| Release and branch hygiene| Is the repository clean, reproducible, and ready for release?

For each:

- Confirm, revise, downgrade, upgrade, or reject.
- Identify exact supporting source.
- Identify the relevant test coverage.
- State whether the issue was reproduced.
- Record downstream implications.
- Recommend its preliminary disposition.

Add newly discovered findings using unique identifiers.

Historical hygiene leads

The previous audit also recorded the following items for revalidation:

- Historical main HEAD: "b0a3f28362f9e63ac57436b34e793f760c36fde3".
- Historical package version: "0.3.0".
- The dependency declaration referenced CNS "v2.3.0" while an adjacent comment reportedly referenced "v2.2.0".
- Historical branch names included:
  - "claude/audit-export-signatures"
  - "fix/hmac-sha256-key-id"
  - "fix/unused-source-accepted-import"
- The signature branch reportedly contained optional Ed25519 export-signature work and cross-process verification tests.
- The HMAC branch reportedly diverged from main.
- The unused-source branch reportedly contained no unique commits.
- The previous audit found no published releases, no tag refs, and no root "CHANGELOG.md".
- Pytest and Bandit were reportedly not exactly pinned in CI.
- GitHub Actions used mutable major-version references such as "actions/checkout@v4" and "actions/setup-python@v5".
- "ARCHITECTURE_GHOSTS.md" reportedly described tests as skipped even though the current tests appeared to execute assertions.
- A mismatch reportedly existed between source-verification requirements described in documentation and permissive "ConfidenceGate()" defaults.

These are historical observations. Verify current state and exact details before making conclusions.

Do not delete or merge the historical signature or HMAC branches simply because they look stale.

---

8. HERALD'S PURPOSE AND ARCHITECTURAL BOUNDARIES

Establish HERALD's intended mission from its Constitution, public contracts, implementation, research documents, and established project intent.

Do not blindly preserve accidental behavior merely because it exists in code.

Evaluate whether HERALD's responsibilities are appropriately separated into:

- Source extraction.
- Evidence representation.
- Claim construction.
- Claim validation.
- Confidence assessment.
- Human confirmation.
- Provenance.
- Export and verification.
- Evidence persistence.
- Calibration and evaluation.

Explicitly distinguish these from responsibilities that may belong elsewhere:

- Consequence governance.
- Policy decisions.
- Authorization.
- Enterprise identity management.
- External trust-root administration.

Review "HERALD_CONSEQUENCE_GOVERNANCE_RESEARCH.md" and determine whether keeping consequence governance outside HERALD remains architecturally sound.

Do not expand HERALD into a general governance or authorization engine unless evidence and an explicit change in project intent justify that conclusion.

---

9. CNS AND UAI-1 INTEGRATION REVIEW

Independently reassess the actual HERALD-to-CNS integration.

Inspect, at minimum, where present:

- "HeraldSourceGate"
- "HeraldConfidenceGate"
- "full_chain()"
- "run_governed()"
- "cns_chain()"
- "herald/cns_connector.py"
- Corresponding connector tests.
- Actual CNS contract definitions and version compatibility.

Investigate:

1. ALPHA source-side entry.
2. OMEGA claim-side exit.
3. Source-to-claim lineage.
4. Gate status behavior.
5. Failure propagation.
6. Claim and evidence binding.
7. Contract-version compatibility.
8. Cross-process operation.
9. Behavior when source documents are absent.
10. Whether the connector works independently of the full governed path.
11. Whether the implementation is genuinely interoperable or merely locally compatible.
12. What UAI-1 capabilities are present, missing, or only proposed.

Distinguish endpoint architecture from general bidirectional peer-to-peer communication.

Preserve CNS's intended role as a thin, stdlib-only contract and binding layer. CNS passes and binds objects; it must not become HERALD's evidence authority, policy engine, or authorization engine.

Keep native component digests distinct from CNS binding digests. A CNS binding digest is not an authorization grant.

Identify which improvements can remain entirely within HERALD and which would require a CNS contract change.

Do not assume that a CNS change is necessary simply because HERALD has an integration limitation.

---

10. DOWNSTREAM DEPENDENCY DISCOVERY

This is a mandatory and central part of Phase 0.

Identify all actual upstream and downstream dependencies relevant to HERALD.

At minimum, investigate the possibility of relationships with:

- CNS
- TIE
- CCC
- Conservation_Kernel
- Governance_Gateway
- CCCb
- Other STACK repositories established by source references, dependencies, data flow, or actual integration evidence.

Do not claim an integration simply because two repositories are part of STACK.

For each verified relationship, capture:

Dependency identity

- Repository and exact version/commit inspected.
- Direct or indirect relationship.
- Producer and consumer.
- Direction of data or control flow.
- Integration mechanism.
- Actual implementation versus planned integration.

Contract inventory

Identify:

- Protocols.
- Dataclasses and schemas.
- Field names and types.
- Status values.
- Error semantics.
- Digests and signature formats.
- Version constraints.
- Export/import formats.
- Identity assumptions.
- Required validation.
- Compatibility expectations.

Change impact

Identify what a HERALD modification could affect:

- Upstream inputs.
- Downstream consumers.
- CNS endpoints.
- TIE evidence intake and verification.
- Persistence or audit records.
- Claim lineage.
- Provenance.
- Signature verification.
- Existing historical data.
- Runtime behavior and failure propagation.

For every relationship, classify it as:

- VERIFIED DIRECT.
- VERIFIED INDIRECT.
- PLANNED ONLY.
- DOCUMENTED ONLY.
- INFERRED.
- UNKNOWN.

Do not promote a documented or inferred relationship to verified integration.

Dependency impact register

Every potential change must eventually have a record containing:

Field| Required content
Change ID| Unique proposed change
HERALD surface| Affected module, interface, or behavior
Upstream impact| Inputs and contracts affected
Downstream consumers| Actual affected systems
Contract impact| Fields, schemas, statuses, signatures, or versions
CNS impact| Whether a CNS change is required
Compatibility| Backward and forward compatibility concerns
Failure propagation| Consequence of mismatched versions
Migration| Required transition
Validation| Required integration tests
Evidence| Supporting source and classification

If a consumer cannot be inspected, explicitly identify the gap and do not guess its requirements.

---

11. SECURITY AND ADVERSARIAL ASSESSMENT

Perform a structured attack-surface review.

Investigate:

- Claim substitution.
- Claim mutation after validation.
- Forged human confirmation.
- Replay and stale confirmation.
- Forged provenance.
- Unknown extractor behavior.
- Missing source documents.
- Invalid source binding.
- HMAC key generation and lifecycle.
- Cross-process verification.
- Ed25519 implementation and trust model.
- Key distribution, rotation, revocation, and compromise.
- Tampered exports.
- Numerical edge cases.
- Concurrency and race conditions.
- Unauthenticated human identity assertions.
- Downstream acceptance of unverified output.

Review the optional Ed25519 branch independently if it remains available.

Determine whether it:

- Solves a real architectural need.
- Can be integrated safely.
- Requires adaptation.
- Introduces unnecessary dependencies.
- Leaves key ownership unresolved.
- Provides cross-process verification in practice.
- Is compatible with TIE and other actual consumers.

Do not assume that Ed25519 automatically solves distributed trust.

Identify what HERALD itself can guarantee and what requires external identity, key-management, or governance infrastructure.

Do not conduct destructive or unauthorized attacks against external services or production systems.

---

12. FACP CAMPAIGN

Apply the Formalized Adversarial Campaign & Closure Protocol as a discovery framework.

Stage A — Baseline

Establish exact repository, code, dependency, branch, and release state.

Stage B — Independent inspection

Inspect implementation, tests, contracts, and documentation.

Stage C — Seam assessment

Map actual HERALD interfaces and upstream/downstream relationships.

Stage D — Adapter and alternative assessment

Identify where existing interfaces can be retained, adapted, replaced, or eliminated. No adapters are implemented.

Stage E — Adversarial assessment

Inspect plausible attack paths and test coverage. Execute safe existing tests when possible, but do not change code.

Stage F — Closure assessment

Determine what is established, unresolved, and ready for deeper Phase 1 research.

Phase 0 does not remediate defects and does not certify HERALD.

---

13. PHASE 0 REQUIRED DELIVERABLES

Produce a complete kickoff package.

The package must be sufficiently detailed that Phase 1 can begin from it without repeating broad repository discovery.

Deliverable 1 — Executive assessment

State:

- Current HERALD condition.
- Architectural strengths and weaknesses.
- Security posture as established by evidence.
- Integration maturity.
- Major risks.
- Overall readiness and limitations.

Do not invent a score. If a score is useful, define its criteria and evidence first.

Deliverable 2 — Verified repository baseline

Exact HEAD, version, branch state, release/tag state, dependencies, CI, tests, and inspection limitations.

Deliverable 3 — Source and architecture inventory

Component list, public interfaces, source locations, responsibilities, data flow, and trust boundaries.

Deliverable 4 — Confirmed findings register

All validated and newly discovered findings, evidence, severity, disposition, and remediation/research questions.

Deliverable 5 — Security and adversarial report

Threats, attack paths, existing defenses, test coverage, unverified assumptions, and external trust requirements.

Deliverable 6 — CNS/UAI-1 assessment

Actual connector architecture, contract compatibility, verified ALPHA/OMEGA behavior, missing capabilities, and proposed research.

Deliverable 7 — Downstream dependency map

Verified upstream/downstream systems, integration evidence, consumers, contracts, and unknown relationships.

Deliverable 8 — Contract and interface inventory

Exact relevant interfaces, schemas, status values, digest/signature formats, version requirements, and compatibility assumptions.

Deliverable 9 — Architectural boundary assessment

What HERALD should own, consume, delegate, replace, separate, or eliminate.

Deliverable 10 — Proposed modification register

Every potential correction, improvement, integration, replacement, or elimination.

Each entry must have:

- Unique ID.
- Evidence.
- Classification.
- Description.
- Business/architectural reason.
- Disposition: KEEP / INTEGRATE / ADAPT / PARTIAL / SEPARATE / DEFER / REJECT / NO ACTION.
- Priority: P0 / P1 / P2 / P3.
- Downstream impact.
- Compatibility and migration questions.
- Phase 1 research requirements.

Deliverable 11 — Unresolved questions register

Every important question that cannot be answered from current evidence, including why the question matters and what source or investigation could resolve it.

Deliverable 12 — Phase 1 research agenda

A prioritized list of investigations that Phase 1 must perform.

For each research item specify:

- Finding or opportunity that triggered it.
- Question to answer.
- Alternative architectures to investigate.
- Required repositories and interfaces.
- Downstream systems to consider.
- Decision criteria.
- Evidence needed for a decision.

Deliverable 13 — Phase 1 kickoff package

Create a self-contained package with these files, or equivalent clearly named sections if the environment cannot create external files:

1. "PHASE0_EXECUTIVE_AND_KICKOFF.md"
2. "PHASE0_FINDINGS_REGISTER.csv"
3. "PHASE0_DEPENDENCY_REGISTER.csv"
4. "PHASE0_CONTRACT_INVENTORY.csv"
5. "PHASE0_QUESTIONS_AND_RESEARCH_AGENDA.md"
6. "PHASE0_SOURCE_INDEX.md"
7. "PHASE0_MANIFEST.json"

The executive and kickoff document must explain how to use the package.

The manifest must record:

- Repository identity.
- Exact HERALD commit and version inspected.
- Inspection date.
- Inspected dependency repository commits/versions, where available.
- Deliverable filenames.
- Finding and dependency identifiers.
- Completeness status.
- Known omissions.
- Whether Phase 1 entry criteria are met.

Create report artifacts outside the inspected Git worktrees. Do not dirty the repositories merely to store audit output. If a suitable external location is unavailable, provide the complete artifacts in the response.

---

14. SECONDARY WORKSTREAM — INDEPENDENT RACE PERFORMANCE EVALUATION

This is a separate research assignment running alongside the primary HERALD review.

It is the first field evaluation of the new RACE structure with its three permanent seats.

It must not interfere with, redirect, or change the primary HERALD assignment.

The evaluation is independent research. It does not have to stack on, inherit, or accept any conclusions from an earlier RACE evaluation report.

Evaluation objective

Determine whether the three-seat RACE structure is genuinely useful or whether it is a hindrance.

Do not presume that the structure works merely because it was designed to work.

Evaluate the following

A. Permanent-seat contribution

- Did UCO contribute strategic or architectural insights that would otherwise have been missed?
- Did Hacker identify materially different risks?
- Did MacG discover simpler or better engineering solutions?
- Did the seats provide complementary work or repeat each other?
- Were disagreements productive?

B. Analytical quality

- Did RACE discover issues a conventional single-perspective review might miss?
- Did the structure improve evidence quality?
- Did it improve downstream dependency discovery?
- Did it expose flawed assumptions?
- Did it help distinguish facts from inference?

C. New capabilities
Identify any demonstrably new capability arising from:

- The three permanent seats.
- Structured deliberation.
- Cross-seat challenge.
- Dependency-aware reasoning.
- Explicit disposition and evidence registers.
- Phase-specific gates and handoffs.

Separate genuinely demonstrated capabilities from marketing-style claims.

D. Operational overhead

- Repetition.
- Unnecessary process.
- Excessive report length.
- Token and context consumption, if measurable.
- Slower progress.
- Conflicting or low-value analysis.
- Any point where RACE obstructed useful work.

Do not invent token or time measurements.

E. Net value verdict

Use one of these outcomes:

- HELP.
- PARTIAL HELP.
- NEUTRAL.
- HINDRANCE.
- INCONCLUSIVE.

Support the verdict with specific evidence from this Phase 0 execution.

Independent output

Produce a standalone report named:

"RACE_PHASE0_INDEPENDENT_EVALUATION.md"

It must be presented as a separate report, not embedded as a finding in the HERALD technical assessment.

Include:

- What worked.
- What did not.
- What was genuinely new.
- What each seat contributed.
- Where the seats overlapped.
- Whether disagreements improved the work.
- What created overhead.
- Net value verdict.
- Concrete recommendations for future RACE use.

Do not use this report to alter the HERALD findings or priorities.

Do not rely on or require a later Phase 1 RACE evaluation to make this report complete.

---

15. PHASE 0 QUALITY GATE

Phase 0 is complete only when:

- The repository baseline is established.
- The major production implementation has been inspected.
- Previous findings are revalidated.
- New findings are documented.
- Security and trust boundaries are assessed.
- CNS integration is inspected.
- Actual downstream relationships are mapped.
- Contract and interface inventory is established.
- Replacement and elimination opportunities are identified.
- Unknowns are explicit.
- Phase 1 research questions are prioritized.
- The kickoff package is self-contained.
- The secondary RACE evaluation is separately produced.

If evidence is incomplete, say so. Do not declare completion merely because every section has a heading.

Phase 0 exit status

Return exactly one:

- "READY FOR PHASE 1"
- "READY FOR PHASE 1 WITH DOCUMENTED GAPS"
- "NOT READY FOR PHASE 1"

Explain the decision.

Phase 1 must not be considered ready merely because a report was generated.

---

16. FINAL AUTHORIZATION BOUNDARY

PHASE 0 ONLY.

No production code changes.

No test changes.

No repository documentation changes.

No commits, pushes, merges, branch deletions, tags, or releases.

Complete architectural replacement and elimination are authorized as subjects of investigation and recommendation. They are not to be executed in Phase 0.

Deliver the full HERALD kickoff package and the separate RACE evaluation report.

Then stop.

Do not begin Phase 1 automatically. Phase 1 requires the completed Phase 0 output as explicit input.
