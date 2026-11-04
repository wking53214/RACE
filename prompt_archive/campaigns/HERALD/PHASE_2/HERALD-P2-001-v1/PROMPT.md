RACE — HERALD

PHASE 2: APPROVED IMPLEMENTATION, DOWNSTREAM INTEGRATION & ADVERSARIAL CLOSURE

1. MISSION

Implement the approved HERALD architecture produced by Phase 1.

This is the first phase authorized to modify production code.

The mission is to implement the selected solutions correctly, eliminate or replace components where authorized, coordinate necessary downstream modifications, validate the resulting architecture, and establish whether the implemented system meets its acceptance criteria.

This is not permission to improvise a new architecture without approval.

Phase 2 must execute the approved Phase 1 blueprint while preserving the authority to identify newly discovered problems and request a revised decision when the approved design proves inadequate.

The objective is not merely to make tests pass.

The objective is to make HERALD correct, secure, interoperable, maintainable, and dependable within its actual STACK relationships.

---

2. MANDATORY PHASE 1 INPUT AND APPROVAL GATE

Phase 2 is INOPERABLE until the actual Phase 1 output is supplied and explicit human approval is established.

Do not begin implementation using:

- A summary of Phase 1.
- Memory of Phase 1.
- The Phase 1 prompt without its results.
- An incomplete implementation plan.
- An unapproved recommendation.
- Assumptions about which downstream changes are acceptable.

Required Phase 1 artifacts

Require:

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

Validate the package

Before making any change:

- Verify every required artifact is present.
- Read the complete blueprint.
- Validate recommendation and implementation-unit IDs.
- Validate repository and dependency references.
- Check that the target architecture agrees with the migration plan.
- Check that acceptance criteria are explicit.
- Identify all destructive and replacement actions.
- Identify all affected repositories.
- Identify deferred decisions and unresolved prerequisites.
- Verify the Phase 1 manifest is complete.
- Verify the referenced Phase 0 baseline and package.

If the package is incomplete, inconsistent, or not ready for implementation, return:

"PHASE 2 BLOCKED — IMPLEMENTATION BLUEPRINT INSUFFICIENT"

List the specific blockers.

Do not invent missing implementation decisions.

Explicit human approval

The human owner must explicitly approve:

- The Phase 1 blueprint/version or exact manifest.
- The implementation units authorized.
- The affected repositories.
- The replacement and elimination actions.
- Any breaking contract or migration decisions.

Do not interpret delivery of the Phase 1 report, this prompt, or prior permission to consider architectural elimination as automatic approval of every implementation recommendation.

A valid authorization must clearly identify the approved blueprint and scope.

If approval is absent, ambiguous, or narrower than the implementation being proposed, stop before modifications and request the missing authorization.

Once an implementation unit and its specified replacement or elimination actions have been approved, do not request redundant approval for every individual file within that approved unit.

Do not expand beyond the approved scope.

---

3. PERMANENT RACE EXPERT PANEL

The same three permanent seats participate throughout implementation.

No additional expert seats may be added.

UCO — Universal Chief Officer

Owns the strategic and architectural challenge.

Must verify:

- Each implementation unit serves HERALD's approved purpose.
- The target architecture is preserved.
- Responsibilities remain correctly assigned.
- Downstream requirements are not ignored.
- Local fixes do not compromise the overall system.

Hacker — Adversarial Security Expert

Owns the adversarial implementation challenge.

Must verify:

- Proposed defenses actually close identified attack paths.
- Security does not depend on unverified assumptions.
- Trust boundaries remain explicit.
- New attack surfaces are identified.
- Downstream consumers cannot silently accept invalid or forged information.

MacG — Systems Engineering Expert

Owns the practical engineering challenge.

Must verify:

- Implementation follows the simplest approved effective design.
- Existing capabilities are reused appropriately.
- Unnecessary abstractions are not introduced.
- Changes remain maintainable.
- The implementation does not grow beyond its approved purpose.

All three seats must participate in major implementation decisions and adversarial closure reviews.

Record material disagreement and its resolution.

Do not claim independent AI agents were executed unless they actually were.

---

4. ARCHITECTURAL REPLACEMENT AND ELIMINATION AUTHORITY

