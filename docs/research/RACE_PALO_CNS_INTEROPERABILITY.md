# RACE × PALO × CNS
## Comparative Governance Research and Interoperability Opportunity

**Document type:** Architecture and ecosystem research
**Date:** 2026-11-03
**Status:** Research findings and proposed direction
**Implementation status:** NOT IMPLEMENTED
**Integration status:** NOT TESTED
**Authorization:** No implementation or external integration authorized by this document

---

# 1. Executive Summary

RACE was initially conceived as an engine for AI prompt engineering: a repeatable process for transforming a human objective into a high-quality, mission-specific AI execution prompt.

Its design has developed into something broader.

RACE does not merely optimize prompt wording. It structures the work that happens before, during, and after an AI assignment:

- Define the human objective.
- Establish scope and constraints.
- Investigate the existing situation.
- Separate evidence from assumptions and unknowns.
- Apply mandatory adversarial and problem-solving perspectives.
- Develop a defensible blueprint.
- Establish authorization boundaries.
- Construct controlled AI execution instructions.
- Define evidence-based verification and closure.

This makes RACE a candidate **AI mission-governance framework**, with prompt construction as its practical output.

Public research into the PALO Framework identifies a complementary governance ecosystem. PALO addresses AI lifecycle governance, use-case classification, impact assessment, controls, measurement, evidence, and review. Its PALO-AM methodology addresses agentic authority and delegated action. PALO-AI explores technical enforcement and evidence for agent actions, but remains a Developer Preview with explicit production limitations.

The potential architectural relationship is:

- **RACE:** Governs the individual mission or assignment given to AI.
- **PALO:** Governs the broader AI use case, system lifecycle, risks, controls, and assurance.
- **CNS:** Could provide a shared interoperability and integrity boundary between independently governed systems.
- **STACK evidence components:** Could support provenance, evidence preservation, transformation integrity, artifact admission, and claim continuity.

These are complementary responsibilities, not a reason to merge the repositories.

The recommended direction is to preserve RACE as an independent project and investigate a standards-based exchange with PALO through CNS.

No uniqueness, production readiness, or integration success is claimed.

# 2. RACE: Current Purpose and Architectural Boundary

## 2.1 What RACE is

RACE — Red-Team Analysis, Construction & Evaluation — is a governed framework for transforming human objectives into disciplined, mission-specific AI execution prompts.

Its central premise is that a prompt should be treated as a governed assignment rather than merely a collection of instructions.

A properly formed assignment should establish:

- Human objective and desired outcome.
- Mission scope and constraints.
- Available resources.
- Required source evidence.
- Deliverables.
- Acceptance criteria.
- Authorization boundaries.
- Known uncertainties.
- Required expert perspectives.
- Verification and closure requirements.

## 2.2 Three-phase operating model

### Phase 0 — Discovery, Investigation, and Blueprint

Determines what is actually required, what is known, what remains uncertain, and what should be done.

Phase 0 is investigative. It does not authorize implementation.

### Phase 1 — Controlled Construction

Translates an accepted blueprint into bounded implementation instructions and authorized work.

Phase 1 must not silently exceed the authorization granted by the human.

### Phase 2 — Verification and Closure

Inspects resulting artifacts, performs authorized testing, conducts adversarial retesting, compares outcomes with acceptance criteria, and records unresolved risks.

Completion of one phase does not automatically authorize the next.

## 2.3 Permanent expert panel

Every RACE mission retains three permanent expert seats:

1. **UCO — Universal Chief Officer:** Executive and operational integration, feasibility, organizational readiness, resource constraints, prioritization, risk, strategy, communication, ethics, continuity, and sustainability.
2. **The Hacker:** Adversarial examination, attack surfaces, exploit discovery, assumption challenges, and security weaknesses.
3. **MacG:** Resourcefulness, unconventional alternatives, practical engineering, and overcoming constraints.

Mission-specific experts may supplement these three seats but cannot replace them.

A critical limitation must remain explicit: multiple simulated perspectives in one AI execution do not establish independent agents or independent reviews.

## 2.4 Current implementation boundary

The RACE repository describes itself as a prompt-generation and governance framework.

It does not claim to be an independently operating execution engine, production authorization service, or runtime enforcement system.

Documentation and structured prompts do not, by themselves, prove that an external execution environment enforces the instructions.

RACE must preserve that distinction.

# 3. PALO: Public Governance Ecosystem

## 3.1 Overview

PALO is a public open-source AI governance framework maintained by Fabrizio Degni.

