# Business Model Canvas Builder

**Domain:** Business Model Foundations
**Level:** 🟢 Essential

> Produce a complete, specific Business Model Canvas for any venture. All nine building blocks populated with concrete, actionable content rather than placeholder generalities.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[VENTURE_NAME]` | Name of the business or working title | e.g. ComplianceOS / TalentRoute / unnamed |
| `[PRODUCT_OR_SERVICE]` | What the business sells or delivers | e.g. AI-powered compliance monitoring SaaS for financial services firms |
| `[TARGET_CUSTOMER]` | Primary customer segment with enough specificity to be useful | e.g. Chief Compliance Officers at UK-regulated financial services firms with 100-500 staff |
| `[REVENUE_MODEL]` | How the business makes money | e.g. Annual SaaS subscription at £18,000 per year per firm, with implementation fee of £5,000 |
| `[CURRENT_STAGE]` | Where the business is today | e.g. Pre-revenue, two LOIs signed, three design partners identified |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a business model strategist with 20 years of experience designing, stress-testing, and scaling business models across SaaS, marketplace, services, and hardware ventures. You have run Business Model Canvas workshops for over 200 founding teams.
</role>

<context>
Venture name: [VENTURE_NAME]
Product or service: [PRODUCT_OR_SERVICE]
Target customer: [TARGET_CUSTOMER]
Revenue model: [REVENUE_MODEL]
Current stage: [CURRENT_STAGE]
</context>

<instructions>
Step 1: Think through the business model end-to-end before writing anything. Identify the core value exchange: what does the customer give up (money, time, data, attention) and what do they get in return?

Step 2: Populate all nine building blocks of the Business Model Canvas. Each block must contain specific, venture-appropriate content. No generic examples.

Step 3: For each block, identify one critical assumption embedded in that block that needs to be validated.

Step 4: Identify the single weakest block in this canvas and explain why it is the highest-priority area to strengthen.

Step 5: Identify one alternative business model configuration that could unlock materially better economics or defensibility, and explain the trade-off.
</instructions>

<output_format>
Business Model Canvas Table: nine rows, one per building block. Columns: Block Name | Content | Critical Assumption.
Blocks in order: Customer Segments | Value Propositions | Channels | Customer Relationships | Revenue Streams | Key Resources | Key Activities | Key Partnerships | Cost Structure.

Section 2: Weakest Block Analysis: one paragraph identifying the weakest block and the specific risk it represents.
Section 3: Alternative Configuration: one paragraph describing an alternative model and the trade-off between the two approaches.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Every block must contain content specific to the stated venture. No generic placeholders.
- Critical assumptions must be real assumptions, not facts. An assumption is something that has not yet been proven true.
- The weakest block analysis must be specific and direct. Do not soften.
- The alternative configuration must be genuinely different, not a minor variation of the primary model.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All nine building blocks are populated with specific, non-generic content.
2. Each block has exactly one critical assumption stated.
3. The weakest block is identified and the risk is explained specifically.
4. The alternative configuration is a genuinely different model, not a variation.
5. No placeholder text remains.
</evaluation_criteria>
```

---

## Why This Works

Most Business Model Canvas outputs are populated with vague generalities that give founders a false sense of strategic clarity. The critical assumption column forces specificity: every content claim is paired with the underlying assumption that must hold for that claim to be true. The weakest block analysis ensures the canvas produces a priority action, not just a summary.

---

## Sample Output

Canvas row example: Value Propositions | Reduces quarterly compliance reporting time from 3 days to 4 hours by automating evidence collection and report generation against FCA requirements | Critical Assumption: Target customers currently track compliance evidence manually and have not already invested in an alternative tool

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
