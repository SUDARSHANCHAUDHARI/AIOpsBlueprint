# Evaluation

Evaluation proves an AI system is good enough for its intended job before it reaches users.

## Minimum Evaluation Plan

Define these before launch:

- **Task:** what the model or agent is supposed to do.
- **Inputs:** prompt, context, files, tool results, retrieved documents, or user messages.
- **Expected output:** format, tone, constraints, and required fields.
- **Failure modes:** hallucination, unsafe action, leakage, wrong tool use, bad refusal, latency, cost.
- **Golden set:** 20-50 representative examples for the first MVP.
- **Review owner:** who decides if a regression blocks release.

## Core Metrics

- **Pass rate:** percentage of examples that meet the expected outcome.
- **Critical failure count:** failures that leak data, take unsafe action, or mislead the user.
- **Grounding score:** whether claims are supported by source context.
- **Format validity:** JSON/schema/markdown/output contract correctness.
- **Latency and cost:** p95 response time and average cost per successful task.

## Release Gate

Do not launch unless:

- all critical examples pass
- output schema validation passes
- known limitations are documented
- rollback is possible without code changes
- logs are sufficient for debugging

## Regression Loop

1. Add every production failure as a new eval case.
2. Re-run the golden set before prompt, model, retrieval, or tool changes.
3. Compare current results against the previous accepted baseline.
4. Block release on new critical failures.
5. Record the decision and owner in the release notes.
