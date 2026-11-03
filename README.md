# RACE
## Red-Team Analysis, Construction & Evaluation

**A governed framework for turning human objectives into disciplined, mission-specific AI execution prompts.**

RACE is designed to make AI-assisted work more rigorous, traceable, adversarially examined, and operationally useful. It provides a repeatable structure for investigating a mission, designing an approach, authorizing controlled work, and independently examining the result.

RACE is built around a simple principle:

> A good prompt is not just a set of instructions. It is a governed assignment with a defined objective, evidence requirements, constraints, expert perspectives, authorization boundaries, deliverables, and acceptance criteria.

RACE is intended to work across different missions and repositories. Its governing requirements remain consistent while mission-specific context, specialist expertise, and technical requirements change.

## What RACE Does

RACE provides a structured process for:

- Translating a human objective into a clearly bounded mission.
- Investigating the existing system and available evidence before proposing changes.
- Identifying technical, operational, security, human, and resource constraints.
- Applying permanent adversarial and problem-solving perspectives.
- Producing a documented architectural or operational blueprint.
- Converting an approved blueprint into controlled implementation instructions.
- Defining evidence-based verification and closure criteria.
- Preserving exact prompts, configurations, decisions, results, and lessons.
- Improving future prompts through traceable evaluation and human approval.

RACE distinguishes prompt generation from prompt execution. Producing a prompt does not authorize its execution, and completing one phase does not automatically authorize the next.

## The Three-Phase Operating Model

### Phase 0 — Discovery, Investigation, and Blueprint

**Question: What is actually required, what is true about the current situation, and what should be done?**

Phase 0 establishes an evidence-supported understanding of the mission before implementation begins.

It includes:

- Defining the objective, scope, constraints, and acceptance conditions.
- Inspecting relevant source material, systems, repositories, and evidence.
- Separating verified facts from inferences and unknowns.
- Mapping dependencies and identifying failure conditions.
- Conducting adversarial analysis.
- Comparing possible approaches and identifying trade-offs.
- Recording unresolved questions, risks, and specialist requirements.
- Producing a recommended blueprint and structured handoff.

**Primary deliverables:** Phase 0 manifest and architectural or operational blueprint.

Phase 0 is investigative. It does not authorize implementation.

### Phase 1 — Controlled Construction

**Question: How should the approved design be carried out without exceeding its authorization?**

Phase 1 translates an accepted Phase 0 blueprint into bounded implementation work.

It includes:

- Confirming the approved scope and requirements.
- Identifying affected components and dependencies.
- Defining the change sequence and implementation boundaries.
- Establishing acceptance criteria and rollback considerations.
- Recording required approvals.
- Executing only work explicitly authorized by the responsible human.

**Primary deliverables:** Phase 1 manifest, implementation instructions, and change record.

Approval of a plan is not blanket authorization for unrelated changes, external actions, commits, pushes, or deployments.

### Phase 2 — Verification, Adversarial Retesting, and Closure

**Question: Did the result actually satisfy the approved requirements, and what evidence supports that conclusion?**

Phase 2 examines the resulting artifacts and evidence against the approved requirements.

It includes:

- Inspecting the resulting implementation.
- Executing authorized tests.
- Conducting adversarial retesting.
- Comparing observed results with acceptance criteria.
- Identifying defects, unresolved risks, and deviations.
- Recording what was independently verified and what was only reviewed.
- Producing a closure recommendation and final disposition.

**Primary deliverables:** Phase 2 manifest, verification record, and final evaluation.

Phase 2 distinguishes independent verification from self-review. A separate prompt, invocation, model, or expert persona does not by itself establish independence.

## The Permanent Expert Panel

Every RACE mission retains three permanent expert seats. Mission-specific specialists may supplement them, but may not replace them.

### UCO — Universal Chief Officer

The executive generalist and operational integrator.

UCO examines whether an undertaking can work under real conditions and remain workable. Its perspective connects objectives, people, resources, dependencies, operational constraints, consequences, and continuity.

