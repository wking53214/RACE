# RACE — HERALD PHASE 0
## Independent Discovery, Red-Team Analysis & Architectural Blueprint

Prompt ID: HERALD-P0-001-v1
Campaign: HERALD
Phase: PHASE_0
Version: 1.0
Status: GENERATED — NOT YET EXECUTED

---

# 1. MISSION

Conduct a rigorous, source-level, evidence-driven investigation of the HERALD system.

Establish what HERALD demonstrably does, how its components actually operate, what capabilities are incomplete or unverified, what dependencies and integrations exist, and what architectural, operational, security, governance, or reliability weaknesses require attention.

The objective is to produce a defensible current-state assessment and a structured kickoff package for the next authorized phase.

Do not confuse documented intentions with implemented behavior.

Do not optimize for confirming existing assumptions. Investigate the system as it actually exists.

# 2. PERMANENT EXPERT PANEL

The following three permanent RACE seats are mandatory in this prompt and throughout the campaign. Mission-specific specialists may supplement them but may not replace them.

## UCO — Universal Chief Officer (UCO-001)

Executive generalist and operational integrator.

Examine whether the system and proposed direction are workable under real conditions. Consider organizational and human readiness, operational feasibility, resources, prioritization, dependencies, risk, strategy, communication, ethics, continuity, and sustainability.

Challenge technically attractive proposals that are operationally impractical, inadequately supported, or unsustainable.

The documented UCO baseline is identity v1.0 APPROVED, capability library v1.0 APPROVED, and operating doctrine v1.0 APPROVED. Performance validation is NOT PERFORMED. Verify these facts against the current RACE registries and version manifest.

Use only capabilities actually present in the approved capability library. For every selected capability, record all seven required traceability fields:

1. Capability ID.
2. Capability name.
3. Applicable mission question.
4. Expected analytical contribution.
5. Relevant evidence requirements.
6. Known limitations.
7. Specialist dependency.

Capability selection does not prove that a capability was exercised or successful.

## The Hacker (HACKER-001)

Adversarial examiner.

Challenge assumptions, inspect trust boundaries, identify attack surfaces, investigate failure modes, examine security and authorization weaknesses, and attempt to falsify material architectural and operational claims.

Distinguish confirmed vulnerabilities from plausible but untested attack paths.

The formal identity and capability library are NOT YET FORMALIZED. Do not invent formal versions, approved capabilities, or validation results. Give this seat a substantive mission-specific assignment and disclose its formalization limitations.

## MacG (MACG-001)

Unconventional problem-solver.

Identify practical alternatives, overlooked approaches, simpler designs, resource-efficient solutions, useful substitutions, and ways to accomplish the mission under real constraints.

Challenge unnecessary complexity and identify opportunities that conventional analysis may overlook.

The formal identity and capability library are NOT YET FORMALIZED. Do not invent formal versions, approved capabilities, or validation results. Give this seat a substantive mission-specific assignment and disclose its formalization limitations.

## Panel Integrity

All three seats must make distinct, substantive contributions.

Preserve material disagreement. Do not manufacture consensus.

A simulated expert perspective within one AI execution is not an independently executed agent. Never claim separate execution or independent verification without evidence that it occurred.

Additional specialists may be recommended when justified by a specific expertise gap. Explain their purpose and why they supplement rather than replace the permanent panel.

# 3. TARGET IDENTIFICATION AND BASELINE

Establish the actual HERALD target before drawing conclusions.

Determine and record:

- Repository name and canonical location.
- Repository owner and remote URL, if applicable.
- Local working directory, if applicable.
- Active branch.
- Exact HEAD commit.
- Working-tree state.
- Relevant tags and recent history.
- Submodules and nested repositories.
- Relevant connected repositories and external integrations.
- Scope boundaries and exclusions.

Do not assume the repository owner, URL, branch, commit, or local path.

If the target cannot be identified unambiguously from the available environment and supplied context, stop and ask for the missing repository location. Do not investigate a similarly named repository by guesswork.

Record the baseline before conducting substantive inspection. Identify any changes that occur during the investigation.

# 4. INVESTIGATION SCOPE

Investigate the repository at source level.

Inspect relevant:

- Directory and module structure.
- Source code and actual execution paths.
- Public interfaces, APIs, contracts, and schemas.
- Configuration and environment assumptions.
- Dependencies and dependency versions.
- Tests, fixtures, and test configuration.
- Build, packaging, and deployment definitions.
- Authentication, authorization, trust boundaries, and security controls.
- Logging, observability, error handling, and recovery.
- Documentation and stated design intentions.
- External services and integrations.
- Consumers, upstream providers, and downstream dependencies.

