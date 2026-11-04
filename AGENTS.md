# Instructions for AI maintainers — Founder Skill fork

Project: VahramSargsyan/founder-skill. This is an adaptation fork of Jake Schincariol's MIT-licensed founder-skill. Original Claude skills and Python code remain upstream-compatible.

Governance: follow the accepted Vahram APP universal standard v1.1.0 at `VahramSargsyan/vbos-app/docs/governance/VAHRAM_APP_UNIVERSAL_GOVERNANCE_v1.1.0.md`, subject to this repository's stricter rules. Read this file and `PROJECT_GOVERNANCE.md` before a change.

- Select an explicit mode (AUDIT_ONLY, DIAGNOSTIC_ONLY, IMPLEMENT_FEATURE, BUILD_NEW_APP, ECOSYSTEM_PLANNING, etc.).
- Never claim live buyer validation from AI-generated buyer personas.
- Separate real market sources, owner-supplied data, assumptions, simulated responses and missing data.
- Do not invent costs, client counts, subscription revenue, review quotes or conversion rates.
- Keep the original `skills/`, `tests/`, LICENSE and upstream metadata untouched unless a separate approved and tested change requires it.
- Do not put private business records, customer information, credentials, proprietary source code or financial exports in this **public** fork.
- Do not trigger paid API, Codex, independent agents or external services without explicit current permission.
- ChatGPT adapter instructions are prompt-level guidance, not a claim of automatic skill installation or agent orchestration.
- No changes to VBOS or any other product repository are authorized by this fork.
- Use a feature branch and PR; no automatic merge or production deployment. Report exact checks, NOT_RUN and remaining limitations.