UCO is intended to challenge plans that appear technically possible but are operationally unsustainable, inadequately supported, or poorly aligned with the human and organizational realities of the mission.

### The Hacker

The adversarial examiner.

The Hacker examines how a system, plan, assumption, or proposed control can fail, be exploited, bypassed, manipulated, or misused. The role is to expose weaknesses rather than protect the comfort of the proposed design.

### MacG

The unconventional problem-solver.

MacG looks for resourceful, practical, and unconventional ways to solve the mission's problems. This includes identifying simpler approaches, overlooked options, useful substitutions, and ways to accomplish objectives under constraints.

### How the Panel Works

The three perspectives are deliberately different:

- UCO asks whether the undertaking is workable and sustainable.
- The Hacker asks how it can be broken, bypassed, or made to fail.
- MacG asks whether a more resourceful or practical solution exists.

They are required perspectives, not a claim that three independent AI agents are automatically operating. A simulated expert perspective must not be represented as independently executed analysis.

Additional specialists may be included when the mission requires expertise beyond the permanent panel. Their inclusion must have a defined purpose and must not silently change the permanent experts' identities.

## Expert Identity and Capability Governance

RACE separates three components of an expert:

1. **Identity:** Who the expert is and what distinguishes its perspective.
2. **Capabilities:** What the expert is defined to analyze or contribute.
3. **Operating doctrine:** How the expert applies its identity and capabilities.

These components are versioned and governed separately.

The current documented expert baseline is:

| Expert | Identity and capability status |
|---|---|
| UCO-001 — Universal Chief Officer | Identity v1.0, capability library v1.0, and operating doctrine v1.0 approved. Performance validation has not been performed. |
| HACKER-001 — The Hacker | Permanent seat established. Formal identity and capability libraries not yet formalized. |
| MACG-001 — MacG | Permanent seat established. Formal identity and capability libraries not yet formalized. |

Mission assignments do not silently change permanent identities. Selecting a capability for a mission does not establish that it was exercised, demonstrated, or successful.

Permanent changes require documented proposals, evidence, review, and explicit human approval. Mission snapshots preserve the expert configuration used to assemble a prompt.

## Evidence, Traceability, and Evaluation

RACE requires claims to be distinguished by their evidentiary status:

- **EXECUTED:** An action or test was actually performed.
- **INSPECTED:** An artifact, record, or result was examined.
- **INFERRED:** A conclusion was reasoned from available evidence but not directly established.
- **UNKNOWN:** The available evidence does not establish the answer.

RACE is designed to preserve traceability across:

- Human objectives and acceptance criteria.
- Source evidence and findings.
- Expert identities, versions, and mission assignments.
- Selected capabilities and their expected contributions.
- Recommendations and human decisions.
- Authorizations and executed actions.
- Verification evidence and final dispositions.

RACE maintains two distinct evaluation levels:

**Campaign evaluation** examines the quality and conduct of the broader mission across seven campaign dimensions.

**Prompt-execution evaluation** examines the quality and results of an individual generated prompt across ten prompt-specific dimensions.

These assessments are related, but they are not interchangeable. A strong prompt score cannot substitute for campaign-level assessment, and an overall average must not conceal a critical failure.

Evaluation records should identify the evaluator, supporting evidence, limitations, and degree of independence. Human review and acceptance remain controlling.

## Human Authority and Authorization

RACE supports human decision-making. It does not replace the authority of the person or institution responsible for a mission.

The following boundaries apply:

- Recommendations are not authorizations.
- Phase completion does not automatically authorize the next phase.
- Approval of an investigation does not authorize implementation.
- Approval of a prompt does not automatically authorize every action described in it.
- Repository modifications, external actions, financial commitments, commits, pushes, and deployments require explicit authorization.
- An expert's recommendation does not grant real-world authority.

RACE should make authorization boundaries visible in its prompts, records, and handoffs.

## Prompt Archive and Learning

RACE includes a prompt archive and learning structure intended to preserve the exact prompts it generates and the evidence of what happened when they are used.

