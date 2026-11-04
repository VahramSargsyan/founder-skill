# Evidence contract — mandatory for ChatGPT pilot

For every material claim, show the value, unit/currency, period, status, origin, observed/retrieved date, and uncertainty.

| Status | Meaning | May support a factual conclusion? |
| --- | --- | --- |
| OWNER_REPORTED | Explicitly supplied by owner; not independently audited | Only as owner-reported |
| VERIFIED_PUBLIC | Accessible primary/reliable public source with exact URL and date | Yes, within source scope |
| MARKET_PROXY | External market analog, not the target business | Proxy only |
| ASSUMPTION | Explicit hypothetical parameter with a range and reason | Scenario only |
| SIMULATED | Synthetic persona or model-generated opinion | No real conversion/demand claim |
| MISSING | Not known, unavailable or not checked | No numeric substitution |

## Rules
1. No invented customers, companies, prices, reviews, metrics or conversions. If live browsing is unavailable, report `NOT_VERIFIED`, do not backfill from memory.
2. Use data as-of the decision date and name the intended market (e.g., Armenia vs international); avoid converting USD to AMD without an explicit rate, date and source.
3. Keep a clear line between cash collections, recognized revenue, MRR/ARR, contribution margin, operating profit and one-time setup fees.
4. For pre-revenue or low-data businesses, do not produce a 'probability of success' or an estimated buyer conversion percentage from an AI panel.
5. For financial estimates: show formulas, assumptions and sensitivity. Missing price/cost/volume must remain `MISSING`; avoid silently treating blanks as zero.
6. Pricing surveys: simulated answers are not willingness-to-pay evidence. The original Van Westendorp script may process synthetic data, but its result must be labelled `SIMULATED`, never a validated market price.
7. Do not leak private information into a public GitHub repository. Work products that use actual client records, user identities, nonpublic budgets or source code remain in private workspace.
8. A negative or inconclusive answer is acceptable. Favor a concrete next experiment over long speculative plans.

## Minimum answer structure
- Evidence we have (source, date, status).
- Questions still missing (max three owner-only questions; otherwise research independently).
- Three scenarios if grounded inputs permit them.
- Main uncertainty, failure modes, competing alternatives.
- One low-cost real-world validation experiment with a falsifiable pass/fail criterion.
- Verdict: `EXPLORATORY`, `TESTABLE_HYPOTHESIS`, `PARTIALLY_VALIDATED`, or `INSUFFICIENT_EVIDENCE`; never call speculative simulations a proven profitable business.
