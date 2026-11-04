# ChatGPT adapter — first bounded pilot (4 of 11 methods)

This is an **additive prompt-level adapter**, not a native ChatGPT plugin and not an automatic installation. It references the original upstream methods, leaving all original Claude skills and Python scripts unmodified.

## Quick start
1. In a new ChatGPT conversation, provide the repository URL and paste `chatgpt/START_PROMPT.md` (or ask ChatGPT to read that exact file from the repository if access is available).
2. Describe the business idea with only information safe to share in a private chat. **Do not commit confidential evidence to this public fork.**
3. Work through board → competitors → pricing → CFO. Each can run independently. Ask for an evidence table first.
4. If there are too few actual customers, treat the result as **market and feasibility exploration**, not a validated sales forecast.
5. Before moving to the other seven modules, validate whether this pilot produced a decision that can be tested with a real buyer.

## Four adapted sources
- `chatgpt/board.md` → `skills/founder-board/SKILL.md` and `lenses.md`
- `chatgpt/competitors.md` → `skills/founder-competitors/SKILL.md`
- `chatgpt/pricing.md` → `skills/founder-pricing/SKILL.md`
- `chatgpt/cfo.md` → `skills/founder-cfo/SKILL.md`

Use `chatgpt/EVIDENCE_POLICY.md` in every stage and `chatgpt/B2B_SAAS_PILOT.md` for a low-data subscription-business example.

## What is deliberately NOT automatic
ChatGPT does not execute Claude Code `Agent` / `Task` subagents, expand `${CLAUDE_SKILL_DIR}`, or make slash commands work just because this GitHub folder exists. If a Python environment is unavailable, **do not claim** that the original `unit_economics.py` or `van_westendorp.py` ran. A narrative analysis is not a deterministic calculation.

The original CFO sample is a café with daily transactions. A subscription business needs a different customer-month/churn/recurring-revenue model. Do **not** copy café `plan_per_day` into SaaS and call the result MRR.
