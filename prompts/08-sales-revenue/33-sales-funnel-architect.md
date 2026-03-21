# Sales Funnel Architect

**Domain:** Sales and Revenue Growth
**Level:** 🔵 Practitioner

> Design a complete sales funnel with stage definitions, entry criteria, exit criteria, conversion tactics, and metrics. Converts informal sales activity into a repeatable, measurable process.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_OR_SERVICE]` | What you sell | e.g. AI compliance monitoring SaaS at £18,000 ACV |
| `[SALES_MOTION]` | How you currently sell | e.g. Founder-led outbound: LinkedIn outreach to CCOs, discovery call, product demo, pilot proposal, contract |
| `[CURRENT_CONVERSION_DATA]` | Any data on your current funnel performance | e.g. 100 outreach attempts, 15 replies (15%), 8 discovery calls, 4 demos, 2 pilots, 1 closed deal |
| `[AVERAGE_DEAL_SIZE]` | Your average contract value | e.g. £18,000 ACV, 12-month contract, paid annually upfront |
| `[SALES_TEAM]` | Who does sales today | e.g. 1 founder doing all sales, approximately 8 hours per week |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a B2B sales architect with 15 years of experience designing sales processes for SaaS companies from founder-led through to scaled sales organisations. You understand that a sales funnel is not a CRM taxonomy: it is a set of defined buyer commitments that predict deal closure with measurable confidence.
</role>

<context>
Product or service: [PRODUCT_OR_SERVICE]
Sales motion: [SALES_MOTION]
Current conversion data: [CURRENT_CONVERSION_DATA]
Average deal size: [AVERAGE_DEAL_SIZE]
Sales team: [SALES_TEAM]
</context>

<instructions>
Step 1: Define the funnel stages. Each stage must represent a specific buyer commitment, not a seller activity. Use 5-6 stages.

Step 2: For each stage, define: entry criteria (what must be true for a prospect to enter this stage), exit criteria (what must happen to advance to the next stage), primary seller activity, and the most common reason deals stall at this stage.

Step 3: Calculate the current funnel metrics from the stated conversion data. Identify where the biggest drop-off occurs and why.

Step 4: Identify three specific improvements to the lowest-performing conversion point. Each improvement must be actionable and testable within 30 days.

Step 5: Project the impact of each improvement on monthly pipeline output and closed revenue.
</instructions>

<output_format>
Section 1: Funnel Stage Definitions. Table with Stage Name, Buyer Commitment, Entry Criteria, Exit Criteria, Primary Seller Activity, Most Common Stall Reason columns.
Section 2: Current Funnel Metrics. Table with Stage, Input Volume, Output Volume, Conversion Rate, and Assessment (Healthy / Needs Work / Critical) columns.
Section 3: Bottleneck Analysis. One paragraph identifying the primary bottleneck with the specific reason based on the stated data.
Section 4: Improvement Interventions. Three numbered interventions each with: What to Test, Why It Should Work, How to Measure, and Timeline.
Section 5: Impact Projection. Table with Intervention, Current Monthly Revenue Output, Projected Monthly Revenue Output, and Incremental Monthly Value columns.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Funnel stages must represent buyer commitments, not seller activities. "Demo sent" is a seller activity. "Prospect has evaluated core use case" is a buyer commitment.
- Conversion rates must be calculated from the actual data provided, not estimated.
- Improvement interventions must be testable in 30 days with the stated team size.
- Impact projections must show the mathematical basis for the revenue estimate.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All funnel stages are defined as buyer commitments.
2. Conversion rates are calculated from the actual stated data.
3. Bottleneck is identified at the specific stage with the lowest conversion rate.
4. Three interventions are testable within 30 days with a 1-person sales team.
5. Impact projection shows calculation basis.
</evaluation_criteria>
```

---

## Why This Works

Defining stages as buyer commitments rather than seller activities is the single most important structural shift in sales process design. It changes the question from 'what did we do' to 'what has the buyer decided,' which is the only metric that predicts revenue. The impact projection forces founders to quantify the value of process improvement, converting abstract sales hygiene into a concrete ROI argument for investing time in the fix.

---

## Sample Output

Funnel stage: Pilot Agreed | Buyer Commitment: Prospect has agreed to a structured 30-day pilot with defined success criteria | Entry Criteria: Economic buyer has verbally committed to proceed; success criteria agreed in writing | Exit Criteria: Pilot complete, success criteria reviewed, commercial conversation initiated | Most Common Stall: Success criteria not defined before pilot starts, leaving no objective basis for conversion conversation

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
