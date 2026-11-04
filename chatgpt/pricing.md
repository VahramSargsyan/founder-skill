# Pricing hypotheses adapter — not a fake willingness-to-pay result

Original: `skills/founder-pricing/SKILL.md`.

1. Identify billing metric (per customer/month, per seat/month, per project, usage-based, once) and geography/currency.
2. Distinguish **published competitor prices** from **real interview or survey answers** and **simulated personas**.
3. The original Van Westendorp Python tool needs four price answers per respondent. Run it only when responses exist and an execution tool is available; mark result REAL_SURVEY or SIMULATED. Without responses, do not output an 'optimal price' or invented acceptable interval.
4. Estimate break-even **candidate** subscription prices from documented costs and scenario counts, not from assumed demand.
5. Offer at most three transparent packages with scope and customer value; no invented 'was' anchor or fake scarcity.
6. Recommend a direct test (price shown to actual prospects and clear commitment metric). Do not use synthetic purchase rates as a success criterion.

Output: price hypotheses and source status, relative positioning vs substitutes, cost-floor sensitivity, two concrete prices to test, and a validation plan. If price or churn is MISSING, make uncertainty explicit.
