# Project AEGIS — Development Roadmap

**Project phase:** Planning. The milestones below describe intended work, not completed deliverables.

## Phase 0 — Foundation
- Publish mission, licensing, threat model, responsible-use boundaries, and contribution guidance.
- Define a synthetic-data test set and objective evaluation criteria.
- Select a small, maintainable Linux-first stack and document installation.

## Phase 1 — First demonstrable prototype
- Build a local web interface and API.
- Accept only synthetic incident notes in the initial public demonstration.
- Produce structured narrative drafts with explicit source-to-output traceability.
- Provide an officer review/edit workflow and warnings for unsupported claims.
- Test factual preservation and hallucination rates with repeatable cases.

## Phase 2 — Grounded reference assistant
- Index a small set of publicly redistributable legal/training reference documents.
- Return quoted references, precise citations, jurisdiction/date indicators, and uncertainty notices.
- Test citation accuracy and stale-source handling.

## Phase 3 — Scenario-based training
- Generate synthetic scenarios for communication and de-escalation practice.
- Keep training output distinct from live operational guidance.
- Add instructor-controlled review and feedback.

## Phase 4 — Infrastructure evaluation
- Benchmark NVIDIA RTX 4090 / RTX 3090 systems as baselines.
- If available, evaluate DGX Spark large-memory inference and performance-per-watt.
- Publish model, system, and test methodology so results are reproducible.
- Document low-cost deployment configurations.

## Evaluation criteria
- Factual consistency and traceability.
- Citation precision and source freshness.
- Privacy/security review and access control.
- Latency, throughput, memory footprint, and power draw.
- Accessibility and maintainability for small agencies.

No production use should be considered until security, legal, policy, and operational reviews have been completed by the deploying agency.
