# Market Sizing and Opportunity Analyser

**Domain:** Market Research and Competitive Intelligence
**Level:** 🔵 Practitioner

> Produce a structured TAM/SAM/SOM analysis with documented assumptions and methodology. Investor-ready market sizing that can withstand scrutiny.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_OR_SERVICE]` | What you are selling | e.g. AI-powered compliance monitoring SaaS for financial services firms |
| `[GEOGRAPHY]` | The geographic market you are targeting | e.g. United Kingdom, initially; European expansion in Year 3 |
| `[TARGET_CUSTOMER_DEFINITION]` | Precise definition of the addressable customer | e.g. Chief Compliance Officers at FCA-regulated financial services firms with 50-500 employees |
| `[PRICING_MODEL]` | How you charge and at what price | e.g. Annual SaaS subscription at £18,000 per firm |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a market research analyst and venture strategy advisor with 15 years of experience producing investor-grade market sizing analyses. You have supported over 50 fundraising processes and know which market sizing methodologies hold up under investor scrutiny and which collapse at the first question.
</role>

<context>
Product or service: [PRODUCT_OR_SERVICE]
Geography: [GEOGRAPHY]
Target customer definition: [TARGET_CUSTOMER_DEFINITION]
Pricing model: [PRICING_MODEL]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Define the market sizing approach. Choose between top-down (industry reports to segment) and bottom-up (count of addressable customers multiplied by price) and justify the choice. For maximum credibility, use both and triangulate.

Step 2: Calculate TAM using the top-down approach. Identify the broadest relevant market category, find or estimate its size, and document the source or assumption basis.

Step 3: Calculate SAM using the bottom-up approach. Count the number of addressable customers matching the definition, multiply by annual contract value, and document the methodology.

Step 4: Calculate SOM. Apply realistic capture assumptions for Years 1, 3, and 5, based on comparable company trajectories or stated constraints.

Step 5: Identify the two most important growth tailwinds and the single most important risk to the market size assumption.

Step 6: Produce a one-paragraph investor narrative summarising the market opportunity in language suitable for a pitch deck.
</instructions>

<output_format>
Section 1: Methodology: one paragraph explaining approach and why it was chosen.
Section 2: Market Sizing Table: three rows (TAM / SAM / SOM). Columns: Level | Market Definition | Size Estimate | Methodology | Key Assumption.
Section 3: SOM Trajectory Table: three rows (Year 1 / Year 3 / Year 5). Columns: Year | Target Customers | Revenue | Market Share % | Capture Assumption.
Section 4: Market Dynamics: two tailwinds (one sentence each) and one risk (one sentence).
Section 5: Investor Narrative: one paragraph, 80 words maximum, suitable for a pitch deck market slide.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Every size estimate must have a documented assumption or source. No invented numbers.
- SOM capture rates must be credible for an early-stage company. Do not project 10% market share in Year 1.
- The investor narrative must be specific and compelling, not generic. No phrases like "massive opportunity" without numbers to support them.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. TAM, SAM, and SOM are all populated with methodology and assumptions.
2. SOM figures are mathematically consistent with SAM.
3. Market share percentages in SOM trajectory are credible for an early-stage company.
4. Investor narrative is 80 words or fewer and contains at least one specific number.
5. No invented statistics. All numbers have stated assumption basis.
</evaluation_criteria>
```

---

## Why This Works

Triangulating top-down and bottom-up approaches is the standard investors use to test market size claims. Most founders use only one method and produce a figure that cannot survive a follow-up question. Requiring documented assumptions for every number forces the founder to understand their market well enough to defend the analysis.

---

## Sample Output

Market Sizing row: SAM | FCA-regulated firms, 50-500 employees, with a compliance function | £540m | Bottom-up: 30,000 qualifying firms x £18,000 ACV | Assumption: all qualifying firms have budget authority and active compliance function, likely overstates by 40%, true SAM closer to £320m

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
