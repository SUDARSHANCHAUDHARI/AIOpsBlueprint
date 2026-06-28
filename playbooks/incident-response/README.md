# Incident Response

AIOps incidents include unsafe outputs, prompt leaks, tool misuse, bad retrieval, model regressions, runaway cost, and automations taking incorrect action.

## Severity Levels

- **SEV1:** data leak, unsafe action, destructive automation, legal/security exposure.
- **SEV2:** widespread wrong answers, broken workflow, severe latency or cost spike.
- **SEV3:** localized quality regression with workaround.
- **SEV4:** minor issue, documentation gap, or non-user-impacting anomaly.

## First 15 Minutes

1. Assign incident owner.
2. Freeze risky automation or disable the affected feature flag.
3. Preserve logs, prompts, model/version IDs, retrieval IDs, and tool calls.
4. Identify affected users, tenants, repos, or workflows.
5. Decide whether to roll back prompt, model, retrieval index, or tool access.

## Triage Questions

- What changed recently: prompt, model, tools, retrieval data, code, config, provider?
- Is the failure deterministic or intermittent?
- Did the model receive sensitive data or reveal hidden instructions?
- Did any tool mutate external state?
- Can users self-recover, or do we need cleanup?

## Containment Actions

- Disable high-risk tools.
- Switch to a previous prompt/model version.
- Turn off retrieval source or stale index.
- Add temporary refusal/allowlist rule.
- Increase human review for impacted workflows.

## Post-Incident Review

Record:

- timeline
- root cause
- impacted users/data/actions
- detection gap
- rollback or mitigation used
- eval cases added
- owner for permanent fix
