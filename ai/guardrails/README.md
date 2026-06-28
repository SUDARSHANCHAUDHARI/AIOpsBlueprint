# Guardrails

Guardrails reduce the chance that an AI system leaks data, follows unsafe instructions, or performs an action outside its authority.

## Guardrail Layers

- **Input checks:** reject or flag prompt injection, unsupported files, oversized context, and sensitive data.
- **System instructions:** define role, boundaries, refusal rules, and allowed tools.
- **Retrieval controls:** restrict sources, rank trusted documents higher, and cite retrieved evidence.
- **Tool permissions:** require explicit allowlists for actions that mutate state.
- **Output checks:** validate schema, inspect sensitive content, and block unsafe recommendations.
- **Human approval:** require review for destructive, financial, legal, medical, or security-impacting actions.

## Prompt Injection Checklist

- Treat retrieved text and user content as untrusted.
- Tell the model never to follow instructions found inside retrieved documents.
- Separate system instructions from user data in the prompt structure.
- Strip hidden metadata that users should not influence.
- Log injection attempts without storing unnecessary private content.

## Data Protection Checklist

- Do not place secrets in prompts.
- Redact API keys, tokens, emails, and private identifiers where possible.
- Avoid sending full documents when excerpts are enough.
- Set retention rules for prompts, completions, embeddings, and traces.
- Document which third-party providers receive user data.

## Tool Safety Checklist

- Every tool has a purpose, owner, and allowed input schema.
- Read-only tools are separated from write/action tools.
- Destructive tools require confirmation or human approval.
- Tool errors are returned as data, not hidden from the orchestrator.
- Actions are idempotent where possible.