The human owner has expressly authorized complete replacement or elimination of existing HERALD aspects where they do not directly support HERALD's overarching intent and required functionality, and where a better approach can be instituted.

This authority must be applied in accordance with the approved Phase 1 blueprint.

The implementation team must not preserve components simply because they already exist.

Approved actions may include:

- Replacing entire modules.
- Rebuilding a capability using a different approach.
- Removing redundant abstractions.
- Consolidating overlapping responsibilities.
- Separating improperly coupled components.
- Removing obsolete interfaces.
- Eliminating unused or mission-inconsistent functionality.
- Replacing dependencies.
- Changing internal data models.
- Removing old code paths made obsolete by the approved design.

Requirements for complete removal

Before eliminating a component, confirm:

1. The target is explicitly identified in the approved Phase 1 blueprint.
2. The affected files and interfaces are understood.
3. The component's actual functionality has been inventoried.
4. Required functionality is retained or intentionally retired.
5. Downstream dependencies have been addressed.
6. Migration and compatibility requirements have been satisfied.
7. Replacement acceptance criteria are met.
8. Relevant regression and adversarial tests pass.

Do not retain a weak component just to avoid a substantial rewrite.

Do not remove a component simply because its replacement looks cleaner.

If the approved replacement proves inadequate, stop the affected implementation unit, document the evidence, and request a revised decision.

The elimination authority does not authorize removal of unrelated repository functionality or unapproved downstream components.

---

5. REPOSITORY AND WORKSPACE SAFETY BASELINE

Before changing anything, inspect the current state of every repository in the approved scope.

Record:

- Repository identity.
- Current branch.
- Exact HEAD.
- Working-tree status.
- Untracked files.
- Existing modifications.
- Relevant tags and versions.
- Dependency state.
- Test baseline.
- Available CI status.

Never overwrite existing user work.

If a working tree contains unrecognized or unrelated modifications, stop and identify them before proceeding.

Do not assume the current checkout matches Phase 0 or Phase 1.

Baseline drift

Compare current state with:

- Phase 0 repository snapshots.
- Phase 1 research assumptions.
- The approved target architecture.

Record changes in:

- Source.
- Interfaces.
- Dependencies.
- Downstream repositories.
- Contracts.
- Branches.
- Versions.
- Tests.

If drift materially invalidates the approved solution, stop the affected implementation unit and request a decision.

Branch and Git safety

Do not silently:

- Switch branches.
- Create branches.
- Rebase.
- Reset.
- Clean untracked files.
- Delete branches.
- Merge branches.

Work only in an explicitly designated and safe implementation workspace.

If no suitable workspace or branch is designated, identify the requirement before making changes.

Do not commit, push, merge, tag, publish, or release unless the human owner separately authorizes those actions.

---

6. IMPLEMENTATION SEQUENCE

Follow the approved Phase 1 implementation sequence.

Do not reorder work simply because another change appears easier.

For each implementation unit:

Step A — Confirm prerequisites

- Confirm its authorization.
- Confirm the required repositories are available.
- Confirm dependent changes are understood.
- Confirm the working tree is safe.
- Confirm required interfaces and versions.

Step B — Establish the baseline

- Run the relevant existing tests where possible.
- Record failures before modification.
- Identify unrelated pre-existing failures.
- Record the exact commands and results.

Do not attribute existing failures to the new changes.

Step C — Implement one logical intervention

Make only the modifications necessary for the approved implementation unit.

Avoid mixing unrelated cleanup into the change.

If a better design is discovered, document it rather than silently changing the approved target.

Step D — Validate the intervention

Execute the unit's acceptance criteria.

Run:

- Relevant unit tests.
- Regression tests.
- Contract tests.
- Integration tests.
- Security tests.
- Static analysis and type checks where applicable.
- Downstream consumer tests.

Step E — Adversarial retest

Hacker must challenge the actual implementation.

Verify:

- The original attack path is closed.
- The fix cannot be bypassed through another entry point.
- New weaknesses were not introduced.
- Downstream verification remains sound.

Step F — Record closure

For each intervention record:

- Files changed.
- Reason for each change.
- Tests executed.
- Results.
- Failures.
- Regression observations.
- Downstream verification.
- Remaining risks.
- Approval and disposition.

Use one logical intervention per retest wherever practical.

