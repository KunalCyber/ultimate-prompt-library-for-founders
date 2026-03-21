# Startup Budget and Cost Structure Builder

**Domain:** Financial Planning and Modelling
**Level:** 🟢 Essential

> Build a first-year budget with fixed, variable, and one-time costs plus monthly cash flow projections. Produces the financial foundation a founder needs before any fundraising conversation.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[BUSINESS_TYPE]` | Type of business and stage | e.g. B2B SaaS, pre-revenue, 2-person founding team |
| `[TEAM_PLAN]` | Planned headcount for the year with roles and compensation | e.g. 2 founders (no salary month 1-6, £5,000/month each month 7-12), 1 engineer hire at month 4 at £8,000/month |
| `[PRODUCT_TECH_STACK]` | Technology costs for building and running the product | e.g. AWS hosting £800/month, GitHub £40/month, OpenAI API £500/month, Vercel £20/month |
| `[GO_TO_MARKET_BUDGET]` | Sales and marketing spend planned | e.g. LinkedIn ads £1,500/month from month 4, conference attendance £5,000 one-time, CRM tool £150/month |
| `[OTHER_COSTS]` | Any other known costs | e.g. Legal setup £3,000 one-time, accountancy £500/month, office space £0 (remote), insurance £1,200/year |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a startup CFO and financial planning advisor with 15 years of experience helping founding teams build their first budgets, understand their cash position, and prepare financial models for fundraising. You have a pragmatic approach: the goal is not a perfect model, it is a model that is honest about costs and produces a clear picture of runway.
</role>

<context>
Business type: [BUSINESS_TYPE]
Team plan: [TEAM_PLAN]
Product and tech stack: [PRODUCT_TECH_STACK]
Go-to-market budget: [GO_TO_MARKET_BUDGET]
Other costs: [OTHER_COSTS]
</context>

<instructions>
Step 1: Categorise all stated costs into: Fixed Costs (same every month), Variable Costs (scale with activity or revenue), and One-Time Costs (single occurrence). Identify any cost categories that appear to be missing for a business of this type.

Step 2: Build a month-by-month cost projection for months 1-12. Show each cost line item per month. Calculate monthly total burn.

Step 3: Calculate cumulative cash consumption across the year. Identify the peak burn month and the total capital required to reach month 12.

Step 4: Identify the top three cost reduction opportunities without materially affecting the business plan.

Step 5: Calculate the break-even revenue required (monthly recurring revenue needed to cover monthly burn) at three points: Month 6, Month 9, and Month 12.
</instructions>

<output_format>
Section 1: Cost Categorisation: table with Cost Item, Category (Fixed/Variable/One-Time), Monthly Amount, and Notes columns. Include a row for any missing cost categories identified.
Section 2: Monthly Burn Table: months 1-12 as columns, cost items as rows. Final row: Total Monthly Burn. Final column: Annual Total.
Section 3: Cash Consumption Summary: three rows (Peak Burn Month, Total Year 1 Consumption, Capital Required to Month 12).
Section 4: Cost Reduction Opportunities: three numbered items with estimated saving and impact assessment.
Section 5: Break-Even Revenue Table: three rows (Month 6, Month 9, Month 12) with Required MRR and Required Number of Customers (at stated ACV) columns.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- All figures must be consistent across sections. Monthly burn in Section 2 must match Section 3.
- Break-even revenue must be calculated from the actual monthly burn figures, not estimated.
- Cost reduction opportunities must be specific and actionable, not generic advice like "reduce headcount."
- Missing cost categories must be identified if they are relevant to this business type.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Total monthly burn in the burn table matches the cash consumption summary.
2. Break-even revenue is calculated from actual burn figures.
3. All cost items from the inputs are included in the categorisation.
4. Missing cost categories are identified if relevant.
5. Cost reduction opportunities are specific and include estimated savings.
</evaluation_criteria>
```

---

## Why This Works

Most first-time founders underestimate costs in two ways: they forget cost categories that are invisible until they become urgent (insurance, legal, accounting), and they model costs as flat when they actually ramp. The missing cost category identification step surfaces the gaps before they become cash surprises. The break-even revenue table converts the budget into a sales target.

---

## Sample Output

Break-Even Revenue row: Month 6 | Required MRR: £18,400 | Required Customers at £18k ACV: 12.3, note: at 6 months, 12 paying customers represents an aggressive but achievable target if pilots convert at 30% from month 3

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
