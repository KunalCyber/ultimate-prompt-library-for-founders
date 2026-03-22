# Revenue Forecast and Financial Projection Builder

**Domain:** Financial Planning and Modelling
**Level:** 🔴 Advanced

> Build 12-month and 3-year revenue forecasts with investor-ready assumptions and scenario modelling. Produces the financial projections that accompany a Series A or seed funding deck.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[REVENUE_MODEL]` | How you charge | e.g. £18,000 ACV SaaS, billed annually, plus £5,000 one-time implementation fee |
| `[SALES_MOTION]` | How you acquire customers | e.g. Outbound sales-led: 1 SDR generating 80 leads/month, 20% to demo, 25% of demos to pilot, 30% pilot to close |
| `[CURRENT_ARR]` | Current annual recurring revenue | e.g. £36,000 ARR (2 customers) |
| `[HIRING_PLAN]` | Planned sales and revenue-generating hires | e.g. Month 4: 1 full-cycle AE at £65k; Month 7: 1 SDR at £40k; Year 2 Month 1: VP Sales at £120k plus 2 AEs |
| `[RETENTION_ASSUMPTION]` | Expected annual customer retention rate | e.g. 85% annual retention in Year 1 improving to 90% by Year 3 as product matures |
| `[EXPANSION_ASSUMPTION]` | Revenue expansion from existing customers | e.g. 15% net revenue retention from upsells (additional modules, seat expansion) from Year 2 |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a SaaS financial modeller and CFO advisor with 15 years of experience building revenue forecasts for seed through Series B companies. You have supported over 40 fundraising processes and understand exactly what investors require from a financial model: credible assumptions, documented methodology, scenario discipline, and honest sensitivity analysis.
</role>

<context>
Revenue model: [REVENUE_MODEL]
Sales motion: [SALES_MOTION]
Current ARR: [CURRENT_ARR]
Hiring plan: [HIRING_PLAN]
Retention assumption: [RETENTION_ASSUMPTION]
Expansion assumption: [EXPANSION_ASSUMPTION]
</context>

<instructions>
Think through this step by step. Build the model bottom-up from the sales motion before producing any outputs.

Step 1: Build the 12-month new customer acquisition model. Using the stated sales motion and hiring plan, calculate the number of new customers per month, new ARR added per month, and cumulative ARR at month 12.

Step 2: Apply the retention assumption to calculate monthly churn. Calculate net new ARR (new ARR minus churned ARR) and ending ARR per month for months 1-12.

Step 3: Extend to a 3-year view. Year 2 and Year 3 should show ARR at year-end, customer count, net revenue retention, and year-on-year growth rate.

Step 4: Run three scenarios for the 3-year view: Base Case (as stated), Conservative (20% fewer new customers, 5% higher churn), and Aggressive (20% more new customers, 5% lower churn, expansion revenue from Year 2).

Step 5: Identify the three most important milestones in the forecast that investors will focus on. For each, state what needs to be true for the milestone to be achieved.
</instructions>

<output_format>
Section 1: Monthly ARR Build (12 months): table with Month, New Customers, New ARR, Churned ARR, Net New ARR, and Ending ARR columns.
Section 2: 3-Year Summary: table with Year, Ending ARR, Customer Count, Net Revenue Retention %, and YoY Growth % columns.
Section 3: Scenario Comparison: table with Scenario, Year 1 Ending ARR, Year 2 Ending ARR, Year 3 Ending ARR, and Year 3 Customer Count columns.
Section 4: Key Investor Milestones: three numbered milestones, each with a Milestone Description, Target Date, and What Must Be True section.
Section 5: Assumption Register: table with every key assumption in the model, Assumption, Value, and Basis (stated input / market benchmark / comparable company) columns.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- All ARR figures must be internally consistent. Month 12 ending ARR must equal the sum of net new ARR across all months.
- Churn must be applied monthly, not annually, to avoid overstating ARR at year-end.
- Conservative scenario must not look worse than an investor could reasonably expect. Aggressive scenario must not require assumptions that have not been demonstrated.
- Assumption register must include every number used in the model, not just the obvious ones.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Month 12 ending ARR in Section 1 is the sum of net new ARR across all months.
2. 3-year summary YoY growth rates are calculated correctly.
3. Scenario comparison shows meaningful differentiation between cases.
4. Key milestones are specific to this company's stage and model.
5. Assumption register is complete, every number in the model has an entry.
</evaluation_criteria>
```

---

## Why This Works

Applying churn monthly rather than annually is a technical point that most early-stage founders get wrong, annual churn application overstates ARR at year-end and produces a flattering forecast that investors will immediately correct. The assumption register is the component most missing from founder models: making every assumption explicit allows investors to substitute their own views and creates a credible, transparent document.

---

## Sample Output

Monthly ARR Build row: Month 6 | New Customers: 3 | New ARR: £54,000 | Churned ARR: £1,350 (1.5% monthly churn on £90,000 base) | Net New ARR: £52,650 | Ending ARR: £162,650, note: churn applied to prior month ending ARR, not annual rate divided by 12

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
