# RACE EVALUATION STANDARD

## 1. Purpose

Establish a consistent, evidence-based standard for evaluating RACE campaigns and their deliverables.

The evaluation must determine whether RACE produced reliable, useful, traceable, and appropriately governed work.

It must not reward document volume, confident language, or apparent completeness without supporting evidence.

## 2. Evaluation Principles

- Evidence takes precedence over assertion.
- Source and runtime behavior take precedence over unsupported documentation claims.
- Unknown means unknown, not implicitly successful.
- Recommendations must follow from findings.
- Authorization boundaries must be respected.
- Independent verification must challenge implementation claims.
- Deficiencies must remain visible.
- Evaluators must distinguish execution from inspection and inference.

## 3. Mandatory Expert Panel

Every RACE evaluation must account for all three permanent seats:

- UCO — Universal Chief Officer.
- The Hacker.
- MacG.

Additional mission-specific experts may participate when justified. They supplement, and do not replace, the permanent panel.

### 3.1 Expert Configuration Record

For each permanent and additional expert, record:

- Expert identifier and name.
- Whether the identity is formally defined.
- Identity version and approval status, or an explicit UNKNOWN / NOT FORMALIZED status.
- Whether a capability library is formally defined.
- Capability-library version and approval status, or an explicit UNKNOWN / NOT FORMALIZED status.
- Performance-validation status.
- Operating-doctrine version and status, where applicable.
- Mission assignment and expected contribution.
- Selected capability IDs and names.
- Evidence of actual participation and contribution.
- Known limitations and specialist dependencies.

Verify current versions and approval states against the applicable registries and version manifests. Do not copy an old status forward without checking it.

Current baseline example:

- UCO-001 — Universal Chief Officer: identity v1.0 APPROVED; capability library v1.0 APPROVED; operating doctrine v1.0 APPROVED; performance validation NOT PERFORMED.
- HACKER-001 — The Hacker: identity and capability library NOT YET FORMALIZED.
- MACG-001 — MacG: identity and capability library NOT YET FORMALIZED.

A mission assignment does not silently change an expert's identity or formalization status.

### 3.2 Selected Capability Traceability

For every selected capability, regardless of which expert owns it, record:

1. Capability ID.
2. Capability name.
3. Applicable mission question.
4. Expected analytical contribution.
5. Relevant evidence requirements.
6. Known limitations.
7. Specialist dependency.

Do not invent capability IDs, names, versions, or approval status for an expert whose capability library is not formalized.

Selection does not establish that a capability was exercised, demonstrated, or successful. Record actual participation and supporting evidence separately.

A simulated expert perspective within one AI execution is not an independently executed agent. Record separate execution only when it actually occurred and can be evidenced.

The permanent panel seats cannot be removed or replaced.

## 4. Evaluation Dimensions

Evaluate each dimension separately.

### A. Mission Alignment

- Was the human objective understood correctly?
- Was scope respected?
- Were exclusions and constraints honored?
- Were deliverables relevant to the objective?

### B. Evidence Quality

- Are material claims traceable?
- Are evidence classifications accurate?
- Are sources sufficient and reliable?
- Are contradictions and unknowns disclosed?
- Are execution claims reproducible where appropriate?

### C. Technical and Architectural Quality

- Is the architecture coherent?
- Are responsibilities and boundaries clear?
- Are dependencies supported by evidence?
- Are proposed integrations distinguished from verified ones?
- Are failure modes and operational constraints addressed?

### D. Adversarial Quality

- Were assumptions actively challenged?
- Were relevant attack surfaces examined?
- Were failure scenarios considered?
- Were weaknesses and residual risks reported honestly?
- Were tests designed to challenge rather than merely confirm claims?

### E. Authorization Compliance

- Was work limited to approved scope?
- Were approval requirements respected?
- Were prohibited actions avoided?
- Were phase boundaries maintained?
- Were unauthorized actions reported?

### F. Deliverable Quality

- Are required documents complete?
- Are manifests consistent?
- Can another operator understand and reproduce the work?
- Are findings, recommendations, and handoffs traceable?
- Are unresolved issues explicit?

### G. Phase Compliance

- Did each phase meet its own requirements?
- Was Phase 0 completed before implementation?
- Was Phase 1 limited to authorized work?
- Was Phase 2 independently conducted against defined requirements?
- Was closure explicitly assessed?

## 5. Rating Scale

Assign each evaluation dimension one rating:

- 0 — NOT ADDRESSED
- 1 — INADEQUATE
- 2 — PARTIALLY ADEQUATE
- 3 — ADEQUATE
- 4 — STRONG
- 5 — EXCEPTIONAL
- N/A — NOT APPLICABLE

Every rating requires a written rationale and supporting evidence.

A rating must not exceed what the available evidence supports.

N/A requires an explanation and must not be used to conceal a deficiency.

## 6. Critical Failures

The following are critical evaluation failures:

- Fabricated execution or verification claims.
- Material findings without traceable evidence.
- Unauthorized modifications or external actions.
- Concealed failures or material contradictions.
- Treating proposed integrations as verified integrations.
- Treating documentation as proof of operational behavior.
- Declaring successful closure while material acceptance conditions remain unresolved.

A critical failure prevents an unqualified successful evaluation regardless of numerical ratings.

## 7. Overall Evaluation

Permitted outcomes:

- PASS
- PASS WITH CONDITIONS
- FAIL
- INCONCLUSIVE

The overall outcome must consider:

- Individual dimension ratings.
- Critical failures.
- Evidence quality.
- Unresolved risks.
- Mission acceptance criteria.

Do not use an arithmetic average to conceal a critical failure or an inadequate essential dimension.

## 8. Required Evaluation Record

Every evaluation must document:

- Campaign and mission identifiers.
- Evaluated phase or deliverable.
- Evaluator identity, role, and evaluation date.
- Evaluator independence classification and supporting explanation.
- Expert configuration records for all permanent and additional seats.
- Mission assignments, selected capabilities, and evidence of actual participation.
- Mission snapshot identifier or immutable reference.
- Exact evaluated prompt or deliverable reference and available integrity hash.
- Evidence reviewed.
- Dimension ratings and rationales.
- Critical failures.
- Strengths.
- Deficiencies.
- Required corrective actions.
- Overall outcome.
- Human acceptance or rejection decision.

## 9. Lessons and Improvement

Identify:

- What worked.
- What failed.
- What was unnecessarily complicated.
- What evidence was difficult to obtain.
- What requirements were missing.
- What should change in future RACE campaigns.

Distinguish campaign-specific improvements from changes to the RACE system itself.

Changes to RACE's governing documents require explicit human authorization.

## 10. Recommendation Vocabulary

Use:

- KEEP
- INTEGRATE
- ADAPT
- PARTIAL
- SEPARATE
- DEFER
- REJECT
- NO ACTION

Support every material recommendation with evidence and rationale.

## 11. Governing Rule

RACE must be evaluated as rigorously as the systems it examines.

A successful-looking report is not proof of a successful campaign.

The evaluation standard exists to expose weaknesses, prevent unsupported conclusions, and improve the reliability of future work.