The archive supports:

- Unique prompt identifiers and version history.
- Exact prompt preservation.
- Records of prompt origin, configuration, and intended use.
- Execution evaluations based on actual results.
- A learning register for reusable findings.
- A prompt evolution log for proposed and approved improvements.

An unexecuted prompt must not be represented as evaluated. A proposed improvement must not be represented as validated. Historical prompt versions and records must not be silently overwritten.

## Repository Map

| Path | Purpose |
|---|---|
| `RACE_CORE.md` | Governing requirements and operating principles. |
| `ARCHITECTURE.md` | System structure and relationships among the phases and components. |
| `CHANGELOG.md` | Project change history and current documentation status. |
| `experts/` | Permanent expert governance, identity and capability records, operating doctrine, and mission snapshots. |
| `templates/` | Phase, evaluation, and repository-profile templates. |
| `schemas/` | Required information and manifest structures for each phase. |
| `protocols/` | Evidence, authorization, dependency, and handoff rules. |
| `campaigns/` | Mission-specific campaign profiles and constraints. |
| `evaluations/` | Campaign-level evaluation standards and templates. |
| `prompt_archive/` | Exact prompt records, prompt evaluations, learning records, and prompt evolution history. |

The documents in these directories serve different purposes. A template describes the intended structure of an artifact; a schema describes required information; a protocol defines a governing procedure. Their presence does not, by itself, demonstrate automated enforcement.

## Getting Started

For a new mission:

1. Read `RACE_CORE.md` and `ARCHITECTURE.md`.
2. Review the applicable authorization, evidence, dependency, and handoff protocols.
3. Identify the mission's objective, scope, constraints, and acceptance criteria.
4. Assemble the permanent expert panel and add justified mission-specific specialists.
5. Use the Phase 0 template to conduct discovery and produce a blueprint.
6. Obtain the required human review and approval before Phase 1.
7. Use the Phase 1 template to define and conduct only authorized construction.
8. Use the Phase 2 template to verify the result and document closure.
9. Archive the exact prompts and their configurations.
10. Evaluate actual execution results and record lessons only when supported by evidence.

For an existing campaign, begin with its campaign profile and preserve the mission's established context and constraints.

## Current Project Status

RACE is in its initial foundation and documentation-development stage.

The repository contains a documented three-phase architecture, permanent expert governance, phase templates and manifest documentation, operating protocols, campaign documentation, and evaluation and prompt-archive structures.

The current documentation work does **not** establish that RACE has:

- An executable prompt-generation engine.
- Automated enforcement of its protocols or authorization rules.
- An automated manifest or schema validator.
- Runtime integration across external repositories or AI systems.
- Three independently operating expert agents.
- Validated performance for the UCO capability library.
- Completed end-to-end campaign validation.

These are implementation and validation questions, not conclusions that can be drawn from the presence of documentation.

The HERALD campaign profile is the initial reference campaign for developing and examining the repeatable process. Its presence does not, by itself, establish successful end-to-end execution.

## Governing Documents

The following documents define the project more fully:

- `RACE_CORE.md` — governing requirements.
- `ARCHITECTURE.md` — architectural relationships and phase responsibilities.
- `experts/README.md` — expert library governance.
- `experts/ASSEMBLY_PROTOCOL.md` — permanent panel assembly requirements.
- `protocols/` — common operating protocols.
- `evaluations/RACE_EVALUATION_STANDARD.md` — campaign evaluation criteria.
- `prompt_archive/README.md` — prompt preservation and learning rules.
- `CHANGELOG.md` — documented project history.

## Governing Principle

**Preserve the objective. Investigate before building. Challenge assumptions. Make authority explicit. Record what actually happened. Verify against evidence. Improve only through traceable and authorized change.**

## License

RACE is licensed under the Apache License, Version 2.0.

See the `LICENSE` file for the complete license terms and the `NOTICE`
file for the project copyright notice.

Copyright 2026 William N. King.
