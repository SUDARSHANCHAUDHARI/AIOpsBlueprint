# AIOps Blueprint

The open-source blueprint for building, operating, and governing AI-powered engineering systems.

## MVP

AIOps Blueprint is a practical operating manual for teams shipping AI features. It starts with the minimum set of documents a team needs before an AI system reaches real users:

- evaluation plan
- guardrail checklist
- incident response playbook
- production readiness checklist
- reusable runbook template

## How To Use This Repo

1. Start with [Production Readiness](playbooks/production-readiness/README.md) before launch.
2. Define quality gates in [Evaluation](ai/evaluation/README.md).
3. Add safety controls from [Guardrails](ai/guardrails/README.md).
4. Copy the [Runbook Template](templates/runbooks/README.md) for every user-facing AI workflow.
5. Use [Incident Response](playbooks/incident-response/README.md) when a model, prompt, retrieval source, or automation behaves unexpectedly.

## Operating Principles

- Treat prompts, evals, datasets, and agent tools as production assets.
- Prefer small repeatable checks over one-time manual review.
- Log enough context to debug failures without storing sensitive user data.
- Keep humans in the loop for high-impact or irreversible actions.
- Document rollback paths before launch, not during an incident.

## MVP Status

This repo is content-first. Automation, dashboards, CI/CD, and hosted tooling are intentionally out of scope until the blueprint itself is useful.
