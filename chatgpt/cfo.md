# CFO feasibility adapter — subscription-safe guard

Original: `skills/founder-cfo/SKILL.md`, `skills/founder-cfo/unit_economics.py`.

The original `unit_economics.py` uses `plan_per_day` and `ramp_per_day` for a unit **sold** each day. It is suitable for compatible transactional businesses, but **not** an exact SaaS subscription model. Do not interpret daily 'client-month' transactions as monthly recurring subscriptions.

For a SaaS/B2B subscription business:
1. Intake explicit currency and period; starting paying customers; monthly new customers or acquisition range; monthly churn; recurring price/customer; per-customer recurring variable costs; monthly fixed costs; optional setup revenue/cost; acquisition spend and one-off startup costs.
2. Label each numeric input OWNER_REPORTED, VERIFIED_PUBLIC, MARKET_PROXY or ASSUMPTION, and mark unknown inputs MISSING.
3. Use transparent monthly cohort arithmetic in a private calculation environment when all needed assumptions are supplied:
   - retained_customers_t = active_customers_(t-1) * (1 - churn_t)
   - active_customers_t = retained_customers_t + new_customers_t
   - ending_MRR_t = active_customers_t * recurring_price_t (only if uniform plans; otherwise sum by cohort)
   - recurring_contribution_t = recurring_revenue_t - active_customers_t * per_customer_variable_cost_t
   - operating_result_t = recurring_contribution_t - fixed_cost_t - acquisition_spend_t
   - cumulative_cash_t = prior_cash + collections_t - cash_costs_t (not the same as profit)
4. If rounding fractional customers, state rounding policy; avoid false fractional customer forecasts. Recognize timing: ending MRR is a snapshot, not automatically month revenue, and accrual versus cash collections can differ.
5. Show pessimistic/base/optimistic scenarios by varying churn, new customers and price. Scenarios are **hypotheses**, not demand forecasts.
6. If numerical execution is unavailable, report formulas and `NOT_RUN`; do not imply Python was executed. If required inputs are missing, report a conditional sensitivity table only (e.g., needed subscribers at assumed price) and label the assumptions.

Output: input ledger, formula/audit trail, monthly scenarios only when complete, margin/break-even assumptions, runway/cash cautions and one real-world validation needed next. No prediction from a synthetic buyer-panel rate.
