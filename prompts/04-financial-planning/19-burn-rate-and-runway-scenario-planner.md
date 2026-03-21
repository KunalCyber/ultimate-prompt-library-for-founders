# Burn Rate and Runway Scenario Planner

**Domain:** Financial Planning and Modelling
**Level:** 🔵 Practitioner

> Model burn rate scenarios and calculate runway with trigger points for action. Ensures founders know exactly when they need to raise, cut, or accelerate revenue before they are in a crisis.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[CURRENT_CASH_BALANCE]` | Cash in the bank today | e.g. £380,000 |
| `[CURRENT_MONTHLY_BURN]` | Current monthly cash outflow net of any revenue | e.g. £32,000/month net burn (£38,000 costs minus £6,000 MRR) |
| `[REVENUE_GROWTH_ASSUMPTION]` | Expected revenue growth trajectory | e.g. Adding 1 new customer per month at £1,500 MRR from month 3, growing to 3 per month from month 7 |
| `[PLANNED_COST_CHANGES]` | Any known cost increases or decreases coming | e.g. Engineering hire at month 4 adds £9,000/month; if Series A closes by month 8, add £40,000/month in new headcount |
| `[FUNDRAISING_PLAN]` | When and how much you plan to raise | e.g. Targeting £1.5m seed round, aiming to close by month 7, with a 3-month process starting now |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a startup CFO and cash management advisor with 15 years of experience helping founding teams avoid running out of money. You are direct about cash realities, unsentimental about burn, and focused on giving founders the information they need to make decisions before options close.
</role>

<context>
Current cash balance: [CURRENT_CASH_BALANCE]
Current monthly burn: [CURRENT_MONTHLY_BURN]
Revenue growth assumption: [REVENUE_GROWTH_ASSUMPTION]
Planned cost changes: [PLANNED_COST_CHANGES]
Fundraising plan: [FUNDRAISING_PLAN]
</context>

<instructions>
Step 1: Calculate the base case runway. Using current burn and the stated revenue growth trajectory, calculate month-by-month net burn and cumulative cash balance through to zero. Identify the month cash runs out in the base case.

Step 2: Model three scenarios: Base Case (as stated), Conservative (revenue growth 50% slower than stated, costs as planned), and Optimistic (revenue growth 50% faster than stated, costs as planned).

Step 3: Identify three trigger points: (a) the date by which a fundraising process must begin to close before cash out, (b) the date by which a cost reduction decision must be made if fundraising does not close on time, and (c) the month at which the business reaches cash flow positive under the optimistic scenario.

Step 4: Calculate the fundraising buffer. How many months of runway does the stated fundraising plan create if it closes on the planned date? Is this sufficient?

Step 5: Identify the single most dangerous assumption in this cash model and quantify its impact.
</instructions>

<output_format>
Section 1: Base Case Runway Table: months 1-18 as rows. Columns: Month, Revenue, Gross Burn, Net Burn, Cumulative Cash Balance. Final row flags the month cash reaches zero.
Section 2: Scenario Comparison: table with Scenario, Revenue Assumption, Month Cash Runs Out, and Runway (months) columns.
Section 3: Trigger Points: three numbered trigger points, each with a specific date or month number and the action required.
Section 4: Fundraising Buffer Analysis: one paragraph with the calculation and a clear assessment (Sufficient / Tight / Insufficient).
Section 5: Most Dangerous Assumption: one paragraph naming the assumption and quantifying its impact on runway.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- All cash figures must be consistent across sections. Cumulative balance in Section 1 must match Section 2 base case.
- Trigger point dates must be calculated from the actual runway figures, not estimated.
- The fundraising buffer assessment must be honest. Six months of buffer after close is the minimum; less than four months is insufficient.
- The most dangerous assumption must be specific and quantified.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Base case runway table figures are internally consistent month-by-month.
2. Conservative and optimistic scenarios use the stated adjustment (50% slower/faster).
3. Trigger points are derived from actual runway figures, not generic advice.
4. Fundraising buffer is calculated from the specific close date and resulting cash position.
5. Most dangerous assumption includes a quantified impact on runway in months.
</evaluation_criteria>
```

---

## Why This Works

Founders consistently underestimate how long fundraising takes and overestimate how quickly revenue ramps. The three-scenario model forces a confrontation with the conservative case, which is often the realistic case. Trigger points convert the model into a decision calendar, ensuring founders act before options close rather than after.

---

## Sample Output

Trigger Point 2: Cost Reduction Decision Deadline, Month 5. If the seed round has not received at least one term sheet by Month 5, a cost reduction of £12,000/month (deferring the engineering hire and reducing marketing spend) extends the conservative case runway from Month 8 to Month 11, creating adequate time for a second fundraising attempt.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
