<!--
Sync Impact Report
Version change: 0.0.0 -> 1.0.0
Modified principles:
- Template placeholders -> I. Intent Before Implementation
- Template placeholders -> II. Evidence Over Assumption
- Template placeholders -> III. Minimal, Reviewable Scope
- Template placeholders -> IV. Quality Gates Are Non-Negotiable
- Template placeholders -> V. Governance and Change Control
Added sections:
- Project Constraints
- Development Workflow
Removed sections:
- None
Follow-up TODOs:
- None
-->

# Spec-Driven Development Template Constitution

## Core Principles

### I. Intent Before Implementation
This repository MUST be driven by explicit requirements and approved spec artifacts before code changes begin. Features MUST start with a clear problem statement, acceptance criteria, and constraints; undocumented assumptions are not valid inputs for implementation. Rationale: design drift and informal decisions are the primary sources of rework, ambiguity, and inconsistent delivery.

### II. Evidence Over Assumption
Every change MUST be supported by verifiable evidence, including tests, checks, or observed behavior. Claims about correctness, reliability, security, or performance MUST cite the relevant evidence or validation result. Rationale: unverified work creates silent failures and weakens trust in the repository.

### III. Minimal, Reviewable Scope
The project MUST prefer the smallest change that satisfies the stated intent and leaves the codebase easier to understand. Large, mixed-purpose edits are prohibited unless the rationale is explicitly documented and reviewed. Rationale: small, focused diffs reduce risk, improve maintainability, and make review quality measurable.

### IV. Quality Gates Are Non-Negotiable
All changes MUST pass the relevant validation gates before merge or release, including syntax checks, targeted tests, and any required contract or integration validation. Failures MUST be resolved before proceeding. Rationale: quality assurance is a delivery requirement, not an optional checkpoint.

### V. Governance and Change Control
This project MUST record intentional policy updates and preserve accessible historical context for future contributors. Any amendment to these principles or workflows MUST include a version bump, rationale, and a review of operational impact. Rationale: governance prevents local preferences from hardening into undocumented exceptions.

## Project Constraints
- The repository MUST remain a usable template for Spec Kit-driven development workflows.
- Documentation, prompts, and process guidance MUST match the repository’s current behavior; stale instructions are treated as defects.
- Non-trivial work MUST be traceable to an approved spec, plan, or issue context before implementation proceeds.
- Security-sensitive inputs, dependency changes, and externally integrated behaviors MUST be reviewed before they are accepted.

## Development Workflow
- The default delivery sequence is specify -> plan -> tasks -> implement -> validate.
- Every task MUST define its acceptance criteria and the validation evidence required to confirm completion.
- Reviewers MUST verify alignment with this constitution before approving significant changes.
- Any amendment to this constitution MUST update the version, date, and impact summary in the repository record.

## Governance
This constitution supersedes informal preferences and local exceptions for repository governance. Changes to these rules require a documented amendment, an impact review, and an explicit version increment. Compliance is reviewed during pull requests and whenever the project workflow changes.

- Amendment procedure: update the constitution, record the rationale, assess compatibility with current practice, and review the change before merge.
- Versioning policy: MAJOR for incompatible governance or principle changes, MINOR for new or materially expanded principles, and PATCH for wording, clarification, or non-semantic refinement.
- Compliance review expectations: contributors and reviewers MUST verify that work aligns with the active principles and required quality gates before approval.

**Version**: 1.0.0 | **Ratified**: 2026-09-15 | **Last Amended**: 2026-09-15