The public ecosystem includes three related but distinct components:

- **PALO Framework:** Broad AI lifecycle governance.
- **PALO-AM:** Agentic governance methodology, including delegated authority, autonomy, oversight, and reversibility.
- **PALO-AI:** Technical governance and enforcement concepts for agent actions.

The public project identifies its current baseline as PALO Framework v3.1.0 and PALO-AI v2.7.

The repository is MIT-licensed. Any future code reuse must retain the required license and copyright notices.

## 3.2 PALO lifecycle model

PALO organizes governance through six stages:

1. Frame — Define purpose, scope, ownership, and affected people.
2. Classify — Establish the risk route and level of scrutiny.
3. Assess — Evaluate impacts, authority, autonomy, and oversight.
4. Control — Assign owned, testable safeguards and gates.
5. Measure — Define indicators, thresholds, ownership, and review cadence.
6. Prove & Review — Assemble evidence and determine what must be reviewed or reopened.

PALO's current v3.1 public documentation describes:

- 12 applicability-aware governance control packs.
- 31 controls.
- 38 indicators.
- 10 evidence-contract families.

These are published framework counts, not independent proof that every control is effective in a deployed environment.

## 3.3 PALO's evidence orientation

PALO emphasizes converting governance requirements into reviewable artifacts.

Examples include:

- Use-case briefs.
- Risk routes.
- Impact records.
- Control plans.
- KPI/KRI registers.
- Evidence bundles.
- Review decisions.

Its public Evidence Pack workflow is designed to support local-first assessment and reviewable evidence generation.

PALO also distinguishes evidence from authority: the presence of an evidence artifact does not automatically establish that a decision or action is authorized.

## 3.4 PALO-AM

PALO-AM focuses on agentic systems and delegated authority.

Its relevant subject areas include:

- Agent identity.
- Delegated authority.
- Autonomy level.
- Oversight.
- Reversibility.
- Permitted action space.
- Assurance evidence.

This is adjacent to RACE because RACE defines the assignment and its boundaries, while PALO-AM examines the authority and autonomy of the agent operating within a broader system.

## 3.5 PALO-AI

PALO-AI explores technical governance of agent actions.

Its published concepts include:

- Policy evaluation.
- Action claims.
- Approval.
- One-time capabilities.
- Governed execution.
- Signed receipts.
- Outcome verification.
- Incident escalation.

These are potentially relevant to future RACE/CNS interoperability.

However, PALO-AI v2.7 is explicitly identified as a Developer Preview.

Its public integration documentation identifies unresolved production requirements, including:

- Production workload identity.
- Authenticated reviewer identity and separation of duties.
- Unavoidable governed execution.
- Distributed transactional state and exactly-once execution guarantees.
- KMS/HSM-backed key custody and rotation.
- High availability and recovery.
- Connector certification.
- Independent security assessment.

The preview is intended for isolated evaluation with mock or non-consequential tools.

**RACE must not represent PALO-AI as a production-ready authorization boundary.**

# 4. RACE and PALO: Complementary Responsibilities

## 4.1 The central distinction

RACE and PALO overlap in governance concerns, but their principal questions differ.

RACE asks:

> Is this particular assignment to AI properly defined, investigated, challenged, bounded, authorized, and evaluated?

PALO asks:

> Is this AI use case or system appropriately classified, assessed, controlled, measured, and supported by reviewable evidence throughout its lifecycle?

The distinction is between governing an individual mission and governing the broader AI use case or system in which missions occur.

This is a proposed architectural distinction, not a claim that the two frameworks have mutually exclusive capabilities.

## 4.2 Responsibility comparison

| Area | RACE | PALO |
|---|---|---|
| Human objective | Primary input | Use-case context |
| Mission scope | Primary responsibility | Broader system scope |
| Prompt construction | Primary responsibility | Not its central purpose |
| Adversarial mission analysis | Permanent panel requirement | Risk and control assessment |
| AI use-case classification | Could consume this information | Core lifecycle function |
| Impact assessment | Mission-specific considerations | Broader governance assessment |
| Agent authority | Defines assignment boundaries | PALO-AM methodology |
| Runtime action controls | Not currently claimed | PALO-AI preview |
| Acceptance criteria | Mission-specific | Controls and indicators |
| Evidence and review | Phase 2 and traceability | Lifecycle evidence and review |

## 4.3 What RACE should not become

RACE should not attempt to duplicate the entire PALO lifecycle framework.

