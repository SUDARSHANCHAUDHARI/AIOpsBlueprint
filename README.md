# AIOps Blueprint

The open-source blueprint for building, operating, and governing AI-powered engineering systems.

## Table of Contents

- [MVP](#mvp)
- [How To Use This Repo](#how-to-use-this-repo)
- [Operating Principles](#operating-principles)
- [MVP Status](#mvp-status)
- [About](#about)

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

---

## About

I'm Sudarshan Chaudhari, a Senior Quality Engineer, Test Automation specialist, and AI systems builder based in Bangkok, Thailand.

I have 13+ years of experience in software quality engineering, working across SaaS, fintech, gaming, web, mobile, cloud, and digital signage platforms. My background combines hands-on test automation with QA leadership, test strategy, CI/CD, release quality, production investigation, and cross-platform validation.

Alongside my professional QA career, I run [SudarshanTechLabs](https://sudarshantechlabs.com/), my independent engineering and product lab where I design, build, test, and ship software across Android, web, AI, cybersecurity, developer tooling, and cross-platform applications.

### What I work on

- ⚙️ **Quality Engineering & Test Automation** — Playwright, Selenium, Cypress, Appium, API testing, automation frameworks, end-to-end testing, CI/CD, release gates, GitHub Actions, risk-based testing, and production validation
- 🤖 **AI Systems & Automation** — AI agents, multi-agent orchestration, MCP servers, AI-assisted QA, prompt tooling, developer workflows, automation systems, and Claude Code plugins
- 📱 **Mobile & Cross-Platform Applications** — Android applications built with Kotlin and Jetpack Compose, Google Play releases, automated build and publishing pipelines, and cross-platform development spanning iOS, web, Windows, and macOS
- 🌐 **Web Applications & Platforms** — Full-stack applications using Next.js, TypeScript, Firebase, Cloudflare, REST APIs, and modern web infrastructure
- 🛠️ **Developer Tooling & CLI Engineering** — Rust, Python, TypeScript, CLI utilities, multi-repository tooling, build automation, release tooling, and engineering productivity systems
- 🛡️ **Cybersecurity & Observability** — Threat detection, log analysis, security auditing, vulnerability assessment, monitoring, and security-focused developer tools
- 📺 **Digital Signage & Device Platforms** — Content validation, playback testing, device compatibility, production investigation, monitoring, and QA across diverse hardware and operating-system environments

My work sits at the intersection of quality engineering, automation, AI, and software development. I approach products with a QA mindset from the beginning: understanding failure modes, designing for testability, automating repetitive work, and building release confidence into the engineering process.

Through SudarshanTechLabs, I also build products and tools from idea to production, covering architecture, development, testing, CI/CD, release automation, monitoring, and ongoing maintenance.

🌐 [sudarshantechlabs.com](https://sudarshantechlabs.com/) · 💼 [LinkedIn](https://linkedin.com/in/sudarshan-chaudhari) · 🐙 [GitHub](https://github.com/SUDARSHANCHAUDHARI) · ✉️ [sunny.sudarshan@gmail.com](mailto:sunny.sudarshan@gmail.com)
