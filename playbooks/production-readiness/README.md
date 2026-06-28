# Production Readiness

Use this checklist before exposing an AI feature, agent, or automation to real users.

## Product Contract

- The user-facing job is clear.
- Non-goals and unsupported requests are documented.
- The output format is defined and validated.
- Known limitations are visible to support/review teams.

## Model And Prompt

- Model/provider/version are recorded.
- System prompt is versioned.
- Prompt changes are reviewed before release.
- Rollback prompt/model is available.

## Evaluation

- Golden set exists for core workflows.
- Critical safety cases are included.
- Regression results are reviewed by an owner.
- Failures have severity labels and release decisions.

## Retrieval And Data

- Sources are trusted and documented.
- Sensitive fields are redacted or excluded.
- Retrieval freshness is known.
- Citations or evidence are available for user-visible claims.

## Tools And Automation

- Tool list is explicit.
- Write/destructive tools require approval.
- Tool errors are visible and recoverable.
- Rate limits and timeouts are configured.

## Observability

- Prompt/model/tool/retrieval versions are logged.
- Failures can be traced without exposing secrets.
- Cost and latency are monitored.
- There is an owner for alerts.

## Rollback

- Feature flag or kill switch exists.
- Previous prompt/model/config can be restored.
- Incident owner knows the rollback steps.
- Support message is prepared for user-visible impact.