It should not absorb PALO's control library, regulatory mappings, agentic authority methodology, or runtime implementation simply because those capabilities are relevant to some missions.

RACE should retain its mission-governance identity.

PALO should retain its broader AI lifecycle-governance identity.

# 5. The CNS Opportunity

## 5.1 Why CNS matters

CNS is a potential interoperability layer between independently governed systems.

The opportunity is not to make CNS the owner of RACE or PALO policy.

The opportunity is to allow independently governed systems to exchange structured, integrity-bound information without requiring either system to surrender its own decision authority.

The proposed division is:

- RACE owns mission semantics and prompt construction.
- PALO owns its governance methodology, controls, and lifecycle decisions.
- CNS provides shared contracts, identity and integrity bindings, and structured decision exchange.
- Receiving systems retain their own authorization and execution responsibilities.

## 5.2 Proposed exchange

A RACE mission package could eventually carry:

- Mission identifier.
- Mission version.
- Objective.
- Scope.
- Constraints.
- Required expert seats.
- Source evidence references.
- Findings and uncertainties.
- Blueprint.
- Prompt artifact reference.
- Acceptance criteria.
- Authorization record references.
- Phase status.
- Evidence and closure references.
- Content digest.
- Provenance information.

A PALO governance record could potentially provide:

- AI system and use-case context.
- Applicable risk route.
- Impact assessment.
- Relevant controls.
- Delegated authority context.
- Required safeguards.
- Indicators and thresholds.
- Evidence references.
- Accountable review records.

CNS could provide the binding and exchange mechanisms for these records.

## 5.3 Candidate integration pattern

1. RACE defines a mission.
2. RACE creates a versioned mission package.
3. PALO assesses the broader AI use case and relevant governance requirements.
4. The two systems exchange only the necessary structured records.
5. CNS binds exchanged artifacts to identity, version, subject, and integrity information.
6. Human decision-makers retain their respective authority.
7. The receiving execution environment applies its own policies and permissions.
8. Execution evidence is returned for evaluation and closure.

This is a proposed pattern. It has not been implemented or tested.

## 5.4 CNS must not become the policy authority

CNS must not silently acquire responsibility for:

- Defining RACE mission requirements.
- Defining PALO governance controls.
- Selecting the correct risk classification.
- Deciding whether a mission should proceed.
- Granting real-world permissions.
- Declaring evidence truthful.
- Declaring a mission successful.

CNS can bind and validate structured information according to agreed contracts.

Integrity is not truth. A valid digest is not authorization. A passed technical gate is not proof of successful execution.

These distinctions must remain explicit.

# 6. Potential STACK Evidence Integration

The existing STACK evidence components could provide useful support for RACE/PALO exchanges.

The following are candidate responsibilities, not claims of a completed integration.

| Component | Potential contribution |
|---|---|
| HERALD | Extract requirements, claims, and source-backed findings |
| TIE | Preserve source evidence and provenance |
| Conservation_Kernel | Preserve specified properties across transformations |
| Governance_Gateway | Evaluate artifact admission requirements |
| CCC | Maintain claim continuity and controlled status transitions |
| CNS | Bind identity, integrity, contracts, and structured exchange |

A possible evidence path is:

Human objective → RACE mission package → source evidence → governance assessment → approved assignment → execution evidence → verification → closure.

The actual routing, adapters, and component-level acceptance conditions require separate source-level investigation.

No claim is made that this complete path currently exists or has passed an end-to-end test.

# 7. A Controlled Comparative Experiment

The first practical step should be a controlled experiment rather than a software integration.

## 7.1 Test mission

Use a synthetic software-security mission:

> An AI coding assistant is asked to inspect a repository, identify a security weakness, explain its impact, and propose a remediation. It is explicitly prohibited from modifying files, executing consequential actions, or committing code.

Use the same mission description and source material for both systems.

## 7.2 RACE track

Have RACE produce:

- Phase 0 mission definition.
- Evidence and uncertainty register.
- Adversarial findings.
- Permanent expert panel contributions.
- Recommended blueprint.
- Proposed prompt.
- Acceptance criteria.
- Authorization boundaries.
- Phase 2 evaluation requirements.

Do not authorize implementation merely because a prompt has been generated.

## 7.3 PALO track

Use the relevant public PALO workflow to produce:

- Use-case context.
- Risk classification.
- Impact and authority assessment.
- Relevant controls.
- Required safeguards.
- Indicators and review conditions.
- Evidence bundle.

