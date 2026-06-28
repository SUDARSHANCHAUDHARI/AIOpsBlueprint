# Runbooks

Copy this template for each AI workflow, agent, or automation.

## Runbook Template

### Name

`<workflow or agent name>`

### Purpose

What user or operational problem does this solve?

### Owner

- Product:
- Engineering:
- Support/Ops:

### Entry Points

- UI:
- API:
- Scheduled job:
- Agent/tool trigger:

### Dependencies

- Model/provider/version:
- Prompt/config:
- Retrieval sources:
- Tools/actions:
- External services:

### Normal Operation

1. User or system provides:
2. AI system does:
3. Tools called:
4. Expected output:
5. Success signal:

### Known Failure Modes

- Prompt injection:
- Hallucinated answer:
- Bad retrieval:
- Tool failure:
- Latency/cost spike:
- Unsafe or unsupported request:

### Detection

- Logs:
- Metrics:
- Alerts:
- User reports:

### Mitigation

- Disable:
- Roll back:
- Change prompt/config:
- Escalate to human:

### Verification

- Eval suite:
- Manual smoke test:
- Expected result:

### Post-Incident Follow-Up

- Add regression eval.
- Update prompt/tool contract.
- Update this runbook.
- Record owner and due date.