Do not bundle unrelated fixes into one untraceable modification.

---

7. IMPLEMENTATION RESPONSIBILITIES

Implement all authorized Phase 1 changes, including those that require coordinated downstream work.

The following areas must be addressed whenever they are included in the approved blueprint.

A. HERALD core

Implement approved changes to:

- Source extraction.
- Evidence representation.
- Claim construction.
- Claim validation.
- Confidence assessment.
- Human confirmation.
- Provenance.
- Export and verification.
- Persistence interfaces.
- Calibration and evaluation.

Preserve the approved responsibility boundaries.

B. Security and trust

Implement the approved trust model, including relevant changes to:

- Claim identity binding.
- Validation at trust boundaries.
- Provenance integrity.
- Confirmation integrity.
- Human identity boundaries.
- Extractor validation.
- Numeric validation.
- Concurrency protection.
- Replay resistance.
- Cryptographic signing.
- Cross-process verification.
- Key-management interfaces.

Do not claim authenticated human identity when the implementation only records an asserted identity.

Do not claim cross-process trust when verification still depends on an unshared process-local secret.

C. CNS integration

Implement the approved CNS integration design.

Preserve the intended separation:

- CNS provides the thin contract and binding layer.
- HERALD owns its designated evidence and claim functionality.
- CNS does not become HERALD's policy or authorization engine.

Verify:

- ALPHA source-side behavior.
- OMEGA claim-side behavior.
- Source-to-claim lineage.
- Gate status semantics.
- Failure propagation.
- Contract compatibility.
- Binding and digest behavior.
- Cross-process requirements where approved.

Do not conflate native component digests with CNS binding digests.

Do not change CNS unless the approved blueprint explicitly requires it.

D. Downstream integrations

Implement necessary downstream modifications in the repositories explicitly authorized by the human owner.

Potentially relevant systems include:

- TIE.
- CCC.
- Conservation_Kernel.
- Governance_Gateway.
- CCCb.
- Other repositories established in the Phase 0 and Phase 1 dependency maps.

Do not presume every listed repository requires a change.

For each actual downstream dependency:

- Update the relevant contract or adapter.
- Preserve verification requirements.
- Update affected tests.
- Address version compatibility.
- Validate both producer and consumer behavior.
- Record coordinated release requirements.

If a required repository is unavailable or not authorized, do not silently substitute assumptions. Mark the integration incomplete and identify the precise blocker.

E. Documentation and repository hygiene

Implement approved documentation and hygiene changes.

Inspect and reconcile:

- README.
- Constitution.
- Architecture documentation.
- Architecture ghost inventory.
- Research notes.
- Changelog.
- Dependency comments and pins.
- CI workflows.
- Test claims.
- Installation and compatibility instructions.
- Release documentation.

Documentation must describe actual implemented behavior.

Historical test counts and CI claims must be dated and clearly distinguished from current results.

Do not create a release merely because the documentation has been updated.

Do not delete branches or publish releases without separate authorization.

---

8. DOWNSTREAM COMPATIBILITY AND MIGRATION

No HERALD implementation unit is complete merely because HERALD's own tests pass.

For every affected downstream consumer, validate:

- Expected input.
- Produced output.
- Contract compatibility.
- Version compatibility.
- Provenance semantics.
- Signature and digest verification.
- Error behavior.
- Failure propagation.
- Migration and rollback.
- Historical data behavior where relevant.

Compatibility scenarios

Test the relevant deployment conditions:

1. New HERALD with an older consumer.
2. Older HERALD with a new consumer.
3. Mixed contract versions.
4. Missing or unavailable verification keys.
5. Invalid or unknown schema fields.
6. Verification failure.
7. Partial migration.
8. Consumer rejection.
9. Historical evidence or claims.
10. Rollback following a failed migration.

Where the approved design requires a breaking change:

- Implement the new contract.
- Update all authorized consumers.
- Document the transition.
- Preserve historical verification as specified.
- Record any external coordination still required.

Never report a downstream integration as complete when only the HERALD producer has been changed.

---

9. TESTING AND ADVERSARIAL CLOSURE

Execute the Phase 1 acceptance and test plan.

At minimum, cover applicable cases involving:

- Claim substitution.
- Claim mutation.
- Confirmation binding.
- Forged human provenance.
- Unknown extractors.
- Invalid thresholds.
- NaN and infinity.
- Concurrency.
- Replay.
- Cross-process signature verification.
- Key rotation and revocation.
- Tampered exports.
- Source verification.
- CNS ALPHA/OMEGA behavior.
- TIE consumption and verification.
- Schema evolution.
- Downstream compatibility.
- Migration.
- Failure propagation.
- Adversarial extraction.
- Regression of existing functionality.

Test reporting rules

For every test result record:

- Exact test or command.
- Repository and commit.
- Whether it was actually executed.
- Pass/fail/skip status.
- Relevant output.
- Known limitations.

Distinguish:

- Tests executed and passed.
- Tests executed and failed.
- Tests skipped.
- Tests not run.
- Tests that could not be run.

Do not conceal failures through skip markers, weakened assertions, broad exception handling, or altered test expectations.

A test may be changed when its expected behavior is genuinely obsolete under the approved architecture. Document the old expectation, new contract, reason, and replacement coverage.

Do not reduce test coverage merely to achieve a green result.

Security closure

For each previously identified security defect:

- Reproduce the original behavior where practical.
- Implement the approved correction.
- Demonstrate the attack no longer succeeds.
- Test adjacent bypasses.
- Record any remaining limitations.

A passing regression test is evidence of the tested behavior, not proof of complete security.

---

10. CHANGE MANAGEMENT AND SCOPE CONTROL

Every modification must trace back to:

- A Phase 0 finding or newly validated discovery.
- A Phase 1 solution decision.
- An approved implementation unit.

Maintain a live change register.

Required fields:

- Change ID.
- Source finding ID.
- Approved solution ID.
- Repository.
- Files changed.
- Nature of change.
- Downstream impact.
- Test evidence.
- Review status.
- Remaining risks.

Newly discovered issues

If implementation uncovers a problem not covered by Phase 1:

1. Stop the affected implementation unit if the discovery changes its design, trust assumptions, or downstream compatibility.
2. Document the new finding.
3. Identify its dependencies.
4. Recommend the smallest safe response.
5. Request human authorization when it expands scope.

Do not silently introduce new architectural decisions.

Small, necessary implementation details already contained within an approved design do not require repeated approval.

Material architectural or destructive changes outside the approved blueprint do.

---

11. COMPLETION AND ACCEPTANCE

An implementation unit is complete only when:

- Its approved changes are implemented.
- Its acceptance criteria are satisfied.
- Relevant regression tests pass.
- Relevant adversarial tests pass.
- Downstream requirements are verified.
- Documentation is accurate.
- Remaining risks are recorded.

The overall campaign is not complete until all authorized units are either:

- Completed and validated.
- Formally deferred.
- Blocked with a precise explanation.
- Rejected through an approved decision.

Do not label incomplete downstream work as complete.

Do not issue a blanket certification based on a passing unit-test suite.

Final status

Return one of:

- "IMPLEMENTATION COMPLETE — ACCEPTANCE CRITERIA MET"
- "IMPLEMENTATION PARTIALLY COMPLETE — DOCUMENTED REMAINING WORK"
- "IMPLEMENTATION BLOCKED — HUMAN DECISION REQUIRED"
- "IMPLEMENTATION FAILED — ACCEPTANCE CRITERIA NOT MET"

Explain the evidence supporting the status.

---

12. FINAL DELIVERABLES

Produce:

1. Implementation executive summary — What changed and why.
2. Approved-scope reconciliation — What was approved, completed, deferred, or blocked.
3. Change register — Every modified file and its reason.
4. Replacement and elimination report — What was removed, replaced, consolidated, or retained.
5. Downstream integration report — Each affected repository, contract, and validation result.
6. CNS integration report — Actual ALPHA/OMEGA and contract behavior after implementation.
7. Test execution report — Commands, results, failures, skips, and limitations.
8. Security closure report — Original attack paths, mitigations, and residual risks.
9. Compatibility and migration report — Version changes, transition steps, and outstanding consumer work.
10. Documentation and hygiene report — README, notes, pins, workflows, and release readiness.
11. Deferred work register — What remains and why.
12. Final architectural assessment — Whether the implementation meets the approved target.

Create or update an external execution package, outside the repository worktrees, with:

- "PHASE2_EXECUTIVE_SUMMARY.md"
- "PHASE2_CHANGE_REGISTER.csv"
- "PHASE2_DOWNSTREAM_VALIDATION.csv"
- "PHASE2_TEST_EXECUTION_REPORT.md"
- "PHASE2_SECURITY_CLOSURE.md"
- "PHASE2_MIGRATION_AND_COMPATIBILITY.md"
- "PHASE2_DEFERRED_WORK.md"
- "PHASE2_MANIFEST.json"

The manifest must identify:

- Approved Phase 1 blueprint and manifest.
- Human authorization record.
- Actual repository commits before and after work.
- Implemented change IDs.
- Affected repositories.
- Executed tests and results.
- Outstanding failures and limitations.
- Final completion status.

Do not commit or publish these reports unless separately authorized.

---

13. SECONDARY WORKSTREAM — INDEPENDENT RACE PERFORMANCE EVALUATION

Produce a separate, independent RACE evaluation of the Phase 2 implementation experience.

This is another standalone research artifact. It must not rely on the Phase 0 or Phase 1 RACE evaluation reports.

The evaluator must not change implementation scope or priorities.

Evaluate the permanent seats

UCO

- Did strategic oversight prevent architectural drift?
- Did UCO preserve the intended system boundaries?
- Did it identify downstream consequences before they became defects?

Hacker

- Did adversarial review catch real implementation weaknesses?
- Did security challenge materially improve the finished work?
- Did it detect weaknesses that conventional tests missed?

MacG

- Did engineering analysis reduce complexity?
- Did it identify better or smaller implementations?
- Did it improve integration and maintainability?

Evaluate RACE as an implementation framework

Investigate:

- Whether the three seats made implementation more reliable.
- Whether the seats prevented premature modifications.
- Whether dependency-aware sequencing reduced regressions.
- Whether the framework helped control scope.
- Whether it introduced repetition or overhead.
- Whether disagreements improved implementation choices.
- Whether the RACE process consumed disproportionate resources.
- Whether the structure was practical during real code changes.

New capability analysis

Identify capabilities demonstrated through Phase 2 that were not merely theoretical.

Distinguish actual improvements from claims that cannot be proven.

Net value verdict

Use:

- HELP.
- PARTIAL HELP.
- NEUTRAL.
- HINDRANCE.
- INCONCLUSIVE.

Support the result with actual observations, not enthusiasm for the framework.

Independent output

Produce:

"RACE_PHASE2_INDEPENDENT_EVALUATION.md"

Include:

- What worked.
- What failed.
- What was genuinely new.
- Contributions of each seat.
- Redundant analysis.
- Implementation overhead.
- Evidence of better or worse outcomes.
- Final net value verdict.
- Recommendations for RACE's future structure.

This report is independent of the HERALD implementation assessment.

---

14. FINAL RACE PANEL CLOSURE

Before closing the campaign, require all three seats to review the final implementation evidence.

UCO final challenge

Does the implemented system fulfill HERALD's approved purpose?

Have responsibilities been placed correctly?

Are downstream dependencies addressed?

Has the architecture improved without unnecessary complexity?

Hacker final challenge

Which original attack paths were closed?

What new weaknesses exist?

Can evidence, claims, confirmation, and provenance be independently trusted to the extent claimed?

Which trust assumptions remain external?

MacG final challenge

Is the resulting system simpler, more maintainable, and more effective?

Did the implementation preserve unnecessary machinery?

Could any remaining component be replaced or removed without loss of required functionality?

Record disagreements and unresolved risks.

---

15. FINAL AUTHORIZATION BOUNDARY

Phase 2 is the implementation phase, but it remains bound to the approved blueprint.

Implement only explicitly authorized scope.

The owner has granted architectural freedom to replace or eliminate components when they fail to support HERALD's mission or a better solution is approved.

Use that authority decisively within the approved implementation units.

Do not preserve weak components out of habit.

Do not destroy useful functionality without demonstrating that its required purpose is preserved or intentionally retired.

No commits, pushes, merges, branch deletions, tags, package publications, or releases without separate authorization.

At completion, present the implementation evidence, final status, remaining risks, and independent RACE evaluation.

Stop.

Do not begin additional architectural work or publish a release without further human direction.