Use PALO-AI only in isolated evaluation if relevant. Do not use the Developer Preview to authorize consequential actions.

## 7.4 Comparison criteria

Compare the outputs against a predefined rubric:

1. Objective clarity.
2. Scope completeness.
3. Identification of affected systems and people.
4. Risk and failure-mode coverage.
5. Adversarial depth.
6. Authorization boundaries.
7. Evidence requirements.
8. Acceptance criteria.
9. Human accountability.
10. Traceability.
11. Operational usability.
12. Unresolved assumptions and uncertainty.

Use documented scoring anchors and retain the underlying evidence.

Do not declare a winner based on an informal impression or an arbitrary aggregate score.

The purpose is to identify complementary coverage, duplication, and gaps.

## 7.5 Independent review

Have reviewers who did not construct the respective outputs assess them against the same rubric.

Record:

- Reviewer identity or role.
- Materials reviewed.
- Evaluation method.
- Findings.
- Disagreements.
- Limitations.
- Final disposition.

Do not describe simulated expert perspectives as independent review.

# 8. Community and Open-Source Opportunity

PALO's public repository welcomes contributions.

Its documented contribution paths include:

- Regulatory mappings and citations.
- Control and KPI/KRI review.
- Examples and worked case studies.
- Translations.
- Accessibility improvements.
- Tests and report-generation checklists.
- Synthetic or safely publishable Casebook artifacts.

A RACE/PALO comparative case could be a useful community contribution after the experiment is completed.

Potential contribution:

**A synthetic case demonstrating the complementary roles of mission governance and AI lifecycle governance.**

Such a contribution should:

- Use synthetic information.
- Clearly identify RACE and PALO responsibilities.
- Avoid claiming that either system certifies the other.
- Preserve source links and version information.
- Disclose all limitations.
- Avoid presenting proposed CNS interoperability as implemented.

PALO's public repository is MIT-licensed. Any copied or adapted code must comply with its license, including preservation of required notices.

Initial engagement should be technical and evidence-based, not a premature partnership announcement.

# 9. Risks and Design Guardrails

## 9.1 Scope expansion

**Risk:** RACE becomes a second general-purpose AI governance platform.

**Guardrail:** Keep RACE focused on mission definition, investigation, prompt construction, authorization boundaries, and mission evaluation.

## 9.2 Governance duplication

**Risk:** RACE duplicates PALO's risk, control, and lifecycle registries.

**Guardrail:** Prefer references and structured exchange over duplicating entire governance frameworks.

## 9.3 CNS authority creep

**Risk:** CNS becomes responsible for policy or business decisions.

**Guardrail:** CNS remains a shared contract, identity, integrity, and interoperability layer.

## 9.4 Simulated independence

**Risk:** The permanent RACE panel is mistaken for three independently executing agents.

**Guardrail:** Record actual execution identity and review provenance. Disclose when multiple perspectives are simulated within one execution.

## 9.5 Integrity confused with truth

**Risk:** A signed or digest-bound artifact is treated as proof that its contents are accurate.

**Guardrail:** Distinguish integrity, provenance, factual truth, authorization, execution, and outcome verification.

## 9.6 Preview confused with production

**Risk:** PALO-AI Developer Preview capabilities are treated as production security controls.

**Guardrail:** Respect the published maturity limits. Use isolated evaluation and non-consequential actions only until the required production controls are independently demonstrated.

## 9.7 Prompt quality confused with mission success

**Risk:** A well-structured prompt is treated as proof of a successful AI outcome.

**Guardrail:** Evaluate actual results against the original human objective and acceptance criteria.

# 10. Recommended Work Sequence

| Sequence | Work | Proposed disposition |
|---|---|---|
| 1 | Preserve RACE as an independent mission-governance framework | KEEP |
| 2 | Benchmark RACE against PALO using one synthetic mission | KEEP |
| 3 | Produce a capability and evidence crosswalk | ADAPT |
| 4 | Inspect PALO schemas and CNS contracts in detail | INVESTIGATE |
| 5 | Draft a RACE Mission Interoperability Contract | DESIGN |
| 6 | Test a local, non-production exchange prototype | DEFER until design approval |
| 7 | Prepare a synthetic PALO Casebook contribution | DEFER until experiment |
| 8 | Explore maintainer engagement | KEEP OPEN |
| 9 | Import PALO runtime code into RACE | NO ACTION absent a demonstrated need |

# 11. Proposed Next Architecture Deliverable

The next design deliverable should be:

## RACE Mission Interoperability Contract

A versioned, digest-bound mission package that can be:

- Created by RACE.
- Reviewed by another governance system.
- Enriched with applicable governance context.
- Bound to identity and provenance.
- Presented for human authorization.
- Handed to an independent AI execution environment.
- Returned with execution evidence.
- Evaluated against the original mission.
- Preserved for later review.

The receiving system must retain its own policy, permissions, and execution authority.

The contract should define:

- Required fields.
- Optional fields.
- Version compatibility.
- Identity and digest semantics.
- Evidence references.
- Authorization references.
- Decision semantics.
- Expiration and revocation behavior.
- Error and retry behavior.
- Selective disclosure.
- Provenance requirements.
- Closure and outcome records.

No contract should be implemented until its ownership, security boundaries, and compatibility requirements have been reviewed.

# 12. Final Architectural Position

RACE should remain independent.

PALO should remain independent.

CNS should connect systems without absorbing their responsibilities.

The potential relationship is:

**RACE governs the assignment. PALO governs the broader AI use case and lifecycle. CNS makes structured information and decisions portable and checkable. STACK can provide supporting evidence and provenance capabilities.**

This is a credible architectural hypothesis and a worthwhile subject for controlled investigation.

It is not yet a demonstrated product integration, an independently validated architecture, or proof of global novelty.

The immediate objective is to establish the practical value of RACE through comparative testing, then design interoperability around demonstrated needs.

---

# 13. Evidence and Source Register

Research snapshot date: 2026-11-03.

The following public sources informed this document. Version and maturity claims should be rechecked before future implementation or publication.

## PALO primary sources

1. PALO Framework public website and current release overview:
   https://paloframework.org/

2. PALO Governance Lifecycle Guide:
   https://paloframework.org/PALO_Guide.html

3. PALO v3.1 Governance Control Plane:
   https://paloframework.org/docs/palo-v3.1-governance-control-plane.html

4. PALO v3.1 Semantic Foundation:
   https://paloframework.org/docs/palo-v3-semantic-foundation.html

5. PALO-AI Governance Integration Guide:
   https://paloframework.org/docs/palo-ai-governance-integration-guide.html

6. PALO-AI Adoption Paths:
   https://paloframework.org/docs/palo-ai-adoption-paths.html

7. PALO-AI Developer Preview:
   https://paloframework.org/examples/agentic-interface/README.html

8. PALO Platform Map:
   https://paloframework.org/PALO_PlatformMap.html

9. PALO worked governance evidence example:
   https://paloframework.org/docs/ai-governance-evidence-worked-example.html

10. PALO public GitHub repository:
    https://github.com/sev7enITA/PALOframework

11. PALO MIT License:
    https://github.com/sev7enITA/PALOframework/blob/main/LICENSE

12. PALO contribution guidance:
    https://github.com/sev7enITA/PALOframework

## RACE primary sources

1. RACE repository:
   https://github.com/wking53214/RACE

2. RACE Core:
   https://github.com/wking53214/RACE/blob/main/RACE_CORE.md

3. RACE Architecture:
   https://github.com/wking53214/RACE/blob/main/ARCHITECTURE.md

4. RACE README:
   https://github.com/wking53214/RACE/blob/main/README.md

## CNS primary sources for future investigation

1. CNS repository:
   https://github.com/wking53214/CNS

2. CNS gate implementation:
   https://github.com/wking53214/CNS/blob/main/cns/gate.py

3. CNS Decision Guard:
   https://github.com/wking53214/CNS/blob/main/cns_composition/decision_guard.py

4. CNS UAI-1 interoperability specification:
   https://github.com/wking53214/CNS/blob/main/docs/interop/UAI-1.md

5. CNS provider protocol:
   https://github.com/wking53214/CNS/blob/main/cns_composition/providers/protocol.py

## Evidence classification

**INSPECTED:** Public RACE documentation, public PALO documentation and repository license were examined for this research.

**INFERRED:** The proposed separation of mission governance, lifecycle governance, and interoperability responsibilities.

**PROPOSED:** RACE/PALO capability mapping, CNS exchange contract, comparative experiment, and community contribution.

**UNKNOWN:** Whether the proposed integration produces measurable improvements, whether the systems can exchange all required information without semantic loss, and whether the architecture has commercial demand.

**NOT EXECUTED:** No RACE/PALO comparative experiment, CNS integration, interoperability test, production deployment, or independent validation has been performed as a result of this document.

---

**End of document**