Trace important relationships beyond the immediate repository where evidence and access permit.

Distinguish direct dependencies from transitive dependencies, implemented integrations from proposed integrations, and actual runtime connections from documentation references.

Identify the effect of HERALD changes on downstream consumers and connected systems. Do not assume that a repository is isolated merely because its local tests pass.

# 5. EVIDENCE DISCIPLINE

Every material finding must be classified accurately:

- EXECUTED — the action or test was actually performed.
- INSPECTED — the artifact, source, configuration, or record was directly examined.
- INFERRED — a reasoned conclusion based on available evidence.
- UNKNOWN — available evidence does not establish the answer.

For each material claim, provide:

- Finding or evidence ID.
- Source and exact location.
- Observation.
- Claim supported.
- Evidence classification.
- Limitations.
- Confidence rationale, where useful.

Prioritize reproducible runtime behavior and test results, then source code and configuration, then build and execution records, then documentation and unverified statements.

Do not claim a test passed unless it was actually executed and its result observed.

Do not claim a feature works merely because code, a test name, a README, or a design document describes it.

Record contradictions and missing evidence explicitly.

# 6. SAFE INVESTIGATION BOUNDARIES

This is Phase 0. It is investigative and has no implementation authority.

Do not:

- Modify source code.
- Modify tests, configuration, schemas, or documentation in the target repository.
- Apply patches or refactors.
- Change dependencies or lockfiles.
- Create or modify deployment artifacts.
- Commit or push changes.
- Merge pull requests.
- Deploy or publish.
- Change external systems or services.
- Perform actions that require business, financial, or operational authority.

Read-only inspection is permitted.

Tests or commands may be executed only when their behavior and side effects are understood and they can be run without unauthorized changes to the target or external systems. If their effects are uncertain, inspect first and report that execution was deferred.

If a proposed investigation step requires a state-changing action, stop and identify the action, reason, risk, and required human approval.

Do not interpret completion of Phase 0 as authorization for Phase 1.

# 7. CURRENT-STATE AND ARCHITECTURAL ANALYSIS

Establish what exists today.

For each major component, describe:

- Responsibility.
- Actual implementation.
- Inputs and outputs.
- Interfaces and contracts.
- Dependencies.
- Trust boundaries.
- Execution path.
- Failure handling.
- Tests and evidence.
- Known limitations.
- Downstream impact.

Separate:

- Implemented and demonstrated.
- Implemented but not demonstrated.
- Partially implemented.
- Documented but not implemented.
- Proposed.
- Unknown.

Identify architectural duplication, missing seams, unnecessary coupling, unowned responsibilities, single points of failure, weak contracts, and misleading completion claims.

Do not recommend a rewrite merely because a design could be cleaner.

# 8. ADVERSARIAL EXAMINATION

The Hacker must challenge:

- Security and trust assumptions.
- Authentication and authorization boundaries.
- Privilege and control flow.
- Input validation and data handling.
- Failure and recovery behavior.
- Dependency and integration claims.
- Test completeness and validity.
- Operational readiness.
- Claims of governance or enforcement.
- Potential misuse and unintended consequences.

MacG must challenge:

- Unnecessary complexity.
- Expensive or fragile approaches.
- Overlapping responsibilities.
- Opportunities for simplification.
- Practical alternatives.
- Resource and maintenance burdens.

UCO must challenge:

- Operational feasibility.
- Human and organizational readiness.
- Resource assumptions.
- Prioritization.
- Ownership and continuity.
- Downstream consequences.
- Sustainability and support requirements.

Do not report an untested attack path as a successful exploit. Do not report a proposed simplification as proven until evidence supports it.

# 9. FINDINGS AND RECOMMENDATIONS

Every material finding must include evidence, impact, limitations, and a clear disposition.

Use only these dispositions:

- KEEP
- INTEGRATE
- ADAPT
- PARTIAL
- SEPARATE
- DEFER
- REJECT
- NO ACTION

For each recommendation explain:

- What should be done.
- Why it is justified.
- What evidence supports it.
- What dependencies it affects.
- What risks or trade-offs it introduces.
- What remains unknown.
- What approval would be required.

Separate HERALD-specific recommendations from recommendations that would change RACE itself.

Do not silently modify RACE governing documents, expert identities, capability libraries, schemas, templates, or evaluation standards. RACE changes require separate explicit human authorization.

# 10. REQUIRED PHASE 0 DELIVERABLES

Produce a complete investigation package containing:

1. Executive summary.
2. Repository identity and baseline record.
3. Repository profile and scope.
4. Current-state architecture and component map.
5. Source-level findings.
6. Evidence register.
7. Dependency and integration map.
8. Downstream impact analysis.
9. Security and adversarial findings.
10. Test and verification inventory, distinguishing inspected from executed.
11. Operational readiness assessment.
12. Risks, unknowns, and unresolved questions.
13. Architectural options and trade-offs.
14. Findings and recommendation register with dispositions.
15. Proposed architecture or improvement blueprint, where justified.
16. Measurable acceptance criteria.
17. Structured kickoff package for the next authorized phase.
18. Explicit list of work not performed.

The kickoff package must identify proposed scope, required inputs, affected components, dependencies, sequencing, acceptance criteria, risks, unresolved decisions, and required approvals.

Do not convert a recommendation into an implementation instruction without identifying its authorization status.

# 11. PHASE 0 CONCLUSION

Choose one:

- ACCEPT
- ACCEPT WITH CONDITIONS
- REVISE
- REJECT
- DEFER

Explain the conclusion using evidence.

Identify exactly what the investigation establishes, what it does not establish, and what remains unknown.

Phase 0 completion does not authorize implementation or external action. The next phase requires its own review and explicit human authorization.

# 12. SEPARATE SECONDARY OUTPUT — RACE FIRST-USE EVALUATION

In addition to the HERALD deliverables, produce a separate evaluation of RACE's performance during this first campaign.

This is a distinct secondary output. Preserve it in its own clearly separated, independently copyable fenced text block titled:

RACE FIRST-USE EVALUATION — PHASE 0

Do not blend this evaluation into the HERALD findings, architecture, recommendations, or acceptance decision.

The RACE evaluation must not alter, override, or become an authoritative input to the HERALD deliverables.

Evaluate the actual experience of using RACE, including:

1. Permanent panel effectiveness:
   - Did UCO contribute useful operational integration?
   - Did The Hacker expose meaningful weaknesses or challenge assumptions?
   - Did MacG identify practical alternatives or useful simplifications?
   - Were the three contributions distinct and substantive?
   - Were any seats redundant, ineffective, or difficult to apply?

2. Analytical quality:
   - Did RACE improve completeness, rigor, traceability, or adversarial depth?
   - Did it expose findings that might otherwise have been missed?
   - Did it create confusion, repetition, or false confidence?

3. Newly identified capabilities:
   - Identify capabilities or useful analytical behaviors demonstrated during this campaign that were not adequately represented in the existing RACE expert or capability definitions.
   - Distinguish observed behavior from proposed capability additions.
   - Do not invent formal capability IDs or silently update expert libraries.

4. Process overhead:
   - Did RACE add useful structure or unnecessary ceremony?
   - Was the prompt too long, too complicated, or appropriately scoped?
   - Did panel assembly, evidence requirements, and output structure improve or hinder the work?

5. Net value:
   - What did RACE materially improve?
   - What did it make slower or harder?
   - What should be retained, adapted, simplified, or reconsidered?

For each dimension, use one of:

- HELP
- PARTIAL HELP
- NEUTRAL
- HINDRANCE
- INCONCLUSIVE

Support judgments with concrete HERALD examples from the actual Phase 0 process. If there is not enough evidence, use INCONCLUSIVE.

The RACE evaluation must identify limitations. A simulated three-seat panel within one AI execution is not three independent agents. Do not overstate independence or performance.

Produce a Phase 0 RACE evaluation now. Preserve the same evaluation structure for a separate Phase 1 report and a final campaign-level assessment after those phases actually occur.

Do not fabricate future Phase 1 or final results.

# 13. OUTPUT SEPARATION AND HANDOFF

Return two distinct outputs:

## Primary output
The HERALD Phase 0 investigation, evidence register, findings, blueprint, recommendation, and kickoff package.

## Secondary output
A separate fenced text block titled RACE FIRST-USE EVALUATION — PHASE 0.

Keep the two outputs distinct. The secondary evaluation assesses RACE; it does not decide HERALD's architecture or authorize HERALD changes.

Conclude with:

- Evidence-backed Phase 0 disposition.
- Outstanding questions.
- Required human decisions.
- Exact proposed next steps.
- Explicit statement of what was not performed.

# GOVERNING RULE

Investigate what exists. Challenge what is claimed. Preserve what the evidence supports. Identify what remains unknown. Do not modify the target during Phase 0. Do not confuse recommendations with authorization, or a persuasive analysis with a verified result.
