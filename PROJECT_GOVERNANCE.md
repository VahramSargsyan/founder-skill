# Founder Skill — local project governance

Profile: `RESEARCH_LOCAL` / prompt-adapter pilot. Mode for initial adaptation: `IMPLEMENT_FEATURE`.

## Goal
Make four original Founder Skill methods usable in ChatGPT for evidence-oriented early-stage business evaluation, preserving upstream behavior and avoiding fabricated certainty.

## In scope
Additive, documented ChatGPT-facing workflows: board, competitor research, pricing hypotheses and CFO input/scenario handling. A generic B2B SaaS low-data pilot template. No new paid infrastructure or agent orchestration.

## Out of scope
Changing original 11 skills, replacing the original Python engines, automatic Claude plugin compatibility, launching 100 buyer agents, uploading business data, modifying VBOS or making a release to a production environment.

## Source and boundaries
- Upstream: https://github.com/Jakeschincariol/founder-skill ; LICENSE MIT, retain attribution.
- Fork source baseline for first block: `fd9385b0cfe1b96bebce3898fbd506d73eff5a9d`.
- `skills/` and original `tests/` remain the canonical reference for what the original pack does.
- `chatgpt/` is an additive adapter; original Python commands work only in a Python-enabled environment and must not be reported as executed by merely reading documentation.
- Project-specific/private facts stay in a private chat/workspace. Only neutral examples and templates live here.

## Evaluation / TEST
1. Static inspect that four adapter instructions map to the correct original skill.
2. Inspect numerical methodology for SaaS/subscription versus per-sale/day compatibility.
3. GitHub read-back of the exact branch/commit and files.
4. Optional local Python test suite, when execution environment with the repository is available. Mark NOT_RUN otherwise.
5. Manual user pilot on one private business case before further scope.

Rollback: close PR and delete feature branch; no schema, external side effects or product runtime changes.
Promotion: user accepts documented outputs first; then PR may be merged. No PROD concept in this research-only adapter.
