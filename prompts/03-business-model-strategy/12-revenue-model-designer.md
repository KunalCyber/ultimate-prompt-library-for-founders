# Revenue Model Designer

**Domain:** Business Model and Strategy
**Level:** 🔵 Practitioner

> Evaluate and design the optimal revenue model with pricing logic, unit economics, and projection scaffolding. Move from 'we charge X' to a revenue architecture that scales.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_OR_SERVICE]` | What you are selling | e.g. AI compliance monitoring SaaS for financial services |
| `[TARGET_CUSTOMER]` | Who buys it | e.g. CCOs at FCA-regulated firms, 50-500 employees |
| `[CURRENT_PRICING_IDEA]` | What you are currently thinking of charging | e.g. £18,000 per year flat fee |
| `[COMPARABLE_PRODUCTS]` | Products customers currently pay for in this category | e.g. ComplyAdvantage at £30-80k/year, manual compliance consultant at £150k/year, spreadsheet tools at £0 |
| `[UNIT_ECONOMICS_TARGET]` | Your target gross margin | e.g. 75-80% gross margin at scale |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a SaaS pricing strategist and revenue model designer with 15 years of experience building pricing architectures for B2B software companies from pre-revenue through Series B. You understand value-based pricing, competitive anchoring, and the unit economics that investors require to fund a growth round.
</role>

<context>
Product or service: [PRODUCT_OR_SERVICE]
Target customer: [TARGET_CUSTOMER]
Current pricing idea: [CURRENT_PRICING_IDEA]
Comparable products: [COMPARABLE_PRODUCTS]
Unit economics target: [UNIT_ECONOMICS_TARGET]
</context>

<instructions>
Step 1: Evaluate three alternative revenue model types relevant to this product: (a) flat subscription, (b) usage-based or outcome-based, (c) tiered by company size or feature set. Score each on: Predictability, Scalability, Alignment with Customer Value, and Sales Cycle Simplicity.

Step 2: Recommend the optimal revenue model. Explain why it maximises value capture for this specific product and customer at this stage.

Step 3: Design the pricing architecture. Define tiers (if applicable), price points, and the value metric that drives pricing.

Step 4: Calculate the unit economics at the recommended price point: ACV, gross margin, CAC estimate, LTV, and LTV:CAC ratio.

Step 5: Identify one pricing risk and one expansion revenue opportunity embedded in this model.
</instructions>

<output_format>
Section 1: Revenue Model Evaluation: table with Model Type, Predictability (1-5), Scalability (1-5), Value Alignment (1-5), Sales Simplicity (1-5), and Total Score columns.
Section 2: Recommended Model: one paragraph with rationale.
Section 3: Pricing Architecture: table with Tier, Target Customer, Price, Included Features, and Value Metric columns.
Section 4: Unit Economics Table: ACV | Gross Margin % | Estimated CAC | LTV (3-year) | LTV:CAC Ratio.
Section 5: Pricing Risk and Expansion Opportunity: two one-paragraph blocks.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Unit economics must be mathematically consistent.
- LTV calculation must show the methodology (ACV x gross margin x average customer lifetime).
- LTV:CAC ratio must be realistic for an early-stage B2B SaaS company (3:1 minimum, 5:1 target).
- Pricing must be anchored against the comparables provided, not invented in isolation.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All three revenue model types are evaluated with scores.
2. Unit economics are mathematically consistent.
3. LTV:CAC ratio is calculated correctly.
4. Pricing architecture has tiers with specific prices and value metrics.
5. Pricing risk and expansion opportunity are specific to this product and model.
</evaluation_criteria>
```

---

## Why This Works

Most founders anchor their pricing on what feels comfortable to charge rather than on value delivered or competitive context. The comparative model evaluation produces a reasoned choice rather than a default. The unit economics output produces the exact figures a Series A investor will ask for on the first call.

---

## Sample Output

Unit Economics row: ACV: £18,000 | Gross Margin: 78% | Estimated CAC: £8,500 | LTV (3-year): £42,120 (£18,000 x 0.78 x 3) | LTV:CAC: 4.96:1, above 3:1 threshold, approaching 5:1 target

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
